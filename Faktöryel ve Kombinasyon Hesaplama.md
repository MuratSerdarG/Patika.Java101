# Proje Sahibi: Patika.Dev 
# Proje Konusu: Başlangıç Seviye Java ile Backend Web Development Patikası
## Konu : Java101

#### 1. Faktöriyel Hesaplayan Program:
- Java ile faktöriyel hesaplayan program yazıyoruz.
- N elemanlı bir kümenin elemanları ile oluşturulacak r elemanlı farklı grupların sayısı n’in r’li kombinasyonu olarak adlandırılır. N’in r’li kombinasyonu C(n,r) şeklinde gösterilir.
- Java ile kombinasyon hesaplayan program yazınız.
-Kombinasyon formülü : C(n,r) = n! / (r! * (n-r)!)

```java
import java.util.Scanner;
public class Main
{
	public static void main(String[] args) {
	    
	    int sayi,eleman,grup; 
	    
	    Scanner input = new Scanner(System.in);
	    
	    int sonuc=1;
        
        System.out.println("Lutfen faktoryel alacaginiz sayiyi giriniz : ");   
        sayi = input.nextInt();
        
        System.out.println("Lutfen kume eleman sayisini giriniz : ");   
        eleman = input.nextInt();
        System.out.println("Lutfen kacli grup istediginizi giriniz : ");   
        grup = input.nextInt();
        
        for(int i=1;i<=(sayi);i+=1){
            sonuc=sonuc*i;
        }
        int deger1=1;
        int deger2=1;
        int deger3=1;
        int formul=eleman-grup;
        
        for(int i=1;i<=(eleman);i+=1){
            deger1=deger1*i;
        }
        for(int i=1;i<=(grup);i+=1){
            deger2=deger2*i;
        }
        for(int i=1;i<=(formul);i+=1){
            deger3=deger3*i;
        }
        int komb=deger1/(deger2*deger3);
        System.out.println("Faktoryel sonucunuz : "+sonuc);
        System.out.println("Kombinasyon sonucunuz : "+komb);
	}
}
```

