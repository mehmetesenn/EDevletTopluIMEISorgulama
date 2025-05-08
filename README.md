# 📱E-Devlet Toplu IMEI Sorgulama Aracı

Bu Python projesi, bir Excel dosyasındaki IMEI numaralarını kullanarak [turkiye.gov.tr/imei-sorgulama](https://www.turkiye.gov.tr/imei-sorgulama) adresinden otomatik olarak IMEI sorgusu yapar. CAPTCHA doğrulaması için [2Captcha](https://2captcha.com) hizmeti kullanılmaktadır. Sorgulama sonuçları yeni bir Excel dosyasına kaydedilir.

## 📦 Gereksinimler

Aşağıdaki Python kütüphanelerinin sisteminizde yüklü olması gerekir:

```bash
pip install pandas openpyxl selenium twocaptcha tkinter webdriver-manager

### ⚙️ Kurulum ve Kullanım
1. Projeyi İndirin veya Klonlayın
