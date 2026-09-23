---
layout: post
title: ".NET 11 RC1 Yayımlandı: C# 15, ASP.NET Core ve MAUI Geliştiricileri İçin Notlar"
subtitle: "Microsoft'un 8 Eylül 2026 sürümü, yeni .NET sürümünü kararlı yayına bir adım daha yaklaştırırken geliştirme ve test için güncel bir temel sunuyor."
date: 2026-09-23 18:00:00 +0300
author: Hasan Pehlivanlar
thumbnail-img: "/assets/img/2026-09-23-dotnet11-rc1-csharp15.svg"
tags: [.NET 11, C# 15, ASP.NET Core, Blazor, MAUI]
---

Microsoft, **8 Eylül 2026'da .NET 11 Release Candidate 1'i (RC1) yayımladı.** Bu sürüm runtime ve SDK'nın yanında C#, ASP.NET Core, Blazor, .NET MAUI, NuGet, MSBuild ve Windows Forms gibi geniş bir ekosistemdeki iyileştirmeleri bir araya getiriyor.

RC1, genel kullanıma sunulmuş son sürüm değil. Bununla birlikte Microsoft'un **go-live destek kapsamına** aldığı ilk sürüm adayı olması, önizleme sürümlerinden farklı bir güvence sağlıyor. Yine de mevcut sistemleri yükseltmeden önce bağımlılık uyumluluğunu ve performansı ölçmek gerekiyor.

## C# 15 ve JSON modelleri

C# 15 geliştirme gündeminde **union türleri** ve **kapalı tür hiyerarşileri** dikkat çekiyor. Microsoft, 10 Eylül'de bu yapıların System.Text.Json ile ASP.NET Core Minimal API, MVC, SignalR, Blazor ve OpenAPI senaryolarında nasıl kullanılacağını ayrıca ele aldı.

Bu yaklaşım özellikle bir API'nin birden fazla, fakat önceden tanımlı sonuç tipi döndürdüğü durumlarda önemli. Örneğin başarılı sonuç, doğrulama hatası ve iş kuralı hatası gibi yanıtları gevşek nesneler yerine açık türlerle ifade etmek, istemci ile sunucu arasındaki sözleşmeyi daha görünür hale getirebilir.

Ancak yeni dil özellikleri için üretim kararını yalnızca sözdizimi örneklerine bakarak vermemek gerekiyor. JSON serileştirme, OpenAPI şeması, istemci kodu üretimi ve mevcut middleware davranışı birlikte test edilmeli.

## ASP.NET Core ve Blazor tarafında izlenecekler

.NET 11 RC1 duyurusunda ASP.NET Core ve Blazor güncellemeleri de yer alıyor. Özellikle API ve Blazor uygulamalarını aynı çözümde geliştiren ekipler için yükseltme testlerini iki ayrı başlıkta yürütmek yararlı:

1. **API uyumluluğu:** JSON giriş-çıkış modelleri, authentication, authorization, HTTP istemcileri ve OpenAPI dokümanları.
2. **Arayüz uyumluluğu:** Blazor bileşenlerinin yaşam döngüsü, form doğrulama, render davranışı ve JavaScript etkileşimleri.

Yalnızca derleyici hatalarının bitmiş olması regresyon testlerinin tamamlandığı anlamına gelmez.

## .NET MAUI ve mobil uygulamalar

.NET 11 geliştirme döngüsünde MAUI için CoreCLR geçişi önemli teknik başlıklardan biri oldu. Mobil tarafta yeni runtime veya SDK sürümünü denemeden önce iOS ve Android hedeflerinin tamamını, üçüncü taraf paketleri ve fiziksel cihaz testlerini kontrol etmek gerekiyor.

Mevcut bir uygulama için ayrı yükseltme dalı açmak, aynı işlevin eski ve yeni .NET sürümündeki sonuçlarını karşılaştırmayı kolaylaştırır.

## Deneme ortamında ilk adımlar

.NET 11 RC1 SDK'sı yüklendikten sonra test amaçlı ayrı bir proje açabilirsiniz:

~~~bash
dotnet --list-sdks
dotnet new webapi --framework net11.0 -o Net11Deneme
cd Net11Deneme
dotnet restore
dotnet build
dotnet test
~~~

Son komutun anlamlı bir regresyon kontrolü sağlayabilmesi için çözümde test projelerinizin bulunması gerekir. Üretim projelerinde önce mevcut testleri yeni hedef çerçeveyle çalıştırın; sonra performans ölçümlerini karşılaştırın.

## Performans ve yayın takvimi

Microsoft, 14 Eylül'de yayımladığı teknik yazıda .NET 11'deki yüzlerce performans iyileştirmesini ayrıntılandırdı. Bu sonuçlar kendi uygulamanızdaki hızlanmanın garantisi değil; HTTP, JSON, veri erişimi ve tahsisat gibi kritik yollarınızı benchmark ile ölçmeniz gerekir.

.NET Conf 2026'nın **10–12 Kasım** tarihleri için planlandığı ve .NET 11 genel sürümünün bu etkinlikte tanıtılmasının beklendiği duyuruldu.

## Sonuç

.NET 11 RC1, yeni runtime ve dil özelliklerini kontrollü biçimde denemek için somut bir aşama. Kurumsal projelerde geçiş kararını **derleme uyumluluğu, test sonuçları ve üretim performansı** birlikte belirlemeli.

---

**Kaynaklar**

- [Microsoft .NET Blog: Announcing .NET 11 Release Candidate 1](https://devblogs.microsoft.com/dotnet/dotnet-11-rc-1/)
- [Microsoft .NET Blog: Performance Improvements in .NET 11](https://devblogs.microsoft.com/dotnet/performance-improvements-in-net-11/)
- [Microsoft .NET Blog: C# unions and closed hierarchies in ASP.NET Core](https://devblogs.microsoft.com/dotnet/)
- [Microsoft: .NET 11 indirme ve sürüm bilgileri](https://dotnet.microsoft.com/en-us/download/dotnet/11.0)
