---
layout: page
title: Adresliyorum
subtitle: Kiracı, ev sahibi ve konut için kontrollü referans geçmişi
permalink: /adresliyorum/
---

<style>
.adres-hero {
  border: 1px solid #ececec;
  border-radius: 18px;
  padding: 28px;
  background: linear-gradient(135deg, #ffffff 0%, #fff8d9 100%);
  margin: 12px 0 28px;
}
.adres-hero h2 { margin-top: 0; font-size: 30px; }
.adres-badge {
  display: inline-block;
  background: #ffc400;
  color: #1f1f1f;
  border-radius: 999px;
  padding: 7px 12px;
  font-weight: 700;
  margin-bottom: 14px;
}
.adres-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(240px, 1fr));
  gap: 16px;
  margin: 24px 0;
}
.adres-card {
  border: 1px solid #e7e7e7;
  border-radius: 14px;
  padding: 20px;
  background: #ffffff;
}
.adres-card h3 { margin-top: 0; }
.adres-actions {
  display: flex;
  flex-wrap: wrap;
  gap: 10px;
  margin: 24px 0;
}
.adres-btn {
  display: inline-block;
  padding: 11px 16px;
  border-radius: 9px;
  text-decoration: none !important;
  font-weight: 700;
}
.adres-btn.primary { background: #ffc400; color: #1e1e1e !important; }
.adres-btn.dark { background: #222222; color: #ffffff !important; }
.adres-btn.light { background: #eeeeee; color: #222222 !important; }
.adres-flow {
  border-left: 4px solid #ffc400;
  padding-left: 18px;
  margin: 22px 0;
}
</style>

<div class="adres-hero">
  <div class="adres-badge">Adres bazlı güven ve referans sistemi</div>
  <h2>Kiralamada geçmişi görün, kararınızı bilgiyle verin.</h2>
  <p>
    <strong>Adresliyorum</strong>; kiracı, ev sahibi ve konut geçmişini doğrulanmış kiralama ilişkileri
    üzerinden değerlendiren ve bu geçmişe KRC / EV referans kodlarıyla kontrollü erişim sağlayan
    iOS ve web platformudur.
  </p>
  <p>
    Sistem herkese açık bir kişi arama veya kara liste hizmeti değildir. Geçmiş bilgiler; kullanıcı hesabı,
    doğrulanmış kiralama, konut sahipliği ve süreli referans paylaşımı gibi yetki kontrolleriyle sınırlandırılır.
  </p>
</div>

<div class="adres-actions">
  <a class="adres-btn primary" href="https://www.adresliyorum.com">Web Sitesi</a>
  <a class="adres-btn dark" href="https://www.adresliyorum.com/app">Web Uygulamasını Aç</a>
  <a class="adres-btn light" href="{{ '/adresliyorum-gizlilik-bildirimi/' | relative_url }}">Gizlilik & KVKK</a>
</div>

## Nasıl çalışır?

<div class="adres-flow">
<strong>Kiracı → Konut ve ev sahibi</strong><br>
Bir kiracı, doğrulanmış olarak yaşadığı konutu ve ilgili ev sahibini değerlendirebilir.
</div>

<div class="adres-flow">
<strong>Ev sahibi → Kiracı</strong><br>
Ev sahibi, kiralama tamamlandıktan sonra o konutta yaşamış kiracıyı ödeme düzeni, bakım, iletişim ve sözleşme uyumu gibi kriterlerle değerlendirebilir.
</div>

<div class="adres-flow">
<strong>KRC referans kodu</strong><br>
Kiracı kendi doğrulanmış geçmişini aday ev sahibiyle süreli ve kontrollü bir KRC kodu aracılığıyla paylaşabilir.
</div>

<div class="adres-flow">
<strong>EV referans kodu</strong><br>
Aday kiracı, EV kodu üzerinden konut ve ilgili ev sahibinin doğrulanmış geçmişini görüntüleyebilir.
</div>

## Temel özellikler

<div class="adres-grid">
  <div class="adres-card">
    <h3>🏠 Konutlarım</h3>
    <p>Daire, villa, ofis ve rezidans kayıtları; haritadan konum seçme, adres arama ve konumdan açık adres bulma.</p>
  </div>
  <div class="adres-card">
    <h3>🗺️ Harita</h3>
    <p>Kamuya açık görünümde kontrollü/özet konut bilgileri ve yaklaşık konum yaklaşımı.</p>
  </div>
  <div class="adres-card">
    <h3>🔑 Referans Merkezi</h3>
    <p>KRC ve EV kodu oluşturma, sorgulama, gelen/giden referans taleplerini yönetme.</p>
  </div>
  <div class="adres-card">
    <h3>📋 Kiralama Geçmişi</h3>
    <p>Aktif ve tamamlanmış kiralamaları, başlangıç ve çıkış tarihlerini aynı hesap üzerinden takip etme.</p>
  </div>
  <div class="adres-card">
    <h3>⭐ Karşılıklı Değerlendirme</h3>
    <p>Kiracı, ev sahibi ve konut için ayrı puanlama; yazılı yorum, yanıt ve içerik moderasyonu.</p>
  </div>
  <div class="adres-card">
    <h3>🔒 Gizlilik Odaklı Tasarım</h3>
    <p>İsim, telefon veya e-posta üzerinden herkese açık geçmiş araması yerine referans kodu ve doğrulanmış ilişki temelli erişim.</p>
  </div>
</div>

## Konum ve adres yaklaşımı

Konut ekleme veya düzenleme sırasında kullanıcı Apple Maps üzerinden adres arayabilir, haritadan bir nokta seçebilir ve seçilen koordinatın açık adresini otomatik olarak alabilir. Otomatik bulunan adres kullanıcı tarafından kaydetmeden önce düzenlenebilir.

Tam açık adres ve kesin konumun herkese açık yayınlanması varsayılan davranış değildir. Kamuya açık harita görünümünde daha sınırlı ve yaklaşık konum bilgisi kullanılması hedeflenir.

## Çoklu dil

Adresliyorum uygulaması için aşağıdaki dil seçenekleri planlanmış / desteklenmektedir:

- Türkçe
- English
- العربية
- 简体中文

## Planlar

Adresliyorum; temel özelliklerin kullanılabildiği ücretsiz plan ile daha yüksek sorgu/konut limitleri ve gelişmiş özellikler sunan ücretli planlar içerebilir.

Uygulamadaki güncel fiyat ve abonelik koşulları, kullanıcının App Store bölgesine göre Apple tarafından gösterilir. Abonelik işlemleri App Store / StoreKit üzerinden yürütülür.

## Gizlilik, KVKK ve EULA

**Gizlilik Politikası ve KVKK Aydınlatma Metni:**  
[Adresliyorum Gizlilik Politikası]({{ '/adresliyorum-gizlilik-bildirimi/' | relative_url }})

**Apple Standart EULA:**  
[Licensed Application End User License Agreement](https://www.apple.com/legal/internet-services/itunes/dev/stdeula/)

## Destek

**Geliştirici:** Hasan Pehlivanlar  
**E-posta:** [bysiskur@gmail.com](mailto:bysiskur@gmail.com)  
**Web:** [www.adresliyorum.com](https://www.adresliyorum.com)  
**Destek:** [Ulaş Bana]({{ '/ulasbana/' | relative_url }})

[← Uygulamalar sayfasına dön]({{ '/uygulamalar/' | relative_url }})
