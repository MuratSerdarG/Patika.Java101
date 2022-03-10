# Proje Sahibi: Patika.Dev 
# Proje Konusu: Başlangıç Seviye Java ile Backend Web Development Patikası
## Konu : Java101

#### Soru> Hesap Makinesi:
- Videodaki hesap makinesini switch-case kullanarak yapınız.


```java
import java.util.Scanner;

public class Main {
    public static void main(String args[]) {
        double sayi1,sayi2;
        int islem;
        
        Scanner input = new Scanner(System.in);
        System.out.println("Ilk sayiyi giriniz : ");
        sayi1=input.nextInt();
        System.out.println("Ikinci sayiyi giriniz : ");
        sayi2=input.nextInt();
        
        System.out.println("Yapmak istediginiz islemin numarasini girmeniz gerekmektedir.");
        System.out.println("1-Toplama\n2-Cikarma\n3-Carpma\n4-Bolme");
        System.out.println("Lutfen yapmak istediginiz islemi seciniz :");
        islem=input.nextInt();
        
        switch(islem){
            case 1:
                System.out.println("Islem Sonucunuz : "sayi1+" + "+sayi2+" = "+(sayi1+sayi2));
                break;
            case 2:
                System.out.println("Islem Sonucunuz : "sayi1+" - "+sayi2+" = "+(sayi1-sayi2));
                break;
            case 3:
                System.out.println("Islem Sonucunuz : "sayi1+" * "+sayi2+" = "+(sayi1*sayi2));
                break;
            case 4:
                if(sayi2!=0){
                    System.out.println("Islem Sonucunuz : "sayi1+" / "+sayi2+" = "+(sayi1/sayi2));
                break;
                }else if(sayi2==0){
                    System.out.println("Herhangi bir sayi sifira bolunemez. Yeniden deneyiniz.");
                    break;
                }
                
            default:
                System.out.println("Hatali islem yaptiniz. Lutfen yeniden deneyiniz.");
                break;
        }
        
    }
}
```
