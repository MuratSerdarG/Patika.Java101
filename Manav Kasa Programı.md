# Proje Sahibi: Patika.Dev 
# Proje Konusu: Başlangıç Seviye Java ile Backend Web Development Patikası
## Konu : Java101

#### Soru> Manav Kasa Programı:
- Java ile kullanıcıların manavdan almış oldukları ürünlerin kilogram değerlerine göre toplam tutarını ekrana yazdıran programı yazın.
- Meyveler ve KG Fiyatları : Armut : 2,14 TL; Elma : 3,67 TL; Domates : 1,11 TL; Muz: 0,95 TL; Patlıcan : 5,00 TL.

```java
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner deger = new Scanner(System.in);
        
        float armut,elma,domat,muz,pat;   //Degiskeni float olarak ayarliyoruz.
        
        System.out.println("Kac kilogram Armut istersiniz ? : ");   //Kg bilgisini input olarak istiyoruz.
        armut = deger.nextFloat();                                    //Gelen input degerini degiskene esitliyoruz.
        System.out.println("Kac kilogram Elma istersiniz ? : ");   //Kg bilgisini input olarak istiyoruz.
        elma = deger.nextFloat();                                    //Gelen input degerini degiskene esitliyoruz.
        System.out.println("Kac kilogram Domates istersiniz ? : ");   //Kg bilgisini input olarak istiyoruz.
        domat = deger.nextFloat();                                    //Gelen input degerini degiskene esitliyoruz.
        System.out.println("Kac kilogram Muz istersiniz ? : ");   //Kg bilgisini input olarak istiyoruz.
        muz = deger.nextFloat();                                    //Gelen input degerini degiskene esitliyoruz.
        System.out.println("Kac kilogram Patlican istersiniz ? : ");   //Kg bilgisini input olarak istiyoruz.
        pat = deger.nextFloat();                                    //Gelen input degerini degiskene esitliyoruz.
         
        double armutf=armut*(2.14);     //Armutun fiyatini hesapliyoruz.
        double elmaf=elma*(3.67);       //Elma fiyatini hesapliyoruz.
        double domatf=domat*(1.11);     //Domates fiyatini hesapliyoruz.
        double muzf=muz*(0.95);         //Muz fiyatini hesapliyoruz.
        double patf=pat*(5.00);         //Patlican fiyatini hesapliyoruz.
        double toplam=armutf+elmaf+domatf+muzf+patf;    //Toplam alisverisi hesapliyoruz.
        System.out.println("Alisverisiniz sonunda odemeniz gereken toplam tutar: "+toplam+" TL'dir. Yine bekleriz.");  //Toplami yazdiriyoruz.
        }
}
```
