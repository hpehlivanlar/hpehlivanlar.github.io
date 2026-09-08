---
layout: page
title: Uygulamalar
subtitle: Mobil uygulamalar ve gizlilik politikaları
permalink: /uygulamalar/
---

<!-- last-updated: 2026-09-08 16:31 TRT -->

<style>
.app-list {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
  gap: 20px;
  margin-top: 28px;
}

.app-card {
  border: 1px solid #dddddd;
  border-radius: 14px;
  padding: 22px;
  background: #ffffff;
  box-shadow: 0 4px 14px rgba(0, 0, 0, 0.08);
}

.app-card h2 {
  margin-top: 0;
  margin-bottom: 12px;
}

.app-card p {
  line-height: 1.65;
  color: #555555;
  min-height: 105px;
}

.app-icon {
  font-size: 48px;
  margin-bottom: 12px;
}

.app-links {
  display: flex;
  flex-wrap: wrap;
  gap: 10px;
  margin-top: 18px;
}

.app-button {
  display: inline-block;
  padding: 10px 15px;
  border-radius: 8px;
  text-decoration: none !important;
  font-weight: 600;
}

.privacy-button {
  background-color: #1f6feb;
  color: #ffffff !important;
}

.contact-button {
  background-color: #eeeeee;
  color: #222222 !important;
}
</style>

Bu sayfada geliştirdiğim mobil uygulamaları, destek bağlantılarını ve uygulamalara ait gizlilik politikalarını inceleyebilirsiniz.

<div class="app-list">

  <div class="app-card" id="finansal-asistanim">
    <div class="app-icon">💳</div>
    <h2>Finansal Asistanım</h2>
    <p>
      Banka hesapları, kredi kartları, KMH/ek hesaplar, krediler, gelir ve giderleri
      tek yerde takip etmeye; bilanço, nakit akışı ve ödeme planı oluşturmaya yardımcı
      olan, local-first veri saklama yaklaşımına sahip kişisel finans iOS uygulamasıdır.
    </p>
    <div class="app-links">
      <a class="app-button privacy-button" href="{{ '/finans-asistanim-gizlilik/' | relative_url }}">Gizlilik Politikası</a>
      <a class="app-button contact-button" href="{{ '/ulasbana/' | relative_url }}">Destek</a>
      <a class="app-button contact-button" href="https://www.apple.com/legal/internet-services/itunes/dev/stdeula/">EULA</a>
    </div>
  </div>

  <div class="app-card" id="hgs-ihlal-takip">
    <div class="app-icon">🚗</div>
    <h2>HGS İhlal Takip</h2>
    <p>
      Türkiye'deki otoyol ve köprü geçiş ihlallerini plaka bazında takip etmeye,
      kayıtlı plakalar için yaklaşık 8 saatlik periyodik kontrollerle yeni ihlal
      bildirimi almaya ve ödeme hatırlatmaları oluşturmaya yardımcı olan bağımsız
      iOS uygulamasıdır. KGM, PTT veya HGS'nin resmî uygulaması değildir.
    </p>
    <div class="app-links">
      <a class="app-button privacy-button" href="{{ '/hgs-ihlal-takip-gizlilik/' | relative_url }}">Gizlilik Politikası</a>
      <a class="app-button contact-button" href="{{ '/ulasbana/' | relative_url }}">Destek</a>
      <a class="app-button contact-button" href="https://www.apple.com/legal/internet-services/itunes/dev/stdeula/">EULA</a>
    </div>
  </div>

  <div class="app-card" id="ilac-recetem">
    <div class="app-icon">💊</div>
    <h2>İlaç Reçetem</h2>
    <p>
      Özellikle okuma-yazma bilmeyen, görme güçlüğü yaşayan veya birden fazla
      ilacı ayırt etmekte zorlanan kullanıcılar için renk, sembol, ilaç kutusu
      fotoğrafı ve sesli bildirimlerle ilaç takibini kolaylaştıran iOS uygulamasıdır.
    </p>
    <div class="app-links">
      <a class="app-button privacy-button" href="{{ '/ilac-recetem-gizlilik/' | relative_url }}">Gizlilik Politikası</a>
      <a class="app-button contact-button" href="mailto:bysiskur@gmail.com?subject=Ilac%20Recetem%20Destek">Destek</a>
    </div>
  </div>

  <div class="app-card" id="adkal">
    <div class="app-icon">🛡️</div>
    <h2>AdKal</h2>
    <p>
      iPhone ve iPad’de bilinen reklam, izleyici ve zararlı alan adlarını
      DNS düzeyinde filtreleyen; Wi-Fi ve mobil veride şifreli
      DNS-over-HTTPS koruması sunan iOS uygulamasıdır.
    </p>
    <div class="app-links">
      <a class="app-button privacy-button" href="{{ '/adkal-gizlilik/' | relative_url }}">Gizlilik Politikası</a>
      <a class="app-button contact-button" href="mailto:bysiskur@gmail.com?subject=AdKal%20Destek">Destek</a>
    </div>
  </div>

  <div class="app-card" id="dudi">
    <div class="app-icon">🧸</div>
    <h2>DuDi</h2>
    <p>
      İki ayıcığı labirentin kalbinde buluşturan; 100 bölüm, tek ve iki
      oyunculu oyun modları ile 10 farklı sıcak yuva alanı sunan sevimli
      bir iOS bulmaca oyunudur. İlk 10 bölüm ücretsiz oynanabilir.
    </p>
    <div class="app-links">
      <a class="app-button privacy-button" href="{{ '/kalp-koprusu-gizlilik/' | relative_url }}">Gizlilik Politikası</a>
      <a class="app-button contact-button" href="{{ '/ulasbana/' | relative_url }}">Destek</a>
    </div>
  </div>

  <div class="app-card" id="mevzuhakkim">
    <div class="app-icon">⚖️</div>
    <h2>MevzuHakkım</h2>
    <p>
      Türkiye’deki mevzuata, Anayasa maddelerine ve ilgili resmî
      kaynaklara erişimi kolaylaştıran AI destekli mevzuat araştırma
      ve bilgilendirme uygulamasıdır.
    </p>
    <div class="app-links">
      <a class="app-button privacy-button" href="https://hpehlivanlar.github.io/mevzuhakkim-gizlilik/">Gizlilik Politikası</a>
      <a class="app-button contact-button" href="mailto:bysiskur@gmail.com?subject=MevzuHakkim%20Destek">Destek</a>
    </div>
  </div>

  <div class="app-card" id="eser-prompter">
    <div class="app-icon">🎤</div>
    <h2>Eser Prompter</h2>
    <p>
      Türkü, şiir, konuşma ve diğer eser metinlerini kaydetmeyi,
      düzenlemeyi ve otomatik kayan teleprompter ekranında
      görüntülemeyi sağlayan iOS uygulamasıdır.
    </p>
    <div class="app-links">
      <a class="app-button privacy-button" href="{{ '/eser-prompter-gizlilik/' | relative_url }}">Gizlilik Politikası</a>
      <a class="app-button contact-button" href="mailto:bysiskur@gmail.com?subject=Eser%20Prompter%20Destek">Destek</a>
    </div>
  </div>

  <div class="app-card" id="kirmizi-balik">
    <div class="app-icon">🐟</div>
    <h2>Kırmızı Balık</h2>
    <p>
      Deniz ortamında yıldızların toplandığı, engellerin aşıldığı
      ve bölümlerin tamamlandığı çocuklara uygun eğlenceli bir
      mobil oyundur.
    </p>
    <div class="app-links">
      <a class="app-button privacy-button" href="{{ '/kirmizi-balik-gizlilik/' | relative_url }}">Gizlilik Politikası</a>
      <a class="app-button contact-button" href="mailto:bysiskur@gmail.com?subject=Kirmizi%20Balik%20Destek">Destek</a>
    </div>
  </div>

  <div class="app-card" id="kuran-ayet-widget">
    <div class="app-icon">📖</div>
    <h2>Kuran Ayet Widget</h2>
    <p>
      Kur'an-ı Kerim ayetlerini, Türkçe meallerini ve sure bilgilerini
      uygulama içinde, ana ekran widget'larında ve kilit ekranı
      widget'larında görüntülemeyi sağlayan iOS uygulamasıdır.
    </p>
    <div class="app-links">
      <a class="app-button privacy-button" href="{{ '/kuran-ayet-widget-gizlilik/' | relative_url }}">Gizlilik Politikası</a>
      <a class="app-button contact-button" href="mailto:bysiskur@gmail.com?subject=Kuran%20Ayet%20Widget%20Destek">Destek</a>
    </div>
  </div>

</div>

---

## İletişim ve destek

**Geliştirici:** Hasan Pehlivanlar  
**E-posta:** [bysiskur@gmail.com](mailto:bysiskur@gmail.com)
