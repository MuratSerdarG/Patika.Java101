# Proje Sahibi: Patika.Dev 
# Proje Konusu: Başlangıç Seviye Java ile Backend Web Development Patikası
## Konu : Java101

#### Soru> KDV Tutarı Hesaplayan Program:
- Java ile kullanıcıdan alınan para değerinin KDV'li fiyatını ve KDV tutarını hesaplayıp ekrana bastıran programı yazın.
- Örn: "KDV tutarını 18% olarak alın, KDV'siz Fiyat = 10, KDV'li Fiyat = 11.8, KDV tutarı = 1.8" şeklinde.
-Eğer girilen tutar 0 ve 1000 TL arasında ise KDV oranı %18 , tutar 1000 TL'den büyük ise KDV oranını %8 olarak KDV tutarı hesaplayan programı yazınız.


```java
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner deger = new Scanner(System.in);
        
        float fy;   //Degiskeni float olarak ayarliyoruz.
        
        System.out.println("Lutfen almak istediginiz urunun fiyatini giriniz : ");    //Urunun fiyatini input olarak istiyoruz.
        fy = deger.nextFloat();                                                       //Gelen input degerini degiskene esitliyoruz.

        int oran=(fy> 1000) ? 8:18; //KDV oranini buluyoruz.
        float kdv2=(fy*oran)/100; //KDV tutarini buluyoruz.
        float top3=fy+kdv2;     //Toplam bedeli buluyoruz.
        
        System.out.println("Almak istediginiz urunun fiyati : " + fy+" TL'dir.");     //Urun fiyatini yazdiriyoruz.
        System.out.println("Urununuzun KDV oranı : %" + oran +" ,KDV bedeli ise : " + kdv2+" TL'dir.");   //KDV orani ve fiyatini yazdiriyoruz.
        System.out.println("Urunun KDV dahil fiyati : " + top3+" TL'dir.");   //Toplam fiyati yazdiriyoruz.
    }
}
```

