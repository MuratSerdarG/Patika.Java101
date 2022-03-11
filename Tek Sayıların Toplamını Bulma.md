# Proje Sahibi: Patika.Dev 
# Proje Konusu: Başlangıç Seviye Java ile Backend Web Development Patikası
## Konu : Java101

#### Soru> Tek Sayıların Toplamını Bulan Program:
- Java döngüler ile negatif bir değer girilene kadar kullanıcıdan girişleri kabul eden ve girilen değerlerden tek sayıları toplayıp ekrana basan programı yazıyoruz.
- Java döngüler ile tek bir sayı girilene kadar kullanıcıdan girişleri kabul eden ve girilen değerlerden çift ve 4'ün katları olan sayıları toplayıp ekrana basan programı yazıyoruz.
- *NOT: * **Sorunun ismi tek sayıları bulmak fakat sorunun içeriğinde 4 e bölünebilen sayıları istemekte.**

```java
import java.util.Scanner;
public class Main{
	public static void main(String[] args) {
	    
	    int number;
	    int total=0;
	    
	    Scanner input= new Scanner(System.in);
	    
	    do{
	        System.out.print("Sayi giriniz :");
	        number=input.nextInt();
	        
	        if(number%4==0){
	            total+=number;
	       }
	       }while(number%2==0);
	        System.out.print("Toplama sonucu = "+total);
	    }
}
```

