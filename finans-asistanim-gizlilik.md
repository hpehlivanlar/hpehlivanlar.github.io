---
layout: page
title: Finansal Asistanım Gizlilik Politikası
subtitle: Gizlilik, finansal veriler, yapay zekâ, bildirimler ve abonelikler
permalink: /finans-asistanim-gizlilik/
---

**Son güncelleme tarihi: 8 Eylül 2026**

Bu Gizlilik Politikası, **Finansal Asistanım** uygulamasının hangi bilgileri kullandığını, kişisel finans verilerinin nasıl saklandığını, çevrimiçi servislerin hangi amaçlarla kullanıldığını ve kullanıcı gizliliğinin nasıl korunduğunu açıklar.

## 1. Uygulama hakkında

Finansal Asistanım; kullanıcıların banka hesaplarını, kredi kartlarını, KMH/ek hesaplarını, kredilerini, gelir ve giderlerini tek yerde takip etmesine, bilanço ve nakit akışı oluşturmasına, ödeme planlarını değerlendirmesine ve yaklaşan ödemeler için hatırlatmalar almasına yardımcı olan iOS uygulamasıdır.

Uygulama bir banka, ödeme kuruluşu, yatırım kuruluşu veya kamu kurumu değildir. Banka hesabınıza doğrudan bağlanmak, para transferi yapmak veya sizin adınıza finansal işlem gerçekleştirmek amacıyla tasarlanmamıştır.

## 2. Local-first veri saklama yaklaşımı

Finansal Asistanım, kişisel finans verilerini mümkün olduğunca kullanıcının kendi cihazında tutacak şekilde **local-first** mimariyle tasarlanmıştır.

Aşağıdaki bilgiler temel olarak iPhone veya iPad üzerinde tutulabilir:

- Banka ve hesap adları
- Vadesiz hesap bakiyeleri
- KMH/ek hesap limiti ve kullanılan KMH tutarı
- Kredi kartı toplam limiti, kalan limit ve borç bilgileri
- İhtiyaç, konut, taşıt ve diğer kredi bilgileri
- Gelir ve gider kayıtları
- Düzenli ödeme ve ödeme günü bilgileri
- Faiz oranları ve kullanıcı tarafından girilmiş sözleşme bilgileri
- Ödeme planları
- Finansal tercihler
- Aylık bilanço ve geçmiş özetleri

Yerel finans kasası uygulama içinde **AES-GCM** ile şifrelenir. Şifreleme anahtarı iOS Keychain içerisinde cihazla sınırlı erişim politikasıyla saklanır.

## 3. Saklama süresi ve geçmiş bilanço

Uygulama, ayrıntılı işlem hareketlerini performans ve depolama amacıyla sınırlı süreyle saklayabilir.

Varsayılan tasarım:

- Ayrıntılı işlem hareketleri: en az **36 ay**
- Aylık bilanço ve özet kayıtları: **10 yıla kadar**

Bir aya ait bilanço özeti güvenli biçimde oluşturulmadan o döneme ait ayrıntılı hareketlerin otomatik olarak temizlenmemesi hedeflenir. Böylece eski işlem ayrıntıları zamanla azaltılsa bile geçmiş toplam varlık, toplam borç, net varlık, gelir, gider ve banka bazlı özet değerleri korunabilir.

## 4. Kullanıcı hesabı ve sunucu tarafı

Uygulamanın temel kullanımı için geliştiriciye ait bir kullanıcı hesabı oluşturmak zorunlu değildir.

Çevrimiçi servislerin kullanılabilmesi amacıyla anonim cihaz oturumu, kısa ömürlü erişim belirteçleri ve sınırlı teknik güvenlik kayıtları işlenebilir.

Temel finansal kayıtların tamamının geliştirici sunucusunda açık biçimde tutulması amaçlanmaz.

İleride kullanıcı isteğe bağlı şifreli bulut yedekleme özelliğini etkinleştirirse, yedek verinin sunucu tarafında yalnızca şifreli ve geliştirici tarafından doğrudan okunamayacak biçimde saklanması hedeflenir.

## 5. Uygulamaya girilmemesi gereken bilgiler

Finansal Asistanım aşağıdaki bilgileri istemez ve bu bilgilerin uygulamaya girilmemesi gerekir:

- İnternet veya mobil bankacılık parolası
- Kart CVV/CVC güvenlik kodu
- Kart PIN kodu
- SMS/OTP doğrulama kodu
- e-Devlet parolası

Tam kart numarası veya benzeri gereksiz hassas ödeme verilerinin saklanması uygulamanın temel işlevi için gerekli değildir.

## 6. Yapay zekâ özellikleri

Asistanın hesaplanabilir finansal işlevleri — bilanço özeti, borç ödeme sırası, kredi kartı/KMH özeti, gelir-gider analizi, ödeme kapasitesi ve banka bazlı toplamlar gibi işlemler — mümkün olduğunda cihaz üzerinde deterministik olarak hesaplanır.

Kullanıcı gelişmiş yapay zekâ açıklaması istediğinde, mümkün olduğunca asgariye indirilmiş ve doğrudan kimlik bilgileri çıkarılmış finansal özet çevrimiçi yapay zekâ altyapısına iletilebilir.

Yapay zekâ bağlamına ad, e-posta, telefon, T.C. kimlik numarası, IBAN, tam kart numarası gibi doğrudan tanımlayıcıların dahil edilmemesi hedeflenir.

Çevrimiçi yapay zekâ ve barındırma hizmetlerinin Türkiye dışında altyapı kullanması mümkündür. Kullanıcı gelişmiş AI özelliklerini kullanmayarak bu aktarımı sınırlandırabilir.

## 7. Finansal referans verileri ve faiz oranları

Kredi kartı ve KMH için Türkiye Cumhuriyet Merkez Bankası tarafından yayımlanan azami faiz oranları ve diğer kamuya açık finansal referanslar uygulamada bilgi amaçlı gösterilebilir.

Otomatik getirilen oranlar bankanın kullanıcıya özel sözleşme oranı olmayabilir. Kullanıcının kendi banka sözleşmesindeki gerçek oran önceliklidir ve uygulamadaki otomatik oranlar düzenlenebilir.

Finansal Asistanım yatırım danışmanlığı hizmeti vermez ve hisse, fon, kripto veya başka bir sermaye piyasası aracı için kişiye özel al/sat talimatı üretmek amacıyla tasarlanmamıştır.

## 8. Bildirimler

Kullanıcı izin verirse uygulama aşağıdaki amaçlarla yerel bildirim gönderebilir:

- Yaklaşan kredi kartı veya kredi ödemeleri
- KMH ve diğer borç hatırlatmaları
- Haftalık bilanço özeti
- Bütçe ve finansal disiplin hatırlatmaları

Bildirim kategorileri, günleri ve saatleri uygulama içindeki Ayarlar bölümünden değiştirilebilir veya kapatılabilir.

Kullanıcı iOS üzerinden de bildirim iznini istediği zaman değiştirebilir:

```text
iPhone Ayarlar > Bildirimler > Finansal Asistanım
```

## 9. Premium abonelik ve satın almalar

Finansal Asistanım bazı gelişmiş özellikleri Apple App Store üzerinden **otomatik yenilenen Premium abonelik** olarak sunabilir.

Abonelik işlemleri Apple'ın StoreKit ve App Store altyapısı üzerinden gerçekleştirilir. Geliştirici, kullanıcının App Store ödeme kartı bilgilerini kendi sunucusunda işlemez veya saklamaz.

Abonelik kullanıcı tarafından iptal edilmediği sürece seçilen dönem sonunda otomatik olarak yenilenebilir. Abonelik yönetimi ve iptal işlemleri kullanıcının Apple hesabı üzerinden gerçekleştirilir.

Uygun yeni abonelere **7 günlük ücretsiz deneme** gibi App Store Connect üzerinden tanımlanmış bir tanıtım teklifi sunulabilir. Ücretsiz deneme uygunluğu Apple tarafından abonelik grubu bazında belirlenir.

## 10. Kullanıcı kontrolü ve veri silme

Kullanıcı uygulama içinden banka, hesap, kredi kartı, kredi, gelir, gider ve diğer finansal kayıtları ekleyebilir, düzenleyebilir ve silebilir.

Uygulamanın cihazdan kaldırılması durumunda iOS tarafından uygulamaya ait yerel veriler de silinebilir. Apple/iCloud yedekleme davranışı Apple'ın kendi ayar ve koşullarına tabidir.

İsteğe bağlı bir sunucu hesabı veya bulut yedekleme özelliği kullanılması durumunda ilgili hesap ve yedek verileri için ayrıca silme işlemi sağlanabilir.

## 11. Güvenlik

Uygulama; Face ID veya cihaz kilidi, iOS Keychain, AES-GCM yerel şifreleme, HTTPS/TLS bağlantısı, kısa ömürlü oturum belirteçleri ve veri minimizasyonu gibi teknik kontroller kullanır.

Bununla birlikte hiçbir elektronik saklama veya internet üzerinden aktarım yöntemi mutlak güvenlik garantisi vermez.

## 12. Reklam ve kullanıcı takibi

Mevcut sürümün temel işlevleri kullanıcıyı üçüncü taraf uygulama veya web sitelerinde reklam amacıyla takip etmek için tasarlanmamıştır.

Finansal kayıtlar veri aracılarına satılmaz ve hedefli reklam profili oluşturmak amacıyla kullanılmaz.

## 13. Çocukların gizliliği

Finansal Asistanım çocuklara yönelik bir uygulama olarak tasarlanmamıştır.

## 14. Politika değişiklikleri

Uygulamanın özellikleri, kullanılan servisler veya yasal gereklilikler değiştiğinde bu Gizlilik Politikası güncellenebilir. Güncel sürüm her zaman bu sayfada yayımlanacaktır.

## 15. Kullanım Koşulları (EULA)

Özel bir son kullanıcı lisans sözleşmesi belirtilmediği sürece Apple'ın standart Licensed Application End User License Agreement koşulları geçerlidir:

[Apple Standart EULA](https://www.apple.com/legal/internet-services/itunes/dev/stdeula/)

## 16. Destek ve iletişim

**Geliştirici:** Hasan Pehlivanlar  
**E-posta:** [bysiskur@gmail.com](mailto:bysiskur@gmail.com)  
**Destek:** [Ulaş Bana]({{ '/ulasbana/' | relative_url }})  
**Uygulamalar:** [Tüm uygulamalar]({{ '/uygulamalar/' | relative_url }})  
**Ülke:** Türkiye

---

# English Summary — Privacy Policy

**Last updated: September 8, 2026**

**Finansal Asistanım** is a local-first personal finance iOS application. Bank accounts, balances, credit cards, overdrafts, loans, income, expenses, payment plans and historical balance-sheet summaries are primarily stored on the user's device. The local finance vault is encrypted with AES-GCM and its key is stored in iOS Keychain.

Core financial calculations such as balance-sheet summaries, debt prioritization and cash-flow analysis are designed to run locally when possible. If the user chooses an advanced AI explanation, a minimized financial summary without direct identifiers may be sent to external AI infrastructure, which may operate outside Türkiye.

The app does not require internet banking passwords, card CVV/CVC codes, PINs or SMS/OTP verification codes. It does not sell personal financial records to data brokers and is not intended to provide personalized securities investment advice.

Premium features may be offered as auto-renewable subscriptions through Apple's App Store. Eligible users may receive an introductory free trial configured through App Store Connect. Subscription payments, renewals and cancellations are managed by Apple.

For privacy or support questions, contact **bysiskur@gmail.com**.

---

[← Uygulamalar sayfasına dön]({{ '/uygulamalar/' | relative_url }})
