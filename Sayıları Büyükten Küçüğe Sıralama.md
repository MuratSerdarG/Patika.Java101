# Proje Sahibi: Patika.Dev 
# Proje Konusu: Başlangıç Seviye Java ile Backend Web Development Patikası
## Konu : Java101

#### Soru> Sayıları Büyükten Küçüğe Sıralama:
- Girilen 3 sayıyı "küçükten büyüğe" sıralayan programı yazınız.

```java
import java.util.Scanner;
public class Main
{
	public static void main(String[] args) {
	    int a,b,c;
	    
	    Scanner deger = new Scanner(System.in);
	    
	    System.out.println("1. sayi degeri : ");
	    a=deger.nextInt();
	    System.out.println("2. sayi degeri : ");
	    b=deger.nextInt();
	    System.out.println("3. sayi degeri : ");
	    c=deger.nextInt();
	    
	    if(a==b || a==c || b==c){
            System.out.println("Sayilar arasinda esitlik bulunmaktadir. Lutfen kontrol ediniz. Siralama gecersiz.");
        }else if(a>b && a>c){
	        if(b>c){
	            System.out.println(" 1. sayi > 2. sayi > 3. sayi :\n"+a+" > "+b+" > "+c);
	        }else{
	            System.out.println(" 1. sayi > 3. sayi > 2. sayi :\n"+a+" > "+c+" > "+b);
	    }}else if(b>a  &&  b>c){
	        if(a>c){
	            System.out.println(" 2. sayi > 1. sayi > 3. sayi :\n"+b+" > "+a+" > "+c);
	        }else{
	            System.out.println(" 2. sayi > 3. sayi > 1. sayi :\n"+b+" > "+c+" > "+a);
        }}else{
	        if(a>b){
	            System.out.println(" 3. sayi > 1. sayi > 2. sayi :\n"+c+" > "+a+" > "+b);
	        }else{
	            System.out.println(" 3. sayi > 2. sayi > 1. sayi :\n"+c+" > "+b+" > "+a);
        }}
        
    }
}
```
