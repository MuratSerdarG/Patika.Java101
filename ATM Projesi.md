# Proje Sahibi: Patika.Dev 
# Proje Konusu: Başlangıç Seviye Java ile Backend Web Development Patikası
## Konu : Java101

#### ATM Projesi:
- Java döngüler ile kullanıcının banka hesabını yönetebildiği bir ATM projesi yapıyoruz.
- Projedeki ATM işlemlerini "Switch-Case" kullanarak yapınız.

```java
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        String userName, password;
        Scanner input = new Scanner(System.in);
        int right = 3;
        int balance = 3500;
        int secim;
        int moneyadd;
        int moneydiscard;
        
        
        while (right > 0) {
            System.out.print("Kullanıcı Adınız :");
            userName = input.nextLine();
            System.out.print("Parolanız : ");
            password = input.nextLine();

            if (userName.equals("patika") && password.equals("dev123")) {
                System.out.println("Merhaba, MSG Bank'a Hoşgeldiniz!");
                do {
                    System.out.println("1-Para yatırma\n" +
                            "2-Para Çekme\n" +
                            "3-Bakiye Sorgula\n" +
                            "4-Çıkış Yap");
                    System.out.print("Lütfen yapmak istediğiniz işlemi seçiniz : ");
                    secim = input.nextInt();
                    switch(secim){
                        case 1:
                            System.out.println("Lütfen yatırmak istediğiniz tutarı giriniz: ");
                            moneyadd = input.nextInt();
                            balance += moneyadd;
                            break;
                        case 2:
                            System.out.print("Lütfen çekmek istediğiniz tutarı giriniz: ");
                            moneydiscard = input.nextInt();
                            if (moneydiscard > balance) {
                                System.out.println("Bakiye yetersiz.");
                            } else {
                                balance -= moneydiscard;
                            }
                            break;
                        case 3:
                            System.out.println("Bakiyeniz : " + balance);
                        }
                    
                }while (secim != 4);
                System.out.println("Tekrar görüşmek üzere.");
                break;
                    
            }else {
                right--;
                System.out.println("Hatalı kullanıcı adı veya şifre. Tekrar deneyiniz.");
                if (right == 0) {
                    System.out.println("Hesabınız bloke olmuştur lütfen banka ile iletişime geçiniz.");
                } else {
                    System.out.println("Kalan Hakkınız : " + right);
                }
            }
        }
    }
}
```

