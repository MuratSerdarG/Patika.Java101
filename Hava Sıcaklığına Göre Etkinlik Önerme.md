# Proje Sahibi: Patika.Dev 
# Proje Konusu: Başlangıç Seviye Java ile Backend Web Development Patikası
## Konu : Java101

#### Soru> Hava Sıcaklığına Göre Etkinlik Önerme:
- Aynı örnek üzerinden if koşulları başka hangi şekilde oluşturulabilirdi farklı çözüm yolları bulunuz.
- Sıcaklık 5'dan küçük ise "Kayak" yapmayı öner.
- Sıcaklık 5 ve 15 arasında ise "Sinema" etkinliğini öner.
- Sıcaklık 15 ve 25 arasında ise "Piknik" etkinliğini öner.
- Sıcaklık 25'ten büyük ise "Yüzme" etkinliğini öner.

```java
import java.util.Scanner;
public class Main
{
	public static void main(String[] args) {
	    int fah;
	    
	    Scanner derece = new Scanner(System.in);
	    
	    System.out.println("Lutfen beklenen sicaklik degerini giriniz : ");
	    fah=derece.nextInt();
	    
	    if(fah<=5){
	        System.out.println("Hava biraz soguk gibi. Bu havada cok guzel kayak yapilir.");
	    }else if(fah>5 && fah<=15){
	        System.out.println("Riske girmeye gerek yok gibi. Bu havada en iyisi sinemaya gitmek.");
	    }else if(fah>15 && fah<25){
	        System.out.println("Bu havada gunes kendini guzel gosterir. Bu havada en iyisi yesillikler icinde bir piknik.");
	    }else if(fah>=25){
	        System.out.println("Hava cok sicak ve bunaltici. Bu havada en iyisi serin sularda yuzmek olacaktir.");
	    }
    }
}
```
