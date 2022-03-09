# Proje Sahibi: Patika.Dev 
# Proje Konusu: Başlangıç Seviye Java ile Backend Web Development Patikası
## Konu : Java101

#### Soru> Dairenin Alanını ve Çevresini Hesaplayan Program:
- Java ile yarı çapını kullanıcıdan aldığınız dairenin alanını ve çevresini hesaplayan programı yazın.
- Formül olarak; Alan Formülü : π * r * r; Çevre Formülü : 2 * π * r.
- Yarıçapı r, merkez açısının ölçüsü 𝛼 olan daire diliminin alanı bulan programı yazınız. (𝜋 sayısını = 3.14 alınız.)
- Merkez açı alan formülü : (𝜋 * (r*r) * 𝛼) / 360.

```java
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner deger = new Scanner(System.in);
        
        float ycap,maci;   //Degiskeni float olarak ayarliyoruz.
        
        System.out.println("Lutfen yari capin degerini giriniz : ");          //Dairenin yari cap bilgisini input olarak istiyoruz.
        ycap = deger.nextFloat();                                                                   //Gelen input degerini degiskene esitliyoruz.
        System.out.println("Lutfen merkez aci derecesini giriniz : ");          //Merkez aci bilgisini input olarak istiyoruz.
        maci = deger.nextFloat();                                                                   //Gelen input degerini degiskene esitliyoruz.

        double pie=3.14;
        double alan=pie*ycap*ycap;
        double cevre=2*pie*ycap;
        double macideger=(alan*maci)/(360);
        
        System.out.println("Dairemizin alan ölcüsü : "+alan);         //Alani yazdiriyoruz.
        System.out.println("Dairemizin cevre ölcüsü : "+cevre);       //Cevreyi yazdiriyoruz.
        System.out.println("Merkez acisi "+maci+" olan daire diliminin alani "+macideger+" seklindedir.");       //Daire dilimini yazdiriyoruz.
        
    }
}
```
