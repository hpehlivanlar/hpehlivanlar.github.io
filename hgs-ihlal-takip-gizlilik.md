---
layout: page
title: HGS İhlal Takip Gizlilik Politikası
subtitle: Gizlilik, plaka sorguları ve bildirimler
permalink: /hgs-ihlal-takip-gizlilik/
---

**Son güncelleme tarihi: 5 Eylül 2026**

Bu Gizlilik Politikası, **HGS İhlal Takip** uygulamasının hangi bilgileri kullandığını, sorguların nasıl gerçekleştirildiğini ve kullanıcı gizliliğinin nasıl korunduğunu açıklar.

## 1. Uygulama hakkında

HGS İhlal Takip; kullanıcıların Türkiye'deki otoyol ve köprü geçişlerine ilişkin ihlal/borç kayıtlarını plaka bazında takip etmesine, yeni kayıtlar için bildirim almasına ve ödeme işlemlerini unutmaması için hatırlatmalar oluşturmasına yardımcı olan bağımsız bir iOS uygulamasıdır.

Uygulama, kayıtlı plakalar için yaklaşık **8 saatlik kontrol aralıklarıyla** yeni ihlal olup olmadığını kontrol edecek şekilde tasarlanmıştır. Bildirimlerin zamanında ulaşması; internet bağlantısı, iOS bildirim izinleri, Apple Push Notification service (APNs), sunucu erişilebilirliği ve üçüncü taraf hizmetlerin durumuna bağlı olabilir.

**HGS İhlal Takip; Karayolları Genel Müdürlüğü (KGM), PTT, HGS veya başka bir kamu kurumu tarafından geliştirilmiş, işletilen, desteklenen ya da onaylanan resmi bir uygulama değildir.**

## 2. Resmî veri kaynağı

İhlal sorgularında kullanılan bilgiler, Karayolları Genel Müdürlüğü tarafından internet üzerinden sunulan kamuya açık ihlal sorgulama hizmetinden alınır.

Resmî sorgulama kaynağı:

[Karayolları Genel Müdürlüğü — Web İhlal Takip](https://webihlaltakip.kgm.gov.tr/WebIhlalSorgulama/Sayfalar/Sorgulama.aspx)

KGM'nin kendi sistemi, veri yapısı, erişim yöntemi, CAPTCHA mekanizması veya hizmet koşulları zaman içinde değişebilir. Bu değişiklikler uygulamanın sorgu özelliğini geçici veya kalıcı olarak etkileyebilir.

## 3. Kullanıcı hesabı

HGS İhlal Takip'in mevcut sürümünde kullanıcıların geliştiriciye ait bir hesap oluşturması zorunlu değildir.

Uygulama kullanıcıdan doğrudan aşağıdaki bilgileri talep etmez:

- Ad ve soyadı
- Açık adres
- Rehber bilgileri
- Fotoğraf veya video
- Sağlık bilgileri
- Kredi kartı veya banka kartı bilgileri
- İnternet bankacılığı parolası
- e-Devlet parolası

## 4. Plaka ve araç bilgileri

Kullanıcı, takip etmek istediği bir veya daha fazla aracın plakasını uygulamaya kaydedebilir.

Plaka ve araçla ilgili tercihler uygulamanın yerel veri alanında saklanabilir. Kullanıcı bir sorgu başlattığında veya periyodik ihlal kontrolü etkin olduğunda ilgili plaka, sorgunun gerçekleştirilebilmesi için geliştirici tarafından işletilen backend hizmetine iletilebilir.

Backend hizmeti:

`https://hgs-api.adresliyorum.com`

Bu aktarımın amacı yalnızca kullanıcının talep ettiği ihlal sorgusunu gerçekleştirmek, sonuçları uygulamaya iletmek ve etkinleştirilmişse yeni ihlal bildirimlerini oluşturabilmektir.

Plaka bilgileri reklam profili oluşturmak, kullanıcıları pazarlama amacıyla takip etmek veya veri aracılarına satmak amacıyla kullanılmaz.

## 5. Sorgu ve ihlal bilgileri

Sorgu sonucunda aşağıdaki türde bilgiler görüntülenebilir veya uygulama içinde saklanabilir:

- Plaka
- Geçiş/ihlal tarihi ve saati
- Giriş ve çıkış noktaları
- Otoyol, köprü veya işletmeci bilgisi
- Geçiş ücreti
- Borç veya ödenecek tutar
- Ödeme durumu
- Sorgu tarihi
- Bildirim ve ödeme hatırlatma durumu

Bu bilgiler, kullanıcının ihlal geçmişini takip edebilmesi, yeni kayıtları önceki sorgularla karşılaştırabilmesi ve ödeme hatırlatmaları oluşturabilmesi amacıyla kullanılabilir.

## 6. Periyodik kontrol ve bildirimler

Kullanıcı bildirimleri etkinleştirdiğinde uygulama, kayıtlı plakalar için yeni ihlal olup olmadığını periyodik olarak kontrol edebilir. Mevcut tasarımda kontrol aralığı yaklaşık **8 saattir**.

Yeni bir ihlal tespit edildiğinde kullanıcıya bildirim gönderilebilir. Ayrıca mevcut bir ihlalin ödemesini unutmamak için yerel veya uzaktan ödeme hatırlatmaları oluşturulabilir.

Bildirim özelliğinin çalışması için Apple tarafından sağlanan APNs cihaz belirteci gibi teknik bir bildirim kimliği kullanılabilir. Bu teknik kimlik yalnızca bildirimin doğru cihaza ulaştırılması amacıyla kullanılır.

Kullanıcı bildirim iznini istediği zaman aşağıdaki bölümden değiştirebilir:

```text
iPhone Ayarlar > Bildirimler > HGS İhlal Takip
```

## 7. Sunucu ve teknik kayıtlar

Uygulamanın sorgu hizmeti geliştirici tarafından işletilen bir backend üzerinden çalışır. Sunucu güvenliği, hata ayıklama ve hizmet sürekliliği amacıyla aşağıdaki teknik bilgiler sınırlı süreyle sunucu kayıtlarında işlenebilir:

- IP adresi
- İstek tarihi ve saati
- Kullanılan API uç noktası
- HTTP durum kodu
- Teknik hata ve performans bilgileri

Bu teknik kayıtlar reklam veya kullanıcı profillemesi amacıyla kullanılmaz.

## 8. CAPTCHA ve KGM oturumu

KGM'nin sorgulama hizmeti, otomatik erişimi veya sorgu güvenliğini sağlamak amacıyla CAPTCHA ve oturum mekanizmaları kullanabilir.

Sorgunun gerçekleştirilebilmesi için KGM tarafındaki oturum, form alanları, CAPTCHA veya benzeri teknik işlemler backend hizmeti üzerinden yönetilebilir. Bu işlemler yalnızca ihlal sorgusunu tamamlamak amacıyla kullanılır.

## 9. Ödeme işlemleri

**HGS İhlal Takip uygulaması ödeme almaz ve ödeme işlemini kendi sistemi içinde gerçekleştirmez.**

Uygulama:

- Kredi kartı veya banka kartı bilgisi istemez.
- Kart numarası veya ödeme bilgisi saklamaz.
- Kullanıcı adına ödeme tahsil etmez.
- Banka hesabına veya HGS hesabına erişmez.

Kullanıcı ödeme yapmak istediğinde KGM, Gelir İdaresi Başkanlığı, ilgili otoyol/köprü işletmecisi veya diğer yetkili resmî ödeme sayfalarına yönlendirilebilir. Ödeme işlemi ilgili resmî hizmet sağlayıcının kendi sistemi, kullanım koşulları ve gizlilik politikası kapsamında gerçekleştirilir.

## 10. Üçüncü taraf hizmetleri

Uygulama işlevlerinin sağlanması sırasında aşağıdaki üçüncü taraf veya dış hizmetlerle teknik iletişim kurulabilir:

- Karayolları Genel Müdürlüğü'nün kamuya açık ihlal sorgulama sistemi
- Apple Push Notification service (APNs)
- Apple'ın işletim sistemi, App Store ve hata raporlama altyapıları
- Kullanıcının ödeme yapmak için kendi isteğiyle açtığı resmî ödeme sayfaları

Bu hizmetler kendi gizlilik politikaları ve kullanım koşulları kapsamında veri işleyebilir.

## 11. Reklam ve kullanıcı takibi

HGS İhlal Takip'in mevcut sürümünde üçüncü taraf reklam hizmetleri kullanılmamaktadır.

Uygulama:

- Kullanıcıyı başka uygulama veya web sitelerinde reklam amacıyla takip etmez.
- Reklam profili oluşturmaz.
- Plaka veya ihlal verilerini veri aracılarına satmaz.
- Hedefli reklam amacıyla ihlal veya araç bilgisi işlemez.

Gelecekte veri işleme davranışını değiştiren yeni bir özellik, reklam veya analiz hizmeti eklenmesi durumunda bu Gizlilik Politikası ve App Store gizlilik bildirimleri güncellenecektir.

## 12. Veri güvenliği

Uygulama ile backend hizmeti arasındaki veri aktarımında HTTPS kullanılır. Sunucu ve uygulama tarafında yetkisiz erişimi azaltmak için makul teknik önlemler uygulanır.

Bununla birlikte internet üzerinden yapılan hiçbir aktarımın veya elektronik saklama yönteminin mutlak güvenli olduğu garanti edilemez.

## 13. Verilerin silinmesi

Kullanıcı, uygulamada kayıtlı araç/plaka ve sorgu geçmişini mevcut uygulama özellikleri ölçüsünde silebilir.

Uygulamanın cihazdan kaldırılması durumunda iOS tarafından uygulamaya ait yerel veriler de silinebilir. Apple/iCloud yedekleme davranışı Apple'ın kendi ayar ve koşullarına tabidir.

Gizlilik veya veri silme talepleri için geliştiriciyle iletişime geçilebilir.

## 14. Çocukların gizliliği

HGS İhlal Takip çocuklara yönelik bir uygulama olarak tasarlanmamıştır ve çocuklardan bilerek kişisel bilgi toplamaz.

## 15. Sorumluluk ve bilgi doğruluğu

Uygulamada gösterilen ihlal, ücret, borç, ödeme durumu veya tarih bilgileri üçüncü taraf resmî kaynaklardan alınır. Nihai ve bağlayıcı kayıt, ilgili resmî kurum veya işletmecinin sistemindeki kayıttır.

Kullanıcı, ödeme veya itiraz gibi hukuki ya da mali sonuç doğurabilecek işlemler öncesinde bilgileri ilgili resmî kaynaktan doğrulamalıdır.

## 16. Gizlilik politikasındaki değişiklikler

Uygulamanın özellikleri, kullanılan backend altyapısı, veri kaynakları veya yasal gereklilikler değiştiğinde bu Gizlilik Politikası güncellenebilir. Güncel politika her zaman bu sayfada yayımlanacaktır.

## 17. Kullanım Koşulları (EULA)

Özel bir son kullanıcı lisans sözleşmesi belirtilmediği sürece Apple'ın standart Kullanım Koşulları geçerlidir:

[Apple Standart Kullanım Koşulları (EULA)](https://www.apple.com/legal/internet-services/itunes/dev/stdeula/)

## 18. Destek ve iletişim

**Geliştirici:** Hasan Pehlivanlar  
**E-posta:** [bysiskur@gmail.com](mailto:bysiskur@gmail.com)  
**Destek:** [Ulaş Bana]({{ '/ulasbana/' | relative_url }})  
**Ülke:** Türkiye

---

# English Summary — Privacy Policy

**Last updated: September 5, 2026**

**HGS İhlal Takip** is an independent iOS application that helps users monitor toll-road and bridge violation/debt records in Türkiye by license plate, receive notifications about newly detected records, and set payment reminders.

The app is **not an official application of the General Directorate of Highways (KGM), PTT, HGS, or any other governmental authority, and is not endorsed by them.** Violation information is obtained from KGM's publicly available web violation query service.

License plates may be stored locally on the device and are transmitted to the developer-operated backend at `https://hgs-api.adresliyorum.com` when a query or enabled periodic check is performed. The current design may check registered plates approximately every eight hours. Technical server logs such as IP address, request time, HTTP status and error information may be processed for security and service reliability.

The app does not process payments, does not request or store credit/debit card information, and does not access the user's HGS or bank account. When the user chooses to pay, the app may redirect to an official payment website operated by the relevant authority or toll operator.

The current version does not use third-party advertising and does not sell license plate or violation information to data brokers.

For privacy or support questions, contact **bysiskur@gmail.com**.

---

[← Uygulamalar sayfasına dön]({{ '/uygulamalar/' | relative_url }})
