# Proje Sahibi: Patika.Dev 
# Proje Konusu: Başlangıç Seviye Java ile Backend Web Development Patikası
## Konu : Java101

#### Yıldızlar ile Üçgen Yapımı:
- Java'da döngüler kullanarak yıldızlar ile elmas yapınız.
- 
```java
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner deger = new Scanner(System.in);
        System.out.println("Bir Sayı Giriniz :");
        int n = deger.nextInt();

        for (int i = 0; i <= n ; i++) {
            for (int j = 0; j < (n - i); j++) {
                System.out.print(" ");
            }
            for (int k = 1; k <= (2 * i + 1); k++) {
                System.out.print("*");
            }
            System.out.println(" ");
        }
        for (int i = 0; i <= n ; i++) {
            for (int j = 0; j < (n - (n-i)); j++) {
                System.out.print(" ");
            }
            for (int k = 1; k <= (2 * (n-i) + 1); k++) {
                System.out.print("*");
            }
            System.out.println(" ");
        }
    }
}
```

