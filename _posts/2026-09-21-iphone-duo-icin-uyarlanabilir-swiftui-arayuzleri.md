---
layout: post
title: "iPhone Duo İçin Uygulama Tasarımı: SwiftUI'da Katlanabilir Ekrana Hazırlık"
subtitle: "Apple'ın yeni çok ekranlı iPhone'u, sabit ekran ölçülerine dayanan tasarımları yeniden değerlendirmeyi gerektiriyor."
date: 2026-09-21 18:00:00 +0300
author: Hasan Pehlivanlar
thumbnail-img: "/assets/img/2026-09-21-iphone-duo-uyarlanabilir-arayuz.svg"
tags: [iPhone Duo, SwiftUI, iOS 27, Xcode, Mobil Tasarım]
---

Apple'ın ilk çok ekranlı iPhone modeli **iPhone Duo** için geliştirici kaynakları 18 Eylül 2026'da genişletildi. Apple'ın yayımladığı takvime göre cihazın **23 Ekim 2026'da** iOS 27.1 ile kullanıma sunulması planlanıyor. Xcode 27.1 beta ve yeni tasarım kaynakları sayesinde uygulamaları şimdiden farklı açılma durumlarında test etmek mümkün.

Buradaki önemli değişiklik yalnızca ekranın büyümesi değil. Aynı uygulama kapalı, açık, yatay veya kısmen katlanmış durumda farklı kullanılabilir alanlarla karşılaşabiliyor.

## Sabit çözünürlük yerine kullanılabilir alan

Apple'ın teknik oturumlarında vurguladığı ilk ilke, arayüz kararlarını cihaz adından veya sabit ekran boyutundan çıkarmamak. SwiftUI için environment değerlerini, UIKit için trait collection'ı kullanmak daha güvenilir bir yaklaşım.

Duo'nun dış ekranı dikey kullanımda diğer iPhone'lara benzer biçimde yatayda compact size class sunuyor. İç ekran açıldığında ise yatay ve dikey eksende regular alan elde edilebiliyor. Bu durum, daha fazla içerik ve yan menü göstermek için fırsat yaratıyor.

Örneğin tek sütunlu bir etkinlik listesi, açık ekranda kategori listesi ve etkinlik ayrıntısını yan yana gösterebilir.

## NavigationSplitView ile temel uyarlanabilir yapı

SwiftUI'daki NavigationSplitView, küçük alanda tek sütuna daralabilen; geniş alanda ise gezinme ve ayrıntı sütunlarını gösterebilen yerleşimler için uygun bir başlangıç noktasıdır.

~~~swift
import SwiftUI

struct AdaptiveHomeView: View {
    @State private var selection: String?
    private let sections = ["Etkinlikler", "Favoriler", "Ayarlar"]

    var body: some View {
        NavigationSplitView {
            List(sections, id: \.self, selection: $selection) { section in
                Text(section)
            }
            .navigationTitle("Bölümler")
        } detail: {
            Text(selection ?? "Bir bölüm seçin")
                .navigationTitle(selection ?? "Ana Sayfa")
        }
    }
}
~~~

Bu örnek özel bir iPhone Duo kontrolü kullanmıyor. Amacı, **cihazın kapalı veya açık olmasına göre sistemin kendisinin uyarlayabildiği** bir gezinme yapısı kurmak.

## Menteşe ve kamera alanlarına dikkat

Duo'da kullanılabilir alan her zaman düz bir dikdörtgen gibi düşünülemez. Menteşe, kamera ve diğer ayrılmış bölgeler içerik veya etkileşim alanını etkileyebilir. Apple, bu tür durumlar için reserved region bilgilerini ve yeni arrangement yaklaşımlarını dokümante ediyor.

Tam ekran bir grafik, video oynatıcı veya yatay düğme grubu kullanıyorsanız önemli kontrollerin menteşe üzerine düşmediğini doğrulayın. İç ekranın arayüz yönü davranışının dış ekranla bire bir aynı olmadığını da hesaba katın.

## Test planı nasıl olmalı?

Xcode 27.1 beta içindeki iPhone Duo simulator ile uygulamayı kapalı, açık, döndürülmüş ve katlanmış durumlarda açın. Her durumda şu sorulara bakın:

- Liste, ayrıntı ve gezinme arasındaki geçişler tutarlı mı?
- Yazı boyutu büyüdüğünde düğmeler kırpılıyor mu?
- Form klavye açıldığında kullanılabilir durumda kalıyor mu?
- Yan menü açık ekranda anlamlı biçimde kullanılıyor mu?
- Fotoğraf, video ve modal pencereler özel ekran şekline uyum sağlıyor mu?

## Sonuç

Katlanabilir cihazlara hazırlanmanın sürdürülebilir yolu, her model için ayrı ekran yazmak değil. **Uyarlanabilir gezinme, size class kullanımı ve fiziksel cihaz/simulator testleri** mevcut uygulamaların Duo dahil farklı ekranlara daha az özel kodla uyum sağlamasını mümkün kılıyor.

---

**Kaynaklar**

- [Apple Developer: iPhone Duo için yeni geliştirme kaynakları](https://developer.apple.com/news/?id=nyuppv9r)
- [Apple Developer: iPhone Duo hazırlık merkezi](https://developer.apple.com/iphone-duo/)
- [Apple Developer: Prepare your app for iPhone Duo](https://developer.apple.com/videos/play/tech-talks/111461/)
- [Apple Developer: Katlanabilir ekranda uyarlanabilir yerleşimler](https://developer.apple.com/videos/play/tech-talks/111463/)
