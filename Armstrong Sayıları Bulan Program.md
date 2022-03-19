# Proje Sahibi: Patika.Dev 
# Proje Konusu: Başlangıç Seviye Java ile Backend Web Development Patikası
## Konu : Java101

#### Armstrong Sayıları Bulan Program:
- Java döngüler ile sayının armstrong sayı olup olmadığını bulan programı yazıyoruz.
- Bir sayının basamak sayılarının toplamını hesaplayan program yazınız.
- Örnek : 1643 = 1 + 6 + 4 + 3 = 14
```java
import java.util.Scanner;

public class Main {
 public static void main(String[] args) {
	Scanner input=new Scanner(System.in);
	System.out.print("Sayıyı giriniz:");
	int number,toplam=0;
	
	number=input.nextInt();
		
	while(number!=0) {
		int rakam=number%10;
		toplam=rakam+toplam;
		number=number/10;
		}
	System.out.println("Değerler toplamı:"+toplam);
	}
}
```

