# Proje Sahibi: Patika.Dev 
# Proje Konusu: Başlangıç Seviye Java ile Backend Web Development Patikası
## Konu : Java101

#### Soru> Taksimetre Programı:
- Java ile gidilen mesafeye (KM) göre taksimetre tutarını ekrana yazdıran programı yazın.
- Taksimetre KM başına 2.20 TL tutmaktadır.
- Minimum ödenecek tutar 20 TL'dir. 20 TL altında ki ücretlerde yine 20 TL alınacaktır.
- Taksimetre açılış ücreti 10 TL'dir.

```java
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner deger = new Scanner(System.in);
        
        float toplamkm;   //Degiskeni float olarak ayarliyoruz.
        
        System.out.println("Lutfen gitmek istediginiz mesafenin km bilgisini giriniz : ");          //Taksinin gittigi km bilgisini input olarak istiyoruz.
        toplamkm = deger.nextFloat();                                                              //Gelen input degerini degiskene esitliyoruz.

        
        int min=20;                                 //Minimum ucreti belirliyoruz.
        double ilk=10;                              //Acilis ucretını belirliyoruz.
        double tutar=ilk+(toplamkm*2.2);            //Normal Tutarı belirliyoruz.
        double ücret= (tutar < 20 ) ? 20 : tutar;   // Minimum tutara gore kıyaslama yapiliyor.
        

        System.out.println("Toplam gitmek istediginiz mesafe " + toplamkm +" km.");         //Toplam mesafeyi yazdiriyoruz.
        System.out.println("Bu mesafe icin odemeniz gereken tutar "+ücret+" TL'dir");       //Toplam ucreti yazdiriyoruz.
    }
}
```

