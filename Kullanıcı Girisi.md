# Proje Sahibi: Patika.Dev 
# Proje Konusu: Başlangıç Seviye Java ile Backend Web Development Patikası
## Konu : Java101

#### Soru> Kullanıcı Girişi:
- Eğer şifre yanlış ise kullanıcıya şifresini sıfırlayıp sıfırlamayacağını sorun, eğer kullanıcı sıfırlamak isterse yeni girdiği şifrenin hatalı girdiği ve unuttuğu şifre ile aynı olmaması gerektiğini kontrol edip , şifreler aynı ise ekrana "Şifre oluşturulamadı, lütfen başka şifre giriniz." sorun yoksa "Şifre oluşturuldu" yazan programı yazınız.


```java
import java.util.Scanner;

public class Main {
    public static void main(String args[]) {
        String us1,pw1,answer,pw2;
        
        String kadi="patika";
        String sifre="java123";
        Scanner input = new Scanner(System.in);
        
        System.out.println("Lutfen kullanıcı adinizi giriniz : ");
        us1=input.nextLine();
        
        System.out.println("Lutfen parolanizi adinizi giriniz : ");
        pw1=input.nextLine();
        
        if(us1.equals(kadi) && pw1.equals(sifre)){
            System.out.println("Hosgeldiniz. Sisteme yonlendiriliyorsunuz.");
        }else{
            System.out.println("Kullanici adiniz veya parolaniz yanlistir.");
            
            System.out.println("Sifrenizi sifirlamak ister misiniz ?\nSifrenizi sifirlamak icin e,devam etmek icin h yaziniz.");
            answer=input.nextLine();
            
            switch(answer){
                case "e":
                    System.out.println("Lutfen yeni sifrenizi giriniz.\n1-)Yeni sifreniz eski sifreniz ile ayni olamaz.\n2-)Az once girdiginiz hatali sifre kabul edilmez.\nLutfen daha onec kullanmadiginiz bir sifre olusturunuz.");
                    pw2=input.nextLine();
                    
                    if(pw2.equals(sifre) || pw2.equals(pw1)){
                        System.out.println("Malesef hatali islem yaptiniz.\nEski sifrenizi veya az once girdiginiz hatali sifreyi girmis olabilirsiniz.Yeniden baglanmayi deneyebilirsiniz.");
                        break;
                    }
                    else{
                        System.out.println("sifreniz basarili sekilde olusturulmustur.");
                        sifre=pw2
                        break;
                    }
                case "h":
                    System.out.println("Programa eski sifrenizle yeniden baglanmayi deneyebilirsiniz.");
                    break;
                default:
                    System.out.println("Programa eski sifrenizle yeniden baglanmayi deneyebilirsiniz.");
            }
        }        
    }
}
```
