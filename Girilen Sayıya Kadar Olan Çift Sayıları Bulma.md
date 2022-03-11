# Proje Sahibi: Patika.Dev 
# Proje Konusu: Başlangıç Seviye Java ile Backend Web Development Patikası
## Konu : Java101

#### Soru> Girilen Sayıya Kadar Olan Çift Sayıları Bulan Program:
- Java döngüler ile kullanıcının girdiği sayıya kadar çift olan sayıları bulan programı yazıyoruz.
- Java döngüler ile 0'dan girilen sayıya kadar olan sayılardan 3 ve 4'e tam bölünen sayıların ortalamasını hesaplayan programı yazınız.

```java
import java.util.Scanner;
public class Main
{
	public static void main(String[] args) {
	    int sayi;
	    int result=0;
	    int sayac=0;
	    
	    Scanner input= new Scanner(System.in);
	    System.out.print("Sayi giriniz :")
	    sayi=input.nextInt();
	    
	    for(int i=1; i<=sayi;i++){
	        if(i%2==0 && i%3==0 && i%4==0){
	            result+=i;
	            sayac+=1;
	        }
	    }
	    int sonuc=result/sayac;
	    System.out.println(sonuc);
}}
```

