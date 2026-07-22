---
layout: page
title: Uygulamalar
subtitle: Geliştirdiğim mobil uygulamalar
permalink: /uygulamalar/
---

<style>
.app-list {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
  gap: 22px;
  margin-top: 30px;
}

.app-card {
  border: 1px solid #dddddd;
  border-radius: 14px;
  padding: 24px;
  background: #ffffff;
  box-shadow: 0 4px 14px rgba(0, 0, 0, 0.08);
  transition: transform 0.2s ease, box-shadow 0.2s ease;
}

.app-card:hover {
  transform: translateY(-4px);
  box-shadow: 0 8px 22px rgba(0, 0, 0, 0.12);
}

.app-icon {
  font-size: 52px;
  margin-bottom: 12px;
}

.app-card h2 {
  margin-top: 0;
  margin-bottom: 12px;
  font-size: 25px;
}

.app-card p {
  line-height: 1.65;
  color: #555555;
  min-height: 105px;
}

.app-links {
  display: flex;
  flex-wrap: wrap;
  gap: 10px;
  margin-top: 20px;
}

.app-button {
  display: inline-block;
  padding: 10px 15px;
  border-radius: 8px;
  text-decoration: none !important;
  font-weight: 600;
  transition: opacity 0.2s ease;
}

.app-button:hover {
  opacity: 0.82;
}

.privacy-button {
  background-color: #1f6feb;
  color: #ffffff !important;
}

.contact-button {
  background-color: #eeeeee;
  color: #222222 !important;
}

.app-store-button {
  background-color: #111111;
  color: #ffffff !important;
}
</style>

# Mobil Uygulamalar

Bu sayfada geliştirdiğim mobil uygulamaları ve uygulamalara ait gizlilik politikalarını inceleyebilirsiniz.

<div class="app-list">

  <div class="app-card">
    <div class="app-icon">📖</div>

    <h2>Kuran Ayet Widget</h2>

    <p>
      Kur'an-ı Kerim ayetlerini, Türkçe meallerini ve sure bilgilerini
      uygulama içerisinde, ana ekran widget'larında ve kilit ekranı
      widget'larında görüntülemenizi sağlayan iOS uygulamasıdır.
    </p>

    <div class="app-links">
      <a
        class="app-button privacy-button"
        href="{{ '/kuran-ayet-widget-gizlilik/' | relative_url }}">
        Gizlilik Politikası
      </a>

      <a
        class="app-button contact-button"
        href="mailto:bysiskur@gmail.com?subject=Kuran%20Ayet%20Widget%20Destek">
        Destek
      </a>
    </div>
  </div>


  <div class="app-card">
    <div class="app-icon">🎤</div>

    <h2>Eser Prompter</h2>

    <p>
      Türkü, şiir, konuşma ve diğer eser metinlerini kaydetmenizi,
      düzenlemenizi ve otomatik kayan teleprompter ekranında
      görüntülemenizi sağlayan iOS uygulamasıdır.
    </p>

    <div class="app-links">
      <a
        class="app-button privacy-button"
        href="{{ '/eser-prompter-gizlilik/' | relative_url }}">
        Gizlilik Politikası
      </a>

      <a
        class="app-button contact-button"
        href="mailto:bysiskur@gmail.com?subject=Eser%20Prompter%20Destek">
        Destek
      </a>
    </div>
  </div>


  <div class="app-card">
    <div class="app-icon">🐟</div>

    <h2>Kırmızı Balık</h2>

    <p>
      Deniz canlıları, yıldızlar ve çeşitli engeller içeren eğlenceli
      bir mobil oyundur. Oyuncu, kırmızı balığı yönlendirerek yıldızları
      toplar ve bölümleri tamamlamaya çalışır.
    </p>

    <div class="app-links">
      <a
        class="app-button privacy-button"
        href="{{ '/kirmizi-balik-gizlilik/' | relative_url }}">
        Gizlilik Politikası
      </a>

      <a
        class="app-button contact-button"
        href="mailto:bysiskur@gmail.com?subject=Kirmizi%20Balik%20Destek">
        Destek
      </a>
    </div>
  </div>

</div>

---

## İletişim ve destek

Uygulamalarla ilgili soru, görüş, hata bildirimi ve gizlilik talepleriniz için:

**Geliştirici:** Hasan Pehlivanlar  
**E-posta:** [bysiskur@gmail.com](mailto:bysiskur@gmail.com)