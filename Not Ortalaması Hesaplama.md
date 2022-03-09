# Proje Sahibi: Patika.Dev 
# Proje Konusu: Başlangıç Seviye Java ile Backend Web Development Patikası
## Konu : Java101

#### 1. Soru Not Ortalaması Hesaplayan Program:
- Java ile Matematik, Fizik, Kimya, Türkçe, Tarih, Müzik derslerinin sınav puanlarını kullanıcıdan alan ve ortalamalarını hesaplayıp ekrana bastırılan programı yazın.
- Aynı program içerisinde koşullu ifadeler kullanılarak, eğer kullanıcının ortalaması 60'dan büyük ise ekrana "Sınıfı Geçti" , küçük ise "Sınıfta Kaldı" yazsın.
- Not : If ve Else kullanılmayacak...

```java
import java.util.Scanner;

public class JavaPatika {
    public static void main(String[] args) {
        Scanner deger = new Scanner(System.in);
        
        int mt,fz,km,tr1,tr2,mz;  //Derslere basvuracak degiskenleri burada olusturuyoruz.
        
        System.out.println("Lutfen Matematik dersi sinav puani giriniz : ");    //Matematik dersi icin input degerini istiyoruz
        mt = deger.nextInt();                                                       //Gelen input degerini degiskene esitliyoruz.

        System.out.println("Lutfen Fizik dersi sinav puani giriniz : ");    //Fizik dersi icin input degerini istiyoruz
        fz = deger.nextInt();                                                   //Gelen input degerini degiskene esitliyoruz.

        System.out.println("Lutfen Kimya dersi sinav puani giriniz ");      //Kimya dersi icin input degerini istiyoruz
        km = deger.nextInt();                                                   //Gelen input degerini degiskene esitliyoruz.
        
        System.out.println("Lutfen Turkce dersi sinav puani giriniz ");     //Turkce dersi icin input degerini istiyoruz
        tr1 = deger.nextInt();                                                  //Gelen input degerini degiskene esitliyoruz.

        System.out.println("Lutfen Tarih dersi sinav puani giriniz ");      //Tarih dersi icin input degerini istiyoruz
        tr2 = deger.nextInt();                                                  //Gelen input degerini degiskene esitliyoruz.
        
        System.out.println("Lutfen Muzik dersi sinav puani giriniz ");      //Muzik dersi icin input degerini istiyoruz
        mz = deger.nextInt();                                                   //Gelen input degerini degiskene esitliyoruz.
        
        double total=(mt+fz+km+tr1+tr2+mz)/6;                               //Derslerin ortalamasini buluyoruz.
        
        String durum = ( total>= 60 ) ? "Tebrikler Gectiniz." : "Ne yazik ki Kaldiniz.";    //Sonucu belirliyoruz.
        

        System.out.println("Not Ortalamaniz : " + total);   //Ortalamayi yazdiriyoruz.
        System.out.println(durum);                          //Sonucu yazdiriyoruz.
    }
}
```

