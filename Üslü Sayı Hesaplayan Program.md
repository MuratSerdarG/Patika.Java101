# Proje Sahibi: Patika.Dev 
# Proje Konusu: Başlangıç Seviye Java ile Backend Web Development Patikası
## Konu : Java101

#### 1. Üslü Sayı Hesaplayan Program:
- Java ile kullanıcının girdiği değerler ile üslü sayı hesaplayan programı yazıyoruz.
- Java ile kullanıcının girdiği değerler ile üslü sayı hesaplayan programı "For Döngüsü" kullanarak yapınız.

```java
import java.util.Scanner;
public class Main
{
	public static void main(String[] args) {
	    
	    int sayi,sayi2; 
	    
	    Scanner input = new Scanner(System.in);
	    
	    int sonuc=1;
        
        System.out.println("Kuvvetini alacaginiz sayiyi giriniz : ");   
        sayi = input.nextInt();
        System.out.println("Kuvvet bilgisini giriniz : ");   
        sayi2 = input.nextInt();
        
        for(int i=1;i<=(sayi2);i++){
            sonuc=sayi*sonuc;
        }
        System.out.println("İsleminizin sonucu : "+sonuc);
	}
}
```

