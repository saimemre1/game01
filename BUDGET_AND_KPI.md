# Bütçe ve Başarı Metrikleri (KPI)
## Grandma Left Me a Building — İlk Oyun Projesi

### İçindekiler
1. [Bütçe](#1-bütçe)
2. [Steam Gelir Modeli](#2-steam-gelir-modeli)
3. [Sektör Gerçekleri](#3-sektör-gerçekleri--i̇lk-oyun-i̇statistikleri)
4. [KPI Hedefleri](#4-kpi-hedefleri)
5. [Başarı Senaryoları](#5-başarı-senaryoları)
6. [Karşılaştırma Referansları](#6-karşılaştırma-referansları)
7. [Kritik Başarı Faktörleri](#7-kritik-başarı-faktörleri)
8. [Özet Karar Tablosu](#8-özet-karar-tablosu)

| Alan | Detay |
|------|-------|
| **Versiyon** | 2.0 |
| **Tarih** | 2026-02-10 |
| **Proje** | Grandma Left Me a Building |
| **Ekip** | 4 kişi (GD, Sr. Dev, Jr. Dev, Artist) |
| **Geliştirme Süresi** | 18 hafta (16 Şubat → 20 Haziran 2026) |
| **Platform** | Steam (PC) |
| **Motor** | Unity |
| **Hedef Fiyat** | $5.99 |

### Proje Takvimi (Özet)

| Tarih | Milestone |
|-------|-----------|
| 16 Şubat | Geliştirme başlangıcı |
| ~15 Nisan | Steam sayfası açılır |
| 15 Mayıs | Demo Steam'e gönderilir |
| 15 Haziran | Steam Next Fest başlar |
| 20 Haziran | v1.0 tam sürüm çıkışı |

> **Önemli:** Steam sayfası lansmantan ~2 ay önce açılır. Sektör standardı (6+ ay) karşılanamaz, ancak Next Fest ile eş zamanlı çıkış stratejisi bu dezavantajı kısmen telafi eder.

---

## 1. Bütçe

### 1A. Tek Seferlik Araç Maliyetleri

| # | Kalem | Açıklama | Link | Birim Maliyet | Adet | Toplam |
|---|-------|----------|------|---------------|------|--------|
| 1 | Unity Asset Store | Çeşitli assetler (UI, efekt, ses vb.) | [assetstore.unity.com](https://assetstore.unity.com/) | $150 | 1 | **$150** |
| 2 | Ek Kaynak | Öngörülemeyen araçlar + marketing tool'ları için yedek bütçe | — | $150 | 1 | **$150** |
| 3 | Steam Direct | Steam'de oyun yayınlamak için zorunlu ücret (ilk $1,000 gelirden geri alınır) | [partner.steamgames.com](https://partner.steamgames.com/doc/gettingstarted/appfee) | $100 | 1 | **$100** |
| | | | | | **Ara Toplam** | **$400** |

### 1B. Abonelik Maliyetleri

| # | Araç | Açıklama | Link | Aylık Maliyet | Kişi | Süre (ay) | Toplam |
|---|------|----------|------|---------------|------|-----------|--------|
| 1 | Claude Max | Kod yazımında kullanılacak AI aracı | [claude.com/pricing](https://claude.com/pricing) | $100 | 2 | 4 | **$800** |
| 2 | Trello | Task Manager | [trello.com/pricing](https://trello.com/pricing) | $5 | 4 | 4 | **$80** |
| 3 | Rive App | GUI yapımında kullanılacak animasyon aracı | [rive.app/pricing](https://rive.app/pricing) | $9 | 1 | 2 | **$18** |
| 4 | Image-gen AI | Görsel oluşturma (Gemini veya benzeri) | (seçilecek) | $20 | 1 | 3 | **$60** |
| 5 | Eleven Labs AI | Ses üretimi | [elevenlabs.io/pricing](https://elevenlabs.io/pricing) | $20 | 1 | 3 | **$60** |
| | | | | | | **Ara Toplam** | **$1,018** |

### 1C. Pazarlama Bütçesi

| # | Kalem | Açıklama | Tahmini Maliyet |
|---|-------|----------|-----------------|
| 1 | Steam Next Fest | Demo ile katılım — ücretsiz, yüksek ROI | $0 |
| 2 | Sosyal medya içerik üretimi | Devlog, GIF, kısa video (ekip tarafından) | $0 |
| 3 | Capsule art / mağaza görselleri | Ekip içinde üretilecek (inhouse) | $0 |
| 4 | Trailer prodüksiyon | Oyun içi görüntülerden trailer (AI müzik + montaj) | $100 |
| 5 | Hedefli sosyal medya reklamları | Twitter/Reddit/TikTok — kampanyalar | $1,000 |
| 6 | Küçük/orta ölçekli yayıncılara ulaşım | Review key dağıtımı, influencer outreach, hediye/ödeme | $500 |
| | | **Ara Toplam** | **$1,600** |

> **Not:** $0-$2,000 pazarlama harcaması ilk indie oyunlar için tipiktir. Bu bütçenin büyük kısmı sosyal medya reklamlarına ayrılmıştır — performansı düşükse bu kalem azaltılabilir.

### 1D. Toplam Bütçe Özeti

| Kategori | Toplam |
|----------|--------|
| Tek seferlik araçlar | $400 |
| Abonelikler | $1,018 |
| Pazarlama | $1,600 |
| **TOPLAM** | **$3,018** |

> **Ekip maaşları bu dokümana dahil değildir.** Bu bütçe yalnızca araç, abonelik ve pazarlama giderlerini kapsar. Maaşlar ayrı yönetilmektedir.

---

## 2. Steam Gelir Modeli

### 2A. Birim Başına Net Gelir Hesabı ($5.99 Fiyatıyla)

Bir oyun kopyasının satışından geliştirici eline ne geçer:

| Aşama | Tutar | Açıklama |
|-------|-------|----------|
| Liste fiyatı | $5.99 | Steam'deki gösterge fiyat |
| Bölgesel fiyatlandırma etkisi (~%80) | $4.79 | Düşük fiyatlı oyunlarda bölgesel indirim etkisi daha hafiftir |
| KDV / Satış vergisi çıkışı (~%8-9) | $4.36 | Valve otomatik toplar ve öder |
| Steam komisyonu (~%30) | $3.05 | İlk $10M'a kadar %30 keser |
| İade oranı (~%8-10) | $2.75 | Ucuz oyunlarda iade oranı daha düşüktür |
| **Geliştirici net geliri** | **~$2.75** | **Liste fiyatının ~%46'sı** |

> **Not:** Düşük fiyatlı oyunlarda bölgesel fiyatlandırma ve iade oranları genellikle daha uygun seyreder. Ancak bu oranlar tahminidir — gerçek değerler oyunun bölgesel dağılımına ve iade davranışına göre değişir.

### 2B. İndirimli Satışlarda Net Gelir

$5.99 fiyat noktasında indirim dönemleri:

| İndirim | Efektif Fiyat | Tahmini Net Gelir |
|---------|---------------|-------------------|
| Tam fiyat | $5.99 | ~$2.75 |
| %20 indirim | $4.79 | ~$2.20 |
| %33 indirim | $4.01 | ~$1.85 |
| %50 indirim | $2.99 | ~$1.38 |

### 2C. Yıllık Ağırlıklı Ortalama (Tüm Satışlar Dahil)

İlk yılda satışların tahmini fiyat dağılımı — **tüm sonraki hesaplamalarda bu ortalama kullanılır:**

| Dönem | Satış Payı | Ortalama Net Gelir |
|-------|------------|-------------------|
| Lansman haftası (tam fiyat) | %30 | ~$2.75 |
| Normal dönem (tam fiyat + küçük indirimler) | %35 | ~$2.40 |
| Sezon indirimleri (%33-50) | %35 | ~$1.60 |
| **Yıllık ağırlıklı ortalama** | | **~$2.20/kopya** |

> **Not:** Tüm senaryo ve ROI hesapları bu ağırlıklı ortalamayı ($2.20/kopya) baz alır — sadece tam fiyat satışı değil, indirimli dönemleri de kapsar.

---

## 3. Sektör Gerçekleri — İlk Oyun İstatistikleri

Bu metrikleri belirlemeden önce, sektörün gerçeklerini bilmek kritiktir:

| Metrik | Değer | Kaynak |
|--------|-------|--------|
| Steam'de yıllık yeni oyun sayısı (2024) | ~18,324 | How To Market A Game |
| 1,000+ review'a ulaşan oyun oranı | %2.44 (445 oyun) | How To Market A Game |
| 50'den az review alan oyun oranı | %75 | How To Market A Game |
| 100'den az kopya satan oyun oranı (2025) | %47.5 | Game Developers Org |
| Steam Direct ücretini bile karşılayamayan oyun oranı | ~%40 | Game Developers Org |
| Medyan indie oyun ömür boyu geliri | ~$1,200 | VG Insights / Gitnux |
| İlk oyun ortalama brüt geliri | ~$120,000 | VG Insights (aşırı sağa çarpık, medyan çok daha düşük) |
| Top %10 oyunların gelir payı | %89 | Sektör verileri |

> **Yorum:** Bu oyunların büyük çoğunluğu pazarlama yapmayan, demo hazırlamayan veya kalitesi düşük projelerdir. Bu projede Steam sayfası lansmantan ~2 ay önce açılır — sektör standardının (6+ ay) altındadır, bu gerçek bir dezavantajdır. Next Fest demosu ve $5.99 fiyat noktası bu açığı kısmen kapatabilir, ama sihirli bir çözüm değildir. Kısa wishlist penceresi bu projenin en büyük risklerinden biridir.

---

## 4. KPI Hedefleri

### Zaman Çizelgesi ve Strateji Notu

Bu projenin pazarlama takvimi sıkışıktır:

| Dönem | Tarih Aralığı | Süre |
|-------|---------------|------|
| Steam sayfası → Next Fest | 15 Nisan → 15 Haziran | ~9 hafta |
| Next Fest → v1.0 çıkış | 15 Haziran → 20 Haziran | 5 gün |
| **Toplam wishlist biriktirme penceresi** | **15 Nisan → 20 Haziran** | **~9.5 hafta** |

**Stratejik durum:** v1.0, Next Fest başladıktan yalnızca 5 gün sonra çıkar. Bu alışılmadık bir zamanlama:
- **Potansiyel artı:** Demo oynayanlar beğenirlerse 5 gün içinde satın alabilir — wishlist→satış dönüşümü hızlı olur
- **Potansiyel eksi:** Geleneksel "Next Fest'te wishlist biriktir → haftalarca sonra lansmanda dönüştür" döngüsü uygulanamaz. Next Fest'in wishlist biriktirme etkisinden tam yararlanılamaz.
- **Pratik etki:** Wishlist rakamları düşük kalır. Doğrudan satış dönüşümünün bunu ne kadar telafi edeceği belirsizdir.
- $5.99 fiyat noktasında wishlist→satış dönüşüm oranı genellikle daha yüksektir (~%15, $10+ oyunlardaki ~%10'a karşı).

### 4A. Pre-Launch KPI'lar (15 Nisan → 20 Haziran)

| KPI | Hedef | Ölçüm Yöntemi | Neden Önemli |
|-----|-------|----------------|--------------|
| **Steam sayfası açılış zamanı** | ~15 Nisan (lansmantan ~2 ay önce) | Steamworks | Sektör standardının altında ama proje takvimi bunu zorunlu kılıyor |
| **Haftalık wishlist artışı (organik)** | 50-100/hafta | Steamworks dashboard | 9 haftalık pencerede organik büyüme hızı |
| **Lansman öncesi toplam wishlist** | **2,000-4,000** (birincil hedef) | Steamworks dashboard | 2 aylık pencere + Next Fest'in ilk 5 günü ile gerçekçi aralık |
| **Next Fest ilk 5 gün wishlist kazanımı** | 500-2,000 | Steamworks dashboard | Next Fest'in asıl etkisi wishlist değil doğrudan satış olarak yansıyacak |
| **Demo indirme sayısı (Next Fest)** | 500-2,000 | Steamworks | Demo kalitesinin ve Next Fest görünürlüğünün göstergesi |
| **Demo'dan wishlist/satışa dönüşüm** | %10-20 | Steamworks | Demo'nun etkinliği — bu projede wishlist yerine doğrudan satışa dönebilir |
| **Sosyal medya takipçi sayısı** | 300-500 (toplam tüm platformlar) | Twitter/TikTok/Reddit | 2 aylık sürede organik erişim |

### 4B. Launch KPI'lar (Lansman Haftası — 20 Haziran)

| KPI | Hedef | Ölçüm Yöntemi | Neden Önemli |
|-----|-------|----------------|--------------|
| **İlk hafta satış** | 400-1,000 kopya | Steamworks | $5.99 fiyat noktasında dönüşüm oranı ~%15-20 (düşük fiyat + Next Fest yakınlığı) |
| **İlk ay satış** | 1,000-3,000 kopya | Steamworks | Lansman momentumu + Next Fest kuyruk etkisi |
| **İade oranı** | <%10 | Steamworks | $5.99 fiyat noktasında iade oranı düşüktür — %10 üzeri alarm |
| **İlk hafta review sayısı** | 5-15 | Steam mağaza sayfası | Erken sosyal kanıt |
| **Rating** | %80+ (Very Positive hedefi) | Steam mağaza sayfası | Kritik eşik: %70 altı = Mixed = ölüm öpücüğü |
| **Eşzamanlı oyuncu zirvesi** | 30-100 | SteamDB | Topluluk büyüklüğünün göstergesi |
| **Medyan oynama süresi** | 3+ saat | Steamworks | İade riski azalır (2 saat üstü), oyuncuyu tutabilme |

### 4C. Post-Launch KPI'lar (İlk 12 Ay)

| KPI | Mütevazi Hedef | Gerçekçi Hedef | İyimser Hedef |
|-----|----------------|----------------|---------------|
| **Toplam satış (12 ay)** | 2,000-4,000 | 5,000-12,000 | 15,000-30,000 |
| **Toplam review sayısı** | 40-80 | 100-350 | 500-1,000 |
| **Rating** | %75+ (Mostly Positive) | %80+ (Very Positive) | %85+ (Very Positive) |
| **Net gelir (geliştirici payı)** | $4.4K-$8.8K | $11K-$26K | $33K-$66K |
| **Wishlist biriken (kullanılmamış)** | 2,000+ | 5,000+ | 15,000+ |
| **Haftalık aktif oyuncu** | 50-150 | 150-500 | 500-2,000 |
| **Medyan oynama süresi** | 3+ saat | 4+ saat | 6+ saat |
| **DLC / güncelleme sonrası satış artışı** | %10-20 | %20-40 | %40-80 |

---

## 5. Başarı Senaryoları

### Senaryo A: Temel Hedef (Medyan Üstü)
> *"Temel hedefleri tutturduk, deneyim ve knowhow kazandık."*

| Metrik | Değer |
|--------|-------|
| Lansman öncesi wishlist | 1,500-2,500 |
| İlk yıl satış | 2,000-4,000 kopya |
| Net gelir | ~$4,400-$8,800 |
| Review sayısı | 40-80 |
| Rating | %75-79 (Mostly Positive) |

**Bu seviyede ne olur:**
- Temel hedefler tutturulur — oyun Steam'de var ve oynanıyor
- Ekip gerçek bir ürün yayınlama deneyimi kazanır (bu ilk oyun için en değerli çıktı)
- İkinci oyun için portföy, bilgi birikimi ve süreç tecrübesi oluşur
- Finansal olarak beklentilerin altında kalınır ama proje başarısız sayılmaz

### Senaryo B: Gerçekçi Başarı Hedefi (Üst %25)
> *"Asıl hedefimiz — niş bir başarı, küçük ama sadık bir topluluk."*

| Metrik | Değer |
|--------|-------|
| Lansman öncesi wishlist | 2,500-5,000 |
| İlk yıl satış | 5,000-12,000 kopya |
| Net gelir | ~$11,000-$26,400 |
| Review sayısı | 100-350 |
| Rating | %80-85 (Very Positive) |

**Bu seviyede ne olur:**
- Proje finansal olarak kendini karşılar
- DLC veya devam oyunu ekonomik olarak mantıklı hale gelir
- Küçük bir topluluk oluşur (Discord, Steam Forum)
- Yayıncılar / küçük YouTuber'lar organik olarak oyunu keşfedebilir
- Ekip, oyun geliştirmeyi sürdürülebilir bir aktivite olarak görebilir

### Senaryo C: İyimser Başarı (Üst %5-10)
> *"Nişte tanınırlık, ikinci oyun için ciddi bütçe."*

| Metrik | Değer |
|--------|-------|
| Lansman öncesi wishlist | 5,000-10,000 |
| İlk yıl satış | 15,000-30,000 kopya |
| Net gelir | ~$33,000-$66,000 |
| Review sayısı | 500-1,000 |
| Rating | %85+ (Very Positive) |

**Bu seviyede ne olur:**
- Yayıncı teklifleri gelebilir
- Platform portları (Switch, mobil) düşünülebilir
- Tam zamanlı oyun geliştirme bir seçenek olur
- Franchise potansiyeli değerlendirilebilir

### Senaryo D: Hayaldi Gerçek Oldu (Üst %2)
> *"Viral hit — beklentilerin çok üstünde."*

| Metrik | Değer |
|--------|-------|
| Lansman öncesi wishlist | 15,000+ |
| İlk yıl satış | 50,000-100,000+ kopya |
| Net gelir | ~$110,000-$220,000+ |
| Review sayısı | 1,500+ |
| Rating | %90+ (Very Positive / Overwhelmingly Positive) |

> **Not:** Bu senaryo planlanmamalı ama hayal edilebilir. Breakout hit'ler genellikle kalite + zamanlama + şans birleşimidir. İlk oyun için bu senaryoyu "bonus" olarak değerlendirmek sağlıklıdır.

---

## 6. Karşılaştırma Referansları

Bu projeyle benzer ölçek ve fiyat aralığındaki oyunların performansları:

| Oyun | Ekip Büyüklüğü | İlk Oyun mu? | Review | Rating | Tahmini Satış | Fiyat |
|------|----------------|-------------|--------|--------|---------------|-------|
| **Minami Lane** | Çok küçük (1-2) | Evet | 5,066 | %97 | ~177K | $4.99 |
| **Unholy Heights** | Küçük (2-3) | Hayır | 1,573 | %90 | ~55K | $3.99 |
| **Monster Care Sim** | Küçük | Evet (EA) | ~549 | %93 | ~19K | $12.99 |
| **Dungeon Inn** | Küçük | Evet (EA) | ~552 | %92 | ~19K | $12.99 |
| **Spirittea** | Küçük (2-3) | Evet | 645 | %85 | ~23K | $19.99 |
| **Bear and Breakfast** | Küçük (~5) | Evet | 3,251 | %90 | ~114K | $19.99 |

> **Fiyat noktası notu:** Bu projenin $5.99 fiyatı, Minami Lane ($4.99) ve Unholy Heights ($3.99) ile aynı segmentte yer alır. Ancak Minami Lane (~177K satış) bir outlier'dır — o seviyeyi hedef olarak almak yanıltıcı olur. Düşük fiyat, birim geliri azaltır, toplam hacmi artırabilir ama garanti etmez. Gerçekçi karşılaştırma referansı: Monster Care Sim / Dungeon Inn seviyesi (~19K satış).

---

## 7. Kritik Başarı Faktörleri

### Takvim Kısıtları ve Strateji

Bu projenin takvimi standart indie pazarlama önerilerinden farklıdır:

| Standart Öneri | Bu Projedeki Durum | Strateji |
|----------------|-------------------|----------|
| Steam sayfasını 6+ ay önce aç | ~2 ay önce açılıyor (Nisan ortası) | Kısa sürede yoğun sosyal medya + topluluk çalışması |
| 7,000+ wishlist ile lansmana gir | 2,000-4,000 wishlist hedefleniyor | Next Fest eş zamanlı çıkış + düşük fiyatla doğrudan satış dönüşümüne odaklanma |
| Next Fest → birkaç ay sonra çıkış | Next Fest'ten 5 gün sonra çıkış | Demo oynayanların hemen satın alması bekleniyor |
| Uzun süre wishlist biriktir | ~9 hafta pencere | Her haftanın maksimum verimle kullanılması gerekiyor |

### Yapılması Gerekenler (Do)

| # | Aksiyon | Etki | Zamanlama |
|---|---------|------|-----------|
| 1 | **Steam sayfasını Nisan ortasında aç** — trailer + 5 screenshot + açıklama hazır, aynı gün sosyal medyada duyuru | Wishlist biriktirmeye başlama | H9 sonu (~15 Nisan) |
| 2 | Nisan-Haziran arası **haftada 2-3 içerik** paylaş (devlog, GIF, kısa gameplay videosu) | Organik wishlist büyümesi | Sürekli (9 hafta) |
| 3 | **Steam Next Fest**'e cilalı bir demo ile katıl | En yüksek ROI'li ücretsiz pazarlama | 15 Haziran |
| 4 | v1.0 çıkış gününe özel **lansman indirimi (%10-15)** uygula | Demo oyuncularının satın alma teşviki | 20 Haziran |
| 5 | Küçük/orta YouTuber ve streamer'lara **review key** gönder | Organik erişim, sosyal kanıt | Lansman haftası |
| 6 | v1.0 sonrası **düzenli güncelleme** yap (2-4 haftada bir) | Uzun kuyruk satışları | Çıkış sonrası |

### Yapılmaması Gerekenler (Don't)

| # | Hata | Risk |
|---|------|------|
| 1 | Pazarlamayı lansman haftasına bırakmak | 9 haftalık pencereyi boşa harcamak |
| 2 | Next Fest demo kalitesini ihmal etmek | Bu projenin birincil pazarlama aracı demosudur — düşük kalite demo = düşük satış |
| 3 | İlk yılda %50'den fazla indirim yapmak | $5.99 zaten düşük — %50+ indirim algılanan değeri eritir |
| 4 | İlk günden çok fazla özellik sözü vermek | Hayal kırıklığı, negatif review riski |
| 5 | Topluluğu ihmal etmek | Erken destekçileri kaybetmek |
| 6 | Wishlist rakamı düşük diye morali bozmak | 2 aylık pencerede düşük wishlist normaldir — asıl metrik lansman haftası satışıdır |

---

## 8. Özet Karar Tablosu

| Metrik | Minimum Kabul | Birincil Hedef | Uzatmalı Hedef |
|--------|--------------|----------------|----------------|
| **Lansman öncesi wishlist** | 1,500 | 2,500-4,000 | 5,000+ |
| **İlk hafta satış** | 300 | 500-1,000 | 2,000+ |
| **İlk yıl satış** | 2,000 | 5,000-12,000 | 20,000+ |
| **Review (12 ay)** | 40 | 100-350 | 500+ |
| **Rating** | %75+ | %80+ | %85+ |
| **Net gelir (12 ay)** | $4,400 | $11,000-$26,000 | $50,000+ |
| **Medyan oynama süresi** | 2 saat | 3-4 saat | 6+ saat |

---

### Kaynaklar

| Kaynak | Link |
|--------|------|
| How To Market A Game — Wishlist Benchmarks | [howtomarketagame.com](https://howtomarketagame.com/2022/09/26/how-many-wishlists-should-i-have-when-i-launch-my-game/) |
| How To Market A Game — 2024 Analizi | [howtomarketagame.com](https://howtomarketagame.com/2025/01/15/what-the-hell-happened-in-2024/) |
| GameDiscoverCo — Wishlist Dönüşümleri | [newsletter.gamediscover.co](https://newsletter.gamediscover.co/p/the-state-of-steam-wishlist-conversions) |
| GameDiscoverCo — İade Oranları | [newsletter.gamediscover.co](https://newsletter.gamediscover.co/p/steam-refunds-how-many-should-you) |
| VG Insights — 2024 Indie Raporu | [vginsights.com](https://vginsights.com/insights/article/global-indie-games-market-report-2024) |
| Steam Revenue Calculator Blog | [steam-revenue-calculator.com](https://steam-revenue-calculator.com/blog/the-real-talk-on-steams-cut-what-your-game-actually-makes-and-why-its-complicated) |
| Steam Paradox 2025 | [game-developers.org](https://www.game-developers.org/steam-paradox-2025-revenue-volume) |
| Steamworks — App Fee | [partner.steamgames.com](https://partner.steamgames.com/doc/gettingstarted/appfee) |
| Game Oracle — Wishlist to Sales 2025 | [game-oracle.com](https://www.game-oracle.com/blog/wishlist-to-sales-2025) |

---

*Rapor Sonu — Grandma Left Me a Building, Bütçe ve KPI v2.0*
