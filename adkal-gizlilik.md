---
layout: page
title: AdKal Gizlilik Politikası
subtitle: DNS filtreleme, abonelik doğrulama ve veri güvenliği
permalink: /adkal-gizlilik/
---

**Son güncelleme tarihi: 17 Ağustos 2026**

Bu Gizlilik Politikası, **AdKal** iOS uygulamasının ve AdKal DNS hizmetinin bilgileri nasıl işlediğini, hangi hizmetlerden yararlandığını ve kullanıcı gizliliğini nasıl koruduğunu açıklar.

## 1. AdKal hakkında

AdKal; bilinen reklam, izleyici ve zararlı alan adlarına yapılan bağlantıları DNS düzeyinde filtrelemek amacıyla şifreli DNS-over-HTTPS (DoH) kullanan bir iOS uygulamasıdır.

DNS tabanlı filtreleme, bir uygulamanın reklam için kullandığı alan adına erişimi engelleyebilir. Reklamın uygulamayla aynı alan adından sunulduğu durumlarda veya önceden yüklenmiş içeriklerde tüm reklamların engellenmesi garanti edilmez.

## 2. Hesap ve iletişim bilgileri

AdKal kullanmak için geliştirici nezdinde üyelik oluşturulması gerekmez. Uygulama doğrudan:

- Ad ve soyad
- E-posta adresi
- Telefon numarası
- Açık adres
- Konum
- Reklam kimliği
- Apple hesabı parolası
- Kredi veya banka kartı bilgisi

talep etmez.

Satın alma ve abonelik ödemeleri Apple App Store tarafından yönetilir. Geliştirici ödeme kartı bilgilerinin tamamına erişemez.

## 3. DNS sorgularının işlenmesi

AdKal DNS koruması etkinleştirildiğinde cihazın alan adı çözümleme istekleri HTTPS ile şifrelenerek AdKal DNS hizmetine iletilir.

DNS sorguları:

- Reklam ve izleyici alan adı listeleriyle anlık olarak karşılaştırılır.
- Engellenen alan adları için bağlantının kurulmasını önleyen bir DNS yanıtı üretilir.
- Engellenmeyen sorgular şifreli üst DNS çözümleyicilerine aktarılabilir.
- Reklam hedefleme, kullanıcı profili oluşturma veya veri satışı amacıyla kullanılmaz.

AdKal DNS hizmeti **DNS sorgu günlüğü tutmayacak şekilde yapılandırılmıştır**. DNS yazılımındaki kalıcı sorgu günlüğü özelliği kapalıdır.

## 4. Üst DNS sağlayıcıları

Engellenmeyen DNS sorgularının çözümlenmesi için, hizmet sürekliliğine bağlı olarak aşağıdaki şifreli üst DNS sağlayıcılarından yararlanılabilir:

- [Cloudflare 1.1.1.1](https://www.cloudflare.com/privacypolicy/)
- [Quad9](https://www.quad9.net/privacy/policy/)

Bu sağlayıcıların veri işleme faaliyetleri kendi gizlilik politikalarına tabidir.

## 5. Premium abonelik ve Apple StoreKit

AdKal Premium aylık ve yıllık abonelikleri Apple App Store ve StoreKit üzerinden sunulur. Yıllık paket için uygun kullanıcılara App Store tarafından 14 günlük ücretsiz deneme sunulabilir.

Premium erişimini doğrulamak için Apple tarafından imzalanan abonelik işlem verisi kontrol edilir. Sunucuda hizmetin çalışması ve kötüye kullanımın önlenmesi için aşağıdaki sınırlı teknik bilgiler işlenebilir:

- Tek yönlü özetlenmiş kurulum kimliği
- Tek yönlü özetlenmiş işlem ve ilk işlem kimlikleri
- Satın alınan ürün kimliği
- Aboneliğin geçerlilik süresi ve ortam bilgisi
- Cihaz erişiminin etkin veya iptal edilmiş olma durumu
- Tek yönlü özetlenmiş DNS erişim tokenı

AdKal, kullanıcının Apple hesabı e-posta adresini veya Apple hesabı parolasını almaz.

## 6. App Attest ve cihaz doğrulaması

Yetkisiz istemcilerin DNS hizmetini kullanmasını sınırlandırmak için Apple App Attest kullanılabilir.

Bu kapsamda aşağıdaki teknik veriler işlenebilir:

- Özetlenmiş App Attest anahtar kimliği
- Doğrulama için kullanılan cihaz anahtarının açık anahtarı
- Apple tarafından sağlanan App Attest doğrulama makbuzu
- Tekrar kullanımını önleyen doğrulama sayacı
- Kısa süreli, tek kullanımlık doğrulama isteği (challenge)

Bu bilgiler uygulamanın bütünlüğünü doğrulamak, cihaz sınırını uygulamak ve yetkisiz DNS kullanımını engellemek amacıyla kullanılır.

## 7. Cihaz erişim tokenı

Başarılı abonelik ve App Attest doğrulamasından sonra cihaza rastgele bir DNS erişim tokenı verilir.

- Ham token cihazın iOS Anahtar Zinciri'nde (Keychain) saklanır.
- Sunucuda ham token yerine tek yönlü özeti saklanır.
- Token, DNS isteği sırasında Premium erişimin geçerli olup olmadığını denetlemek için kullanılır.
- Kullanıcı Ayarlar ekranından bu cihazın erişimini iptal edebilir.

Tek abonelikle desteklenen cihaz sayısı uygulamadaki güncel paket koşullarına göre sınırlandırılabilir.

## 8. Teknik güvenlik kayıtları

Sunucu ve ters proxy altyapısı; hizmet güvenliği, hata analizi, hız sınırlama ve kötüye kullanımın önlenmesi için IP adresi, istek zamanı, istek yolu, HTTP durum kodu ve benzeri sınırlı teknik erişim kayıtları oluşturabilir.

Token içeren DNS yolu için erişim kaydı kapalı olacak şekilde yapılandırma uygulanır. Güvenlik kayıtları DNS sorgu geçmişi veya reklam profili oluşturmak amacıyla kullanılmaz, satılmaz ve yalnız gerekli olduğu süre boyunca tutulur.

## 9. Verilerin kullanım amaçları

İşlenen sınırlı teknik bilgiler yalnızca şu amaçlarla kullanılır:

- DNS tabanlı reklam ve izleyici filtreleme hizmetini sunmak
- Premium abonelik hakkını doğrulamak
- Yetkisiz istemcileri ve hizmet kötüye kullanımını sınırlandırmak
- Cihaz erişimini etkinleştirmek, yenilemek veya iptal etmek
- Hizmetin güvenliğini, kararlılığını ve sürekliliğini sağlamak
- Teknik hataları incelemek

AdKal kullanıcı bilgilerini reklam amacıyla satmaz veya üçüncü taraf reklam profili oluşturmaz.

## 10. Saklama ve silme

Cihazdaki uygulama ayarları, kurulum kimliği ve erişim bilgileri uygulamanın işlevlerini sağlamak amacıyla cihazda saklanabilir. Uygulamanın kaldırılması cihazdaki uygulama verilerini kaldırabilir; iOS Anahtar Zinciri'ndeki bazı güvenlik verilerinin yönetimi iOS davranışına bağlıdır.

Kullanıcı, AdKal Ayarlar ekranındaki **Bu cihazın erişimini kaldır** seçeneğiyle cihaz tokenını geçersiz kılabilir. Abonelik Apple tarafından yönetildiği için abonelik iptali App Store abonelik ayarlarından yapılır.

Sunucudaki kendinizle ilişkili teknik kayıtların silinmesini talep etmek için aşağıdaki iletişim adresini kullanabilirsiniz. Talebin kötüye kullanılmasını önlemek amacıyla makul doğrulama istenebilir.

## 11. Çocukların gizliliği

AdKal genel amaçlı bir ağ gizliliği ve reklam alan adı filtreleme hizmetidir. Çocuklardan bilerek kişisel bilgi toplamayı hedeflemez.

## 12. Güvenlik

Uygulama ile AdKal hizmeti arasındaki iletişim HTTPS üzerinden şifrelenir. Sunucu erişimi token doğrulaması, App Attest, hız sınırlama ve erişim kontrolleriyle korunur. Bununla birlikte hiçbir internet hizmeti mutlak güvenlik garantisi veremez.

## 13. Politika değişiklikleri

Uygulamanın veri işleme biçimi, kullanılan altyapı veya yasal yükümlülükler değişirse bu Gizlilik Politikası güncellenebilir. Güncel metin bu sayfada yayımlanır ve son güncelleme tarihi sayfanın üstünde gösterilir.

## 14. Kullanım Koşulları

AdKal abonelikleri ve uygulamanın kullanım şartları için Apple’ın standart Kullanım Koşulları geçerlidir:

[Apple Standart Kullanım Koşulları (EULA)](https://www.apple.com/legal/internet-services/itunes/dev/stdeula/)

## 15. İletişim

**Geliştirici:** Hasan Pehlivanlar  
**E-posta:** [bysiskur@gmail.com](mailto:bysiskur@gmail.com)  
**Ülke:** Türkiye

---

[← Uygulamalar sayfasına dön]({{ '/uygulamalar/' | relative_url }})
