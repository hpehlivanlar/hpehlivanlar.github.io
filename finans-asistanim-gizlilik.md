---
layout: page
title: "Finansal Asistanım — Gizlilik, Veri Kullanımı ve Destek"
permalink: /finans-asistanim-gizlilik/
---

# Finansal Asistanım — Gizlilik Politikası

**Son güncelleme:** 8 Eylül 2026

Finansal Asistanım, kişisel finans verilerini mümkün olduğunca kullanıcının kendi cihazında tutacak şekilde tasarlanmış **local-first** bir iOS uygulamasıdır.

## 1. Cihazda tutulan veriler

Banka ve hesap adları, vadesiz hesap bakiyeleri, kredi kartı limit ve borçları, KMH/ek hesap bilgileri, kredi bilgileri, gelirler, giderler, ödeme planları, kişisel finans tercihleri ve geçmiş bilanço özetleri temel olarak kullanıcının iPhone veya iPad cihazında saklanır.

Yerel finans kasası AES-GCM ile şifrelenir. Şifreleme anahtarı iOS Keychain içerisinde cihazla sınırlı erişim politikasıyla tutulur.

## 2. Geçmiş ve saklama politikası

Uygulama ayrıntılı işlem hareketlerini performans ve depolama amacıyla sınırlı bir süre tutabilir. Aylık bilanço snapshot'ları; toplam varlık, toplam borç, net varlık, gelir, gider ve banka bazlı özetler gibi tarihsel değerlerin kaybolmaması amacıyla daha uzun süre saklanabilir.

Varsayılan politika ayrıntılı hareketlerde en az 36 ay, aylık bilanço özetlerinde 10 yıla kadar yerel saklamadır. Bir dönemin özet kaydı güvenli şekilde oluşturulmadan o döneme ait ayrıntılı hareketler otomatik olarak temizlenmez.

## 3. Sunucu tarafında tutulan bilgiler

Uygulamanın temel finansal kayıtları sunucu tarafında zorunlu olarak saklanmaz. Çevrimiçi servislerin kullanılabilmesi için anonim cihaz oturumu, kısa ömürlü erişim belirteçleri ve teknik güvenlik verileri işlenebilir.

Kullanıcı isteğe bağlı bir bulut hesabı veya şifreli yedekleme özelliği kullanırsa, yedek veri sunucuda yalnızca şifreli/opaque biçimde tutulacak şekilde tasarlanmıştır.

## 4. Yapay zekâ ve dış servisler

Asistanın hesaplanabilir finansal işlevleri — bilanço özeti, borç ödeme sırası, kredi kartı/KMH özeti, gelir-gider analizi ve ödeme kapasitesi gibi işlemler — mümkün olduğunda cihaz üzerinde deterministik olarak hesaplanır.

Kullanıcı gelişmiş yapay zekâ açıklaması istediğinde, doğrudan kimlik bilgileri kaldırılmış ve mümkün olduğunca asgariye indirilmiş finansal özet dış yapay zekâ altyapısına iletilebilir. Ad, e-posta, telefon, T.C. kimlik numarası, IBAN ve tam kart numarası gibi doğrudan tanımlayıcıların yapay zekâ bağlamına dahil edilmemesi hedeflenir.

Çevrimiçi yapay zekâ ve barındırma hizmetlerinin Türkiye dışında altyapı kullanması mümkündür. Kullanıcı gelişmiş AI özelliklerini kullanmayarak bu aktarımı sınırlandırabilir.

## 5. Faiz ve finansal referans verileri

Kredi kartı ve KMH için TCMB tarafından yayımlanan azami faiz oranları ve diğer kamuya açık finansal referanslar uygulamada bilgi amaçlı gösterilebilir. Bankanın kullanıcıya sunduğu gerçek sözleşme oranı farklı olabilir. Kullanıcı otomatik getirilen oranları düzenleyebilir.

Finansal Asistanım yatırım danışmanlığı hizmeti vermez; hisse, fon, kripto veya başka bir sermaye piyasası aracı için kişiye özel al/sat talimatı üretmek amacıyla tasarlanmamıştır.

## 6. Bildirimler

Kullanıcı izin verirse uygulama yaklaşan ödemeler, haftalık bilanço özeti ve genel finansal disiplin hatırlatmaları için yerel bildirim gönderebilir. Bildirim zamanları ve kategorileri Ayarlar bölümünden değiştirilebilir veya tamamen kapatılabilir.

## 7. Satın alma ve abonelikler

Premium özellikler Apple App Store üzerinden otomatik yenilenen abonelik olarak sunulabilir. Ödeme, yenileme ve iptal işlemleri Apple hesabı üzerinden yönetilir. Uygulama kredi kartı ödeme bilgilerini kendi sunucusunda işlemez veya saklamaz.

Uygun kullanıcılara App Store Connect üzerinden tanımlanan ücretsiz deneme veya tanıtım teklifi sunulabilir. Deneme ve abonelik uygunluğu Apple tarafından belirlenir.

## 8. Kullanıcının kontrolü

Kullanıcı uygulama içinden finansal kayıtlarını ekleyebilir, düzenleyebilir ve silebilir. Yerel veriler uygulama kaldırıldığında veya kullanıcı tarafından veri silme işlemi yapıldığında cihazdan kaldırılabilir. İsteğe bağlı sunucu hesabı kullanılıyorsa ilgili hesap ve yedek verileri için ayrıca silme işlemi sağlanabilir.

## 9. Güvenlik

Uygulama; cihaz kilidi/Face ID, iOS Keychain, uygulama içi şifreleme, TLS bağlantısı, kısa ömürlü oturum belirteçleri ve veri minimizasyonu gibi kontroller kullanır. İnternet/mobil bankacılık parolası, kart CVV'si, PIN veya SMS/OTP kodlarının uygulamaya girilmemesi gerekir.

## 10. Lisans ve EULA

Uygulamanın App Store dağıtımında özel bir EULA tanımlanmadığı sürece Apple'ın standart Licensed Application End User License Agreement koşulları uygulanır. Uygulamadaki üçüncü taraf yazılım bileşenleri kendi lisans koşullarına tabi olabilir.

## 11. Destek

Finansal Asistanım ile ilgili teknik destek, hata bildirimi veya gizlilik soruları için **hpehlivanlar.io** üzerinden geliştirici iletişim kanallarını kullanabilirsiniz.

Bu sayfa ürünün teknik mimarisini açıklamak amacıyla hazırlanmıştır; yürürlükteki KVKK ve diğer mevzuat kapsamındaki nihai hukuki metinlerin yayın öncesinde hukuk danışmanı tarafından gözden geçirilmesi önerilir.
