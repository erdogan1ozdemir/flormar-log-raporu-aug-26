# Flormar | Sunucu Log Analizi · Temmuz - Ağustos 2026

www.flormar.com.tr erişim kayıtlarının 30 günlük analizi. Kullanıcı, mobil uygulama, arama motoru, AI botu ve sentetik izleme katmanları ayrıştırılmış; AI bot sayıları IP doğrulamasından geçirilmiştir.

**Rapor:** [index.html](index.html) · GitHub Pages açıksa: https://erdogan1ozdemir.github.io/flormar-log-raporu-aug-26/

## Kapsam

| | |
|---|---|
| Alan adı | www.flormar.com.tr (alt alan adları kapsam dışı) |
| Dönem | 7 Tem - 5 Ağu 2026 (30 gün, ilk ve son gün kısmi) |
| Ham kayıt | 43.795.526 satır |
| Değerlendirilen istek | 17.341.122 |
| Gönderilen veri | 370.1 GB |

## Rapor akışı

| # | Bölüm | Kapsam |
|---|---|---|
| 01 | Özet | Altı göstergeli durum tablosu, dönemin öne çıkanları, yöntem notu |
| 02 | Trafik kompozisyonu | Sekiz katman; sayfa tipi ile katman kesişimi |
| 03 | Zaman analizi | Katman seçmeli saatlik ve günlük grafik; 22:00 uygulama zirvesi |
| 04 | Adres ve 404 kümesi | 70 adres ve 45 farklı 404 hedefi; katman kırılımlı, filtrelenebilir tablo |
| 05 | Bot kümeleri | 30 bot ailesi; aile seçildiğinde sayfa tipi, yanıt kodu, adres ve saatlik seyir |
| 06 | AI botları | IP doğrulamalı hacim tablosu, günlük seyir, tarama engelleri, yönerge dosyaları |
| 07 | AI kaynaklı trafik | ChatGPT kaynaklı ziyaretler, giriş sayfaları, Google ile kıyas |
| 08 | Sayfa tipi performansı | Sayfa tipi bazında yanıt süresi |
| 09 | Sentetik trafik ve güvenlik | Üç sentetik küme, kimlik taklidi taraması |
| 10 | Öncelikler | Öncelik 1, Öncelik 2 ve takip edilebilir maddeler |
| 11 | Yöntem ve sözlük | Veri kaynakları, sınıflandırma tanımları, terim sözlüğü |

## Ana bulgular

- Trafiğin **%36.8**'i mobil uygulamadan gelmektedir; uygulama isteklerinin %84.4'ü servis ve API çağrısıdır.
- 404 oranı **%13.80**; hacmin %88'i dört adreste toplanmaktadır.
- Doğrulanmış AI bot isteği **63.698** (trafiğin %0.37'si). OpenAI ailesinin payı %62.3.
- Mobil uygulama trafiği **22:00**'de saatlik ortalamanın 3.7 katına çıkmaktadır.
- Amazonbot **%38.0**, YouBot **%31.1** oranında yönlendirmeye takılmaktadır.
- Bingbot tarama bütçesinin **%26.9**'unu içerik taşımayan tek bir servis adresine harcamaktadır.
- **llms.txt** dönem boyunca hiçbir AI botu tarafından çekilmemiştir.
- Trafiğin **%13.8**'i sentetik izleme kaynaklıdır.

## Veri kaynakları

| Kaynak | Kapsam |
|---|---|
| Sunucu erişim kayıtları | Yanıt süresi ve gerçek istemci IP alanını taşıyan tekil kayıt biçimi |
| OpenAI resmi crawler IP listeleri | gptbot, searchbot, chatgpt-user |
| Google resmi crawler IP listeleri | googlebot, special-crawlers, user-triggered-fetchers |
| Microsoft ve Perplexity resmi IP listeleri | bingbot, perplexitybot |
| Ters DNS doğrulaması | Common Crawl, You.com, Anthropic, barındırma sağlayıcıları |

## Teknik not

`index.html` tek dosyadır: CSS, JavaScript, veri seti ve logolar dosyanın içine gömülüdür. Dış bağımlılık yalnızca Google Fonts (Bricolage Grotesque, Outfit) üzerindendir; font yüklenemediğinde sistem yazı tipine düşer.

## Tasarım

Rapor iskeleti Inbound rapor şablonuna dayanır; palet ve logo Flormar marka kimliğinden alınmıştır (rose `#E45A80`, plum `#2A1B22`).
