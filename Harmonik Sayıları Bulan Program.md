# Proje Sahibi: Patika.Dev 
# Proje Konusu: Başlangıç Seviye Java ile Backend Web Development Patikası
## Konu : Java101

#### Harmonik Sayıları Bulan Program:
- Java ile girilen sayının harmonik serisini bulan program yazacağız.
- 
```java
import java.util.Scanner;

public class Main {
 public static void main(String[] args) {
	Scanner input=new Scanner(System.in);
	System.out.print("Sayı giriniz:");
		
	int number=input.nextInt();
	double start=0.0;

	for(int i=1;i<=number;i++){
		start+=	(1.0/i);
	}
	System.out.println("Değerler toplamı:"+start);
	}
}
```

