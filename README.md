# 📱E-Devlet Toplu IMEI Sorgulama Aracı

Bu Python projesi, bir Excel dosyasındaki IMEI numaralarını kullanarak [turkiye.gov.tr/imei-sorgulama](https://www.turkiye.gov.tr/imei-sorgulama) adresinden otomatik olarak IMEI sorgusu yapar. CAPTCHA doğrulaması için [2Captcha](https://2captcha.com) hizmeti kullanılmaktadır. Sorgulama sonuçları yeni bir Excel dosyasına kaydedilir.

## 📦 Gereksinimler

Aşağıdaki Python kütüphanelerinin sisteminizde yüklü olması gerekir:

```bash
pip install pandas openpyxl selenium twocaptcha tkinter webdriver-manager
```

## ⚙️ Kurulum ve Kullanım
1. Projeyi İndirin veya Klonlayın
   ```bash
   git clone https://github.com/kullaniciadi/toplu-imei-sorgulama.git
    ```
2. 2Captcha API Key Oluşturun
   * [https://2captcha.com/?from=register] adresine giderek bir hesap oluşturun.
   * Giriş yaptıktan sonra kontrol panelinizden API Key’inizi kopyalayın.
     Örnek: 123456abcdef123456abcdef123456ab
3. API Key’i Tanımlayın
    * Koda Manuel Olarak Yazmak captcha.py dosyasındaki şu satırı bulun:
    * ```bash
       API_KEY = os.getenv('APIKEY_2CAPTCHA', 'YOUR-API-KEY')
       ```
4. Programı Başlatın
   * python captcha.py


## 🧑‍💻 Kullanım Adımları
   1. Program açıldığında gelen arayüzde bir Excel dosyası seçin.
    
   2. Dosyanın içinde IMEI adında bir sütun olduğundan emin olun.

   3. “Sorgulamayı Başlat” butonuna tıklayın.

   4. CAPTCHA’lar otomatik olarak çözülecek.

   5. Sorgulama işlemi tamamlandıktan sonra sonuçları kaydedeceğiniz bir konum seçin.

## 📂 Giriş Excel Dosyası Formatı
Excel dosyası şu şekilde olmalıdır:
| IMEI            |
| --------------- |
| 866867079170093 |
| 490154203237518 |
| ...             |

## 📝 Özellikler
 * Otomatik CAPTCHA çözümü (2Captcha API ile)

 * Excel dosyasından toplu IMEI okuma

 * Selenium ile web üzerinden otomasyon

 * Başarısız sorgular için hata mesajları kayıt altına alınır

 * Tkinter arayüzü ile kullanıcı dostu GUI

 * Headless (görünmeden) çalışabilen tarayıcı
   
## ⚠️ Uyarılar
 * Bu araç e-Devlet portalına otomatik sorgular gönderir. Lütfen aşırı sorgu yapmaktan kaçının.

 * CAPTCHA çözümü ücretlidir, 2Captcha bakiyesi gerektirir.

 * Web sayfasında yapılacak değişiklikler kodun çalışmasını engelleyebilir.

 * Bu proje yalnızca eğitim ve otomasyon denemeleri içindir. Ticari amaçla kullanmayınız.

## Uygulama
![IMEI Sorgulama Demo](https://github.com/mehmetesenn/EDevletTopluIMEISorgulama/raw/main/imeiSorgu.gif)








