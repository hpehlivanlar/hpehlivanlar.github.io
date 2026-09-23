---
layout: post
title: "GitHub Copilot'a Yerel Sandbox Geldi: Kod Ajanlarında Dosya ve Ağ Güvenliği"
subtitle: "23 Eylül 2026 duyurulan public preview, yerel ajan oturumlarının erişebileceği dosyaları, ağı ve kimlik bilgilerini proje bazında sınırlamayı amaçlıyor."
date: 2026-09-24 00:00:00 +0300
author: Hasan Pehlivanlar
thumbnail-img: "/assets/img/2026-09-24-copilot-yerel-sandbox.svg"
tags: [GitHub Copilot, Yapay Zeka, Güvenlik, Yazılım Geliştirme, Kod Ajanları]
---

Kod üreten ajanlara yalnızca öneri yazdırmakla, onlara terminal çalıştırma ve proje dosyalarını değiştirme yetkisi vermek aynı güvenlik modeli değil. **GitHub, 23 Eylül 2026'da Copilot uygulaması için yerel sandbox özelliğini public preview olarak duyurdu.** Yeni özellik, yerel depo ve çalışma ağacı oturumlarında ajanın sistem kaynaklarına erişimini sınırlamaya yardımcı oluyor.

Bu duyuru, yapay zeka destekli yazılım geliştirmede önemli bir soruyu yeniden öne çıkarıyor: Bir ajana görevi yaptırırken **hangi dosyalara ve sistem yetkilerine gerçekten ihtiyaç duyduğunu** nasıl tanımlıyoruz?

## Yerel sandbox hangi alanları kontrol ediyor?

GitHub'ın duyurusuna göre proje bazındaki sandbox ayarları üç ana alanı kapsıyor:

- **Dosya sistemi:** Ek okuma-yazma izni verilen klasörler, yalnızca okunabilir klasörler ve erişimi reddedilen klasörler.
- **Ağ:** İnternete çıkış ve yerel ağ erişimiyle ilgili seçenekler.
- **Kimlik bilgileri:** Kimlik doğrulamalı HTTPS Git işlemleri için Git bilgileri ve GitHub CLI kimlik bilgileri.

Bu seçenekler, proje bazında yeni bir oturum açılırken talep edilen erişim politikasını belirliyor. Kurumsal yöneticilerin uyguladığı ayarlar, etkin izinleri daha da kısıtlayabiliyor.

## Özellik varsayılan olarak kapalı

Yerel sandbox **varsayılan olarak etkin değil**. Copilot uygulamasında ilgili projeyi seçip Sandbox bölümündeki **Sandbox new sessions** seçeneğini açmak gerekiyor. Bu ayar yalnızca yeni başlayan oturumları etkiliyor; daha önce başlamış oturumlara otomatik olarak uygulanmıyor.

Etkin bir yerel oturumda sandbox'ı açmak için şu komut da kullanılabiliyor:

~~~text
/sandbox on
~~~

Dosya, ağ veya kimlik bilgisi ayarlarında yapılan değişiklikler yeni oturumlarda ya da mevcut oturum yeniden başlatıldığında geçerli oluyor.

## Koruma sınırlarını doğru anlamak

GitHub, işletim sistemi istenen güvenlik politikasını uygulayamıyorsa sandbox'lı kabuğun korumasız devam etmek yerine hata vereceğini belirtiyor. Bu davranış, izinsiz çalışmayı sessizce kabul etmemek açısından önemli.

Ancak özelliğin kapsamı sınırlı: Duyurudaki yerel sandbox, **bulut sandbox oturumlarına veya uzak sunucudaki oturumlara uygulanmıyor**. Ayrıca Copilot uygulaması ile Copilot CLI'ın sandbox ayarları ayrı yönetiliyor. Özellik public preview durumunda olduğu için davranış ve seçenekler değişebilir.

Sandbox, insan onayının veya kod incelemesinin yerini de almıyor. Kaynak kod değişikliklerini, oluşturulan komutları, bağımlılık güncellemelerini ve ağa çıkan işlemleri yine denetlemek gerekiyor.

## Geliştirme ekipleri nasıl kullanabilir?

Bir ajanı büyük bir projede denemeden önce **en az yetki** yaklaşımıyla başlamak mantıklı:

1. Görevin gerçekten dokunacağı kaynak klasörlerini belirleyin.
2. Gizli anahtarların, sertifikaların ve üretim yapılandırmalarının olduğu klasörleri erişim dışı tutun.
3. Ağ erişimine yalnızca bağımlılık indirme veya gerekli test servisleri için ihtiyaç varsa izin verin.
4. Ajanın değişikliklerini ayrı bir Git dalında tutun.
5. Testleri çalıştırın; diff'i insan incelemesinden geçirmeden üretim dalına birleştirmeyin.

Bu önlemler özellikle birden fazla depoda, aynı geliştirme makinesinde veya farklı müşteri ortamlarında çalışan ekipler için dikkat gerektiriyor.

## Sonuç

Yerel sandbox, kod ajanlarının yetkisini görünür ve sınırlanabilir hale getirme yönünde yeni bir araç. Temel ilke değişmiyor: **Ajana işi yapması için gereken erişimi verin; üretim verilerine, kimlik bilgilerine ve alakasız dosyalara varsayılan erişim vermeyin.**

---

**Kaynaklar**

- [GitHub Changelog: Local sandboxing in the GitHub Copilot app (23 Eylül 2026)](https://github.blog/changelog/2026-09-23-local-sandboxing-in-the-github-copilot-app/)
- [GitHub Copilot belgeleri](https://docs.github.com/en/copilot)
