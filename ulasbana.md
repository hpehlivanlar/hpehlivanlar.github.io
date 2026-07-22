---
layout: page
title: Ulaş Bana
subtitle: Proje, iş birliği, uygulama desteği ve teknik konular için iletişim kanalları.
permalink: /ulasbana/
---

<style>
.contact-page {
  --contact-border: #e3e7ee;
  --contact-text: #263238;
  --contact-muted: #64748b;
  --contact-primary: #1769e0;
  --contact-primary-dark: #0f4fae;
  --contact-soft: #f6f8fb;
  margin-top: 12px;
}

.contact-intro {
  max-width: 780px;
  margin: 0 auto 32px;
  text-align: center;
}

.contact-intro h2 {
  margin: 0 0 12px;
  font-size: 30px;
  line-height: 1.25;
  color: var(--contact-text);
}

.contact-intro p {
  margin: 0;
  color: var(--contact-muted);
  font-size: 17px;
  line-height: 1.75;
}

.contact-primary {
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 22px;
  padding: 26px;
  margin: 0 0 28px;
  border: 1px solid #cfe0ff;
  border-radius: 18px;
  background: linear-gradient(135deg, #f5f9ff 0%, #eef5ff 100%);
  box-shadow: 0 8px 24px rgba(23, 105, 224, 0.08);
}

.contact-primary-content {
  display: flex;
  align-items: center;
  gap: 18px;
}

.contact-primary-icon {
  display: flex;
  align-items: center;
  justify-content: center;
  flex: 0 0 58px;
  width: 58px;
  height: 58px;
  border-radius: 16px;
  background: var(--contact-primary);
  color: #ffffff;
  font-size: 26px;
}

.contact-primary h3 {
  margin: 0 0 6px;
  font-size: 21px;
  color: var(--contact-text);
}

.contact-primary p {
  margin: 0;
  color: var(--contact-muted);
  line-height: 1.6;
}

.contact-email {
  display: inline-block;
  margin-top: 5px;
  font-weight: 700;
  color: var(--contact-primary-dark);
  word-break: break-word;
}

.contact-button {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  gap: 8px;
  min-width: 154px;
  padding: 12px 18px;
  border-radius: 10px;
  background: var(--contact-primary);
  color: #ffffff !important;
  font-weight: 700;
  text-decoration: none !important;
  transition: transform 0.2s ease, background 0.2s ease;
}

.contact-button:hover {
  transform: translateY(-2px);
  background: var(--contact-primary-dark);
}

.contact-grid {
  display: grid;
  grid-template-columns: repeat(3, minmax(0, 1fr));
  gap: 16px;
  margin-bottom: 30px;
}

.contact-card {
  display: flex;
  align-items: center;
  gap: 14px;
  min-height: 96px;
  padding: 18px;
  border: 1px solid var(--contact-border);
  border-radius: 14px;
  background: #ffffff;
  color: var(--contact-text) !important;
  text-decoration: none !important;
  box-shadow: 0 5px 16px rgba(15, 23, 42, 0.05);
  transition: transform 0.2s ease, box-shadow 0.2s ease, border-color 0.2s ease;
}

.contact-card:hover {
  transform: translateY(-3px);
  border-color: #b8c9e6;
  box-shadow: 0 10px 24px rgba(15, 23, 42, 0.09);
}

.contact-card-icon {
  display: flex;
  align-items: center;
  justify-content: center;
  flex: 0 0 44px;
  width: 44px;
  height: 44px;
  border-radius: 12px;
  background: var(--contact-soft);
  font-size: 22px;
}

.contact-card h3 {
  margin: 0 0 3px;
  font-size: 17px;
  color: var(--contact-text);
}

.contact-card p {
  margin: 0;
  color: var(--contact-muted);
  font-size: 14px;
  line-height: 1.45;
}

.contact-help {
  padding: 24px;
  border: 1px solid var(--contact-border);
  border-radius: 16px;
  background: var(--contact-soft);
}

.contact-help h2 {
  margin: 0 0 10px;
  font-size: 23px;
  color: var(--contact-text);
}

.contact-help p {
  margin: 0 0 16px;
  color: var(--contact-muted);
  line-height: 1.7;
}

.contact-help-links {
  display: flex;
  flex-wrap: wrap;
  gap: 10px;
}

.contact-secondary-button {
  display: inline-flex;
  align-items: center;
  gap: 7px;
  padding: 10px 14px;
  border: 1px solid #cbd5e1;
  border-radius: 9px;
  background: #ffffff;
  color: #263238 !important;
  font-weight: 700;
  text-decoration: none !important;
}

.contact-secondary-button:hover {
  border-color: #94a3b8;
  background: #f8fafc;
}

.contact-note {
  margin-top: 22px;
  padding: 16px 18px;
  border-left: 4px solid var(--contact-primary);
  border-radius: 6px;
  background: #f8fbff;
  color: #475569;
  line-height: 1.65;
}

@media (max-width: 900px) {
  .contact-grid {
    grid-template-columns: repeat(2, minmax(0, 1fr));
  }
}

@media (max-width: 640px) {
  .contact-intro {
    text-align: left;
  }

  .contact-intro h2 {
    font-size: 25px;
  }

  .contact-primary {
    align-items: flex-start;
    flex-direction: column;
  }

  .contact-button {
    width: 100%;
  }

  .contact-grid {
    grid-template-columns: 1fr;
  }
}
</style>

<div class="contact-page">

  <section class="contact-intro">
    <h2>İletişim ve destek</h2>
    <p>
      Yazılım projeleri, mobil uygulamalar, teknik destek, iş birliği ve içeriklerle ilgili
      görüşleriniz için aşağıdaki iletişim kanallarını kullanabilirsiniz.
    </p>
  </section>

  <section class="contact-primary">
    <div class="contact-primary-content">
      <div class="contact-primary-icon" aria-hidden="true">
        <i class="fa fa-envelope"></i>
      </div>

      <div>
        <h3>Doğrudan e-posta gönderin</h3>
        <p>Uygulama desteği ve proje talepleri için en uygun iletişim kanalıdır.</p>
        <a class="contact-email" href="mailto:bysiskur@gmail.com">bysiskur@gmail.com</a>
      </div>
    </div>

    <a
      class="contact-button"
      href="mailto:bysiskur@gmail.com?subject=İletişim%20ve%20Destek%20Talebi">
      <i class="fa fa-paper-plane" aria-hidden="true"></i>
      E-posta Gönder
    </a>
  </section>

  <section class="contact-grid" aria-label="Sosyal medya ve iletişim bağlantıları">

    <a class="contact-card" href="https://github.com/hpehlivanlar" target="_blank" rel="noopener noreferrer">
      <div class="contact-card-icon" aria-hidden="true"><i class="fa fa-github"></i></div>
      <div>
        <h3>GitHub</h3>
        <p>Projeler, kaynak kodları ve geliştirme çalışmaları</p>
      </div>
    </a>

    <a class="contact-card" href="https://www.linkedin.com/in/hpehlivanlar" target="_blank" rel="noopener noreferrer">
      <div class="contact-card-icon" aria-hidden="true"><i class="fa fa-linkedin"></i></div>
      <div>
        <h3>LinkedIn</h3>
        <p>Profesyonel profil ve iş bağlantıları</p>
      </div>
    </a>

    <a class="contact-card" href="https://www.youtube.com/@hasanpehlivanlar" target="_blank" rel="noopener noreferrer">
      <div class="contact-card-icon" aria-hidden="true"><i class="fa fa-youtube-play"></i></div>
      <div>
        <h3>YouTube</h3>
        <p>Videolar, teknoloji ve içerik çalışmaları</p>
      </div>
    </a>

    <a class="contact-card" href="https://www.instagram.com/pehlivan__hasan" target="_blank" rel="noopener noreferrer">
      <div class="contact-card-icon" aria-hidden="true"><i class="fa fa-instagram"></i></div>
      <div>
        <h3>Instagram</h3>
        <p>Güncel paylaşımlar ve sosyal içerikler</p>
      </div>
    </a>

    <a class="contact-card" href="https://www.facebook.com/hpehlivanlr" target="_blank" rel="noopener noreferrer">
      <div class="contact-card-icon" aria-hidden="true"><i class="fa fa-facebook"></i></div>
      <div>
        <h3>Facebook</h3>
        <p>Sosyal paylaşımlar ve iletişim</p>
      </div>
    </a>

    <a class="contact-card" href="https://www.twitter.com/hasanpehlivanlr" target="_blank" rel="noopener noreferrer">
      <div class="contact-card-icon" aria-hidden="true"><i class="fa fa-twitter"></i></div>
      <div>
        <h3>X / Twitter</h3>
        <p>Kısa paylaşımlar ve güncel notlar</p>
      </div>
    </a>

  </section>

  <section class="contact-help">
    <h2>Mobil uygulama desteği</h2>
    <p>
      Kuran Ayet Widget, Eser Prompter veya Kırmızı Balık uygulamalarından biriyle ilgili
      destek talebinde bulunurken mesajınıza uygulama adını, cihaz modelini, iOS sürümünü
      ve yaşadığınız sorunun kısa açıklamasını eklemeniz çözüm sürecini kolaylaştırır.
    </p>

    <div class="contact-help-links">
      <a class="contact-secondary-button" href="{{ '/uygulamalar/' | relative_url }}">
        <i class="fa fa-mobile" aria-hidden="true"></i>
        Uygulamaları Görüntüle
      </a>

      <a
        class="contact-secondary-button"
        href="mailto:bysiskur@gmail.com?subject=Mobil%20Uygulama%20Destek%20Talebi">
        <i class="fa fa-life-ring" aria-hidden="true"></i>
        Destek Talebi Oluştur
      </a>
    </div>
  </section>

  <div class="contact-note">
    <strong>Not:</strong> Teknik bir hata bildirirken mümkünse ekran görüntüsü, hata mesajı ve
    sorunu oluşturan işlem adımlarını da ekleyin. Parola, kredi kartı bilgisi veya benzeri
    hassas verileri e-posta ile göndermeyin.
  </div>

</div>
