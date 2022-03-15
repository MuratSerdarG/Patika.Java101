# Proje Sahibi: Patika.Dev 
# Proje Konusu: Başlangıç Seviye Java ile Backend Web Development Patikası
## Konu : Java101

#### 1. Girilen Sayıdan Küçük 2’nin Kuvvetlerini Bulan Program:
- Java döngüler ile girilen sayıya kadar olan 2'nin kuvvetlerini ekrana yazdıran programı yazıyoruz.
- Java döngüler ile girilen sayıya kadar olan 4 ve 5'in kuvvetlerini ekrana yazdıran programı yazıyoruz.

```java
import java.util.Scanner;
public class Main
{
	public static void main(String[] args) {
	    
	    int sayi; 
	    
	    Scanner input = new Scanner(System.in);
        
        
        
        System.out.println("Lutfen sayiyi giriniz : ");   
        sayi = input.nextInt();
        System.out.println("2'nin katlari");
        for(int i=1;i<=(sayi);i*=2){
            System.out.println(i);
        }
        System.out.println("4'un katlari");
        for(int i=1;i<=(sayi);i*=4){
            System.out.println(i);
        }
        System.out.println("5'in katlari");
        for(int i=1;i<=(sayi);i*=5){
            System.out.println(i);
        }
	}
}
```

