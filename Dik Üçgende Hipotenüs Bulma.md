# Proje Sahibi: Patika.Dev 
# Proje Konusu: Başlangıç Seviye Java ile Backend Web Development Patikası
## Konu : Java101

#### Soru> Dik Üçgende Hipotenüs Bulan Program:
- Java ile kullanıcıdan dik kenarlarının uzunluğunu alan ve hipotenüsü hesaplayan programı yazın..
- Üç kenar uzunluğunu kullanıcıdan aldığınız üçgenin alanını hesaplayan programı yazınız.
- Formül olarak şunları kullanın : Üçgenin cevresi= 2u // u = (a+b+c) / 2 // Alan * Alan = 𝑢 * (𝑢 − 𝑎)* (𝑢 − 𝑏) * (𝑢 − 𝑐)

```java
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner deger = new Scanner(System.in);
        
        int akenar,bkenar,ckenar;   //Degiskenleri int olarak ayarliyoruz.
        
        System.out.println("Lutfen almak istediginiz urunun fiyatini giriniz : ");      //A kenar uzunlugunu input olarak istiyoruz.
        akenar = deger.nextInt();                                                       //Gelen input degerini degiskene esitliyoruz.
        System.out.println("Lutfen almak istediginiz urunun fiyatini giriniz : ");      //B kenar uzunlugunu input olarak istiyoruz.
        bkenar = deger.nextInt();                                                       //Gelen input degerini degiskene esitliyoruz.
        System.out.println("Lutfen almak istediginiz urunun fiyatini giriniz : ");      //C kenar uzunlugunu input olarak istiyoruz.
        ckenar = deger.nextInt();                                                       //Gelen input degerini degiskene esitliyoruz.

        
        int cevre=(akenar+bkenar+ckenar);   //Cevreyi buluyoruz.
        int form1=cevre/2;                  //Cevreyi formule uyduruyoruz.
        int form2=(form1)*(form1-akenar)*(form1-bkenar)*(form1-ckenar); //Alan icin formul olusturuyoruz.
        double alan=Math.sqrt(form2);       //Alani buluyoruz.
        
        System.out.println("Ucgenimizin a kenar uzunlugu : " + akenar +"cm, b kenar uzunlugu : " + bkenar +"cm, c kenar uzunlugu : "+ ckenar +"cm seklindedir.");     //Urun fiyatini yazdiriyoruz.
        System.out.println("Ucgenimizin cevresi : " + cevre +" seklindedir.");     //Urun fiyatini yazdiriyoruz.
        System.out.println("Ucgenimizin alanı : " + alan +" seklindedir.");     //Urun fiyatini yazdiriyoruz.
    }
}
```

