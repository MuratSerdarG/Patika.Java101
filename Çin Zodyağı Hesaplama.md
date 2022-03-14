# Proje Sahibi: Patika.Dev 
# Proje Konusu: Başlangıç Seviye Java ile Backend Web Development Patikası
## Konu : Java101

#### 1.Çin Zodyağı Hesaplama:
- Java ile kullanıcıdan doğum tarihini alıp Çin Zodyağı değerini hesaplayan program yazınız.
- Çin Zodyağı nedir? 4000 bin yıldır kullanılan bir astroloji çeşididir Çin astrolojisi ve insanları 12 değişik burç ve sembollerle tanımlar. Çin Zodyağı bu 12 burcun eşit aralıklarla(10 derece genişliğinde) sıralandığı bir hayvan halkasıdır ve yıldızlarla pek bir ilgisi yoktur.
- Çin Zodyağı nasıl hesaplanır? Çin zodyağı hesaplanırken kişinin doğum yılının 12 ile bölümünde kalana göre bulunur.
- Doğum Tarihi %12 = 0 ➜ Maymun
- Doğum Tarihi %12 = 1 ➜ Horoz
- Doğum Tarihi %12 = 2 ➜ Köpek
- Doğum Tarihi %12 = 3 ➜ Domuz
- Doğum Tarihi %12 = 4 ➜ Fare
- Doğum Tarihi %12 = 5 ➜ Öküz
- Doğum Tarihi %12 = 6 ➜ Kaplan
- Doğum Tarihi %12 = 7 ➜ Tavşan
- Doğum Tarihi %12 = 8 ➜ Ejderha
- Doğum Tarihi %12 = 9 ➜ Yılan
- Doğum Tarihi %12 = 10 ➜ At
- Doğum Tarihi %12 = 11 ➜ Koyun

```java
import java.util.Scanner;
public class Main{
	public static void main(String[] args) {
	    
	    int dogumyili;
	    
	    Scanner input= new Scanner(System.in);
	    System.out.println("Lutfen dogum tarihinizi yil olarak giriniz : ");
	    dogumyili=input.nextInt();
	    
	    double zodyak=dogumyili%12;
	    String sonuc="";
	    
	    
	    if(zodyak==0){
	        sonuc="Maymun";
	    }else if(zodyak==1){
	        sonuc="Horoz";
	    }else if(zodyak==2){
	        sonuc="Köpek";
	    }else if(zodyak==3){
	        sonuc="Domuz";
	    }else if(zodyak==4){
	        sonuc="Fare";
	    }else if(zodyak==5){
	        sonuc="Öküz";
	    }else if(zodyak==6){
	        sonuc="Kaplan";
	    }else if(zodyak==7){
	        sonuc="Tavşan";
	    }else if(zodyak==8){
	        sonuc="Ejderha";
	    }else if(zodyak==9){
	        sonuc="Yılan";
	    }else if(zodyak==10){
	        sonuc="At";
	    }else if(zodyak==11){
	        sonuc="Koyun";
	    }else{
	        System.out.println("Hatali giris yaptiniz.");
	    }
	    System.out.println("Çin Zodyağı Burcunuz : "+ sonuc);
    }
}
```

