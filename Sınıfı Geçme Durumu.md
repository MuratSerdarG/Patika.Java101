# Proje Sahibi: Patika.Dev 
# Proje Konusu: Başlangıç Seviye Java ile Backend Web Development Patikası
## Konu : Java101

#### Soru> Sınıfı Geçme Durumunu Gösteren Program:
- Eğer girilen ders notları 0 veya 100 arasında değil ise ortalamaya katılmasın.
- Dersler : Matematik, Fizik, Türkçe, Kimya, Müzik
- Geçme Notu : 55


```java
import java.util.Scanner;
public class Main
{
	public static void main(String[] args) {
	    int mat,fiz,tur,kim,muz;
	    
	    Scanner not= new Scanner(System.in);
	    
	    System.out.println("Matematik notunuz : ");
	    mat=not.nextInt();
	    System.out.println("Fizik notunuz : ");
	    fiz=not.nextInt();
	    System.out.println("Turkce notunuz : ");
	    tur=not.nextInt();
	    System.out.println("Kimya notunuz : ");
	    kim=not.nextInt();
	    System.out.println("Muzik notunuz : ");
	    muz=not.nextInt();
	    
	    double ort=(mat+fiz+tur+kim+muz)/5;
	    
	    if(mat<0 || mat>100 || fiz<0 || fiz>100 || tur<0 || tur>100 || kim<0 || kim>100 || muz<0 || muz>100){
	        System.out.println("Girilen notlardan en az bir tanesi gecersizdir.");
	    }else{
	        System.out.println("Ortalamaniz : "+ort);
	        if (ort<55){
	            System.out.println("Not ortalamaniz yetersizdir. Sinif tekrari yapmaniz gerekmektedir.");
	        }else{
	            System.out.println("Tebrikler gectiniz.");
	        }
	    }
    }
}
```
