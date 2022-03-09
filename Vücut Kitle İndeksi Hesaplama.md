# Proje Sahibi: Patika.Dev 
# Proje Konusu: Başlangıç Seviye Java ile Backend Web Development Patikası
## Konu : Java101

#### Soru> Vücut Kitle İndeksi Hesaplama:
- Java ile kullanıcıdan boy ve kilo değerlerini alıp bir değişkene atayın. Aşağıdaki formüle göre kullanıcının "Vücut Kitle İndeks" değerini hesaplayıp ekrana yazdırın.
- Formül : Kilo (kg) / Boy(m) * Boy(m)

```java
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner deger = new Scanner(System.in);
        
        float boy,kilo;   //Degiskeni float olarak ayarliyoruz.
        
        System.out.println("Lutfen boyunuzu metre cinsinden giriniz : ");          //Boy bilgisini input olarak istiyoruz.
        boy = deger.nextFloat();                                                                   //Gelen input degerini degiskene esitliyoruz.
        System.out.println("Lutfen kilonuzu giriniz : ");          //Agırlık bilgisini input olarak istiyoruz.
        kilo = deger.nextFloat();                                                                   //Gelen input degerini degiskene esitliyoruz.

        float sonuc=(kilo)/(boy*boy);
        
        System.out.println("Vücut kitle indeksiniz: "+sonuc);         //Sonucu yazdiriyoruz.
        }
}
```
