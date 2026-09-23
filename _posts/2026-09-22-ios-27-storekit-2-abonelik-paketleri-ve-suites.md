---
layout: post
title: "iOS 27 ile StoreKit 2: Abonelik Paketleri, Suites ve Yeni Satın Alma Seçenekleri"
subtitle: "Apple, birden fazla aboneliği veya uygulamayı tek satın alma deneyiminde birleştirmeye yönelik yeni olanaklar duyurdu."
date: 2026-09-22 18:00:00 +0300
author: Hasan Pehlivanlar
thumbnail-img: "/assets/img/2026-09-22-ios27-storekit2-abonelik.svg"
tags: [iOS 27, StoreKit 2, App Store, Abonelik, iOS]
---

Birden fazla iOS uygulaması geliştirenler için abonelik yönetimi giderek daha önemli hale geliyor. Apple, **16 Eylül 2026'da iOS 27 abonelik yeniliklerini** duyurdu ve geliştiricilere **StoreKit 2** kullanımına hazırlık çağrısı yaptı.

Yeni duyurunun merkezinde iki kavram var: **Bundles** ve **Suites**. İkisi de abonelik deneyimini genişletmeyi amaçlıyor, ancak sundukları hakların yapısı farklı.

## Bundles ve Suites arasındaki fark

**Bundles**, birden fazla aboneliğin tek bir App Store satın alımı altında sunulmasını sağlamak için tasarlandı. Apple'ın açıklamasına göre uygun yapılandırmalarda aynı uygulamadaki, aynı geliştiricinin farklı uygulamalarındaki ve hatta farklı geliştiricilerin uygulamalarındaki abonelikler bir araya gelebiliyor.

**Suites** ise tek bir aboneliğin aynı geliştiricinin birden fazla uygulamasında geçerli olması için tasarlandı. Örneğin birbirini tamamlayan araçlar yayımlayan bir geliştirici, uygunluk koşullarını karşılıyorsa ortak abonelik deneyimi planlayabilir.

Burada önemli ayrıntı şu: Bu özellikler, mevcut aboneliklerinizi bir ayar değişikliğiyle otomatik olarak birleştirmiyor. Apple ilgili özellikler için **erişim talebi, uygun yapılandırma ve teknik gereksinimler** öngörüyor.

## StoreKit 2 neden temel ön koşul?

Abonelik satın alma ekranından ibaret değil; satın alma sonucunun doğrulanması, hakların etkinleştirilmesi, geri yükleme ve abonelik durumunun değişmesi de işin parçası. Apple, yeni abonelik seçeneklerine hazırlanmak için uygulamaların StoreKit 2 kullanmasını öneriyor.

Bir uygulamada asıl güvenilir veri, butonun başarı mesajı değil **doğrulanmış işlem ve güncel entitlement durumudur**. Uygulama açılışında hakları tekrar sorgulamak, satın alma sonrası durumu güncellemek ve doğrulanamayan işlemleri premium erişim olarak kabul etmemek gerekir.

Aşağıdaki örnek, mevcut hakları incelemek için temel bir Swift yaklaşımıdır:

~~~swift
import StoreKit

func activeProductIDs() async -> Set<String> {
    var productIDs = Set<String>()

    for await result in Transaction.currentEntitlements {
        guard case .verified(let transaction) = result else {
            continue
        }

        productIDs.insert(transaction.productID)
    }

    return productIDs
}
~~~

Gerçek bir uygulamada bu örneğe transaction güncellemelerini dinleme, iptal ve sona erme durumları, sunucu doğrulaması gerekiyorsa arka uç kontrolü ve kullanıcı arayüzünü eşzamanlama adımları eklenmelidir. Bir paket veya Suite için hangi hakkın hangi uygulamada açılacağı ayrıca modellenmelidir.

## Yeni satın alma seçeneklerinin takvimi

Apple'ın duyurduğu takvime göre **Volume Purchasing 22 Ekim 2026'da** başlayacak; **Group Purchases** özelliğinin ise 2026 kışında kullanıma sunulması planlanıyor. Bu tarihler geleceğe ilişkin planlar olduğundan, üretim tasarımını güncel teknik dokümana göre yürütmek önemli.

App Store Connect tarafında abonelik ürünlerinin incelemeye gönderilmesi, gerekli ekran görüntüleri, fiyat ve deneme koşulları ile gizlilik açıklamaları hâlâ yayın sürecinin temel parçaları.

## Uygulama portföyü olanlar için kontrol listesi

- Mevcut abonelikleri, ürün kimliklerini ve uygulamalar arası hak eşlemelerini belgeleyin.
- StoreKit 2 doğrulama, geri yükleme ve abonelik değişikliği testlerini tamamlayın.
- Bundle veya Suite özelliği için uygunluk ve erişim talebi süreçlerini inceleyin.
- Ücretsiz deneme bitişi, iptal, tekrar abonelik ve yeni cihaza geçiş senaryolarını test edin.
- Satın alma ekranında kullanıcıya gerçekte hangi uygulama ve hizmetlerin açıldığını açıkça gösterin.

## Sonuç

iOS 27 ile abonelik mimarisi tek uygulama ve tek ürün modelinin ötesine geçiyor. Ancak **ürün kataloğunu birleştirmeden önce entitlement modelini doğru kurmak**, yeni satın alma seçeneklerinden yararlanmak için en önemli teknik hazırlıklardan biri.

---

**Kaynaklar**

- [Apple Developer: Get your subscriptions ready for iOS 27](https://developer.apple.com/news/?id=likeohx4)
- [Apple Developer: StoreKit](https://developer.apple.com/storekit/)
- [Apple Developer: App Store Connect sürüm notları](https://developer.apple.com/help/app-store-connect/release-notes/)
