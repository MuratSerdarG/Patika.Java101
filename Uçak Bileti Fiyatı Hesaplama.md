# Proje Sahibi: Patika.Dev 
# Proje Konusu: Başlangıç Seviye Java ile Backend Web Development Patikası
## Konu : Java101

#### 1.Uçak Bileti Fiyatı Hesaplama:
- Java ile mesafeye ve şartlara göre uçak bileti fiyatı hesaplayan programı yapın. Kullanıcıdan Mesafe (KM), yaşı ve yolculuk tipi (Tek Yön, Gidiş-Dönüş) bilgilerini alın. Mesafe başına ücret 0,10 TL / km olarak alın. İlk olarak uçuşun toplam fiyatını hesaplayın ve sonrasında ki koşullara göre müşteriye aşağıdaki indirimleri uygulayın ;
- Kullanıcıdan alınan değerler geçerli (mesafe ve yaş değerleri pozitif sayı, yolculuk tipi ise 1 veya 2) olmalıdır. Aksi takdirde kullanıcıya "Hatalı Veri Girdiniz !" şeklinde bir uyarı verilmelidir.
- Kişi 12 yaşından küçükse bilet fiyatı üzerinden %50 indirim uygulanır.
- Kişi 12-24 yaşları arasında ise bilet fiyatı üzerinden %10 indirim uygulanır.
- Kişi 65 yaşından büyük ise bilet fiyatı üzerinden %30 indirim uygulanır.
- Kişi "Yolculuk Tipini" gidiş dönüş seçmiş ise bilet fiyatı üzerinden %20 indirim uygulanır.

```java
import java.util.Scanner;
public class Main{
	public static void main(String[] args) {
	    
	    int yas,km,yon;
	    double sonuc;
	    
	    Scanner input= new Scanner(System.in);
	    
	    System.out.println("Lutfen yasinizi giriniz: ");
	    yas=input.nextInt();
	    System.out.println("Lutfen gitmek istediginiz mesafeyi km cinsinden giriniz: ");
	    km=input.nextInt();
	    System.out.println("Lutfen seyahat seklinizi seciniz.\nTek yon yolculuk icin : 1\nGidis donus icin : 2");
	    yon=input.nextInt();
	    
	    double tutar=km*0.10;
	    
	    if(yas<1 || km<1 || yon<1 || yon>2){
	        System.out.println("Hatalı Veri Girdiniz !");
	    }else{
	        if(yas<12 && yon==1){
	            sonuc=tutar*0.50;   
        	}else if(yas<12 && yon==2){
    	        sonuc=(tutar*2*0.50)*0.80;
            }else if(yas>=12 && yas <=24 && yon==1){
        	    sonuc=tutar*0.90;   
        	}else if(yas>=12 && yas <=24 && yon==2){
        	    sonuc=((tutar*2)*0.90)*0.80;
        	}else if(yas>65 && yon==1){
        	    sonuc=tutar*0.70;
        	}else if(yas>65 && yon==2){
        	    sonuc=(tutar*2*0.70)*0.80;
        	}else if(yas>25 && yas<=65 && yon==1){
        	    sonuc=tutar;
        	}else{
        	    sonuc=tutar*2;
        	}
        	System.out.println("Odenmesi gereken toplam tutar : "+ sonuc +" TL'dir.");
    	}
    }
}
```

