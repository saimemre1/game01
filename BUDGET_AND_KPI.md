# Bütçe ve Başarı Metrikleri (KPI)
## Apartman Oyunu — İlk Oyun Projesi

| Alan | Detay |
|------|-------|
| **Versiyon** | 2.0 |
| **Tarih** | 2026-02-10 |
| **Proje** | Apartman (çalışma adı) |
| **Ekip** | 4 kişi (GD, Sr. Dev, Jr. Dev, Artist) |
| **Geliştirme Süresi** | 18 hafta (16 Şubat → 20 Haziran 2026) |
| **Platform** | Steam (PC) |
| **Motor** | Unity |
| **Hedef Fiyat** | $14.99 (Early Access) → $19.99 (1.0 Release) |

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
| 1 | Unity Asset Store | Çeşitli assetler (UI, efekt, ses vb.) | [assetstore.unity.com](https://assetstore.unity.com/) | $250 | 1 | **$250** |
| 2 | Ek Kaynak | Öngörülemeyen gerekli araçlar için yedek bütçe | — | $100 | 1 | **$100** |
| 3 | Steam Direct | Steam'de oyun yayınlamak için zorunlu ücret (ilk $1,000 gelirden geri alınır) | [partner.steamgames.com](https://partner.steamgames.com/doc/gettingstarted/appfee) | $100 | 1 | **$100** |
| | | | | | **Ara Toplam** | **$450** |

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
| 3 | Capsule art / mağaza görselleri | Profesyonel Steam mağaza görselleri (AI araçlarıyla desteklenebilir) | $100-200 |
| 4 | Trailer prodüksiyon | Oyun içi görüntülerden trailer (AI müzik + montaj) | $50-100 |
| 5 | Hedefli sosyal medya reklamları | Twitter/Reddit/TikTok — küçük ölçekli test kampanyaları | $200-400 |
| 6 | Küçük/orta ölçekli yayıncılara ulaşım | Review key dağıtımı, influencer outreach | $0 (ücretsiz key) |
| | | **Ara Toplam** | **$350-700** |

> **Not:** Sektör standardı, pazarlama bütçesinin toplam proje bütçesinin %25-50'si olmasını önerir. Ancak ilk oyun projesinde organik büyüme (Steam Next Fest, sosyal medya, topluluk oluşturma) öncelikli stratejiler olmalıdır. $0-$2,000 pazarlama harcaması ilk indie oyunlar için tipiktir.

### 1D. Toplam Bütçe Özeti

| Kategori | Minimum | Maksimum |
|----------|---------|----------|
| Tek seferlik araçlar | $450 | $450 |
| Abonelikler | $1,018 | $1,018 |
| Pazarlama | $350 | $700 |
| **TOPLAM** | **$1,818** | **$2,168** |

> **Ekip maaşı dahil değildir.** Bu bütçe yalnızca araç, abonelik ve pazarlama giderlerini kapsar. Ekip üyeleri maaş almıyorsa (tutkuyla/yan proje olarak geliştirme), toplam nakit çıkış budur. Ekip maaşı dahil edilecekse ayrı bir hesaplama yapılmalıdır.

---

## 2. Steam Gelir Modeli

### 2A. Birim Başına Net Gelir Hesabı ($14.99 EA Fiyatıyla)

Bir oyun kopyasının satışından geliştirici eline ne geçer:

| Aşama | Tutar | Açıklama |
|-------|-------|----------|
| Liste fiyatı | $14.99 | Steam'deki gösterge fiyat |
| Bölgesel fiyatlandırma etkisi (~%75) | $11.24 | Düşük fiyatlı bölgeler (TR, BR, AR vb.) ortalamayı düşürür |
| KDV / Satış vergisi çıkışı (~%8-9) | $10.23 | Valve otomatik toplar ve öder |
| Steam komisyonu (~%30) | $7.16 | İlk $10M'a kadar %30 keser |
| İade oranı (~%10-12, EA için) | $6.30 | 2 saat altı oynama ile iade hakkı |
| **Geliştirici net geliri** | **~$6.30** | **Liste fiyatının ~%42'si** |

### 2B. İndirim Dönemlerinde Net Gelir

| İndirim | Efektif Fiyat | Tahmini Net Gelir |
|---------|---------------|-------------------|
| Tam fiyat | $14.99 | ~$6.30 |
| %20 indirim | $11.99 | ~$5.00 |
| %33 indirim | $10.04 | ~$4.20 |
| %50 indirim | $7.49 | ~$3.15 |

### 2C. Yıllık Ağırlıklı Ortalama

İlk yılda satışların tahmini fiyat dağılımı:

| Dönem | Satış Payı | Ortalama Net Gelir |
|-------|------------|-------------------|
| Lansman haftası (tam fiyat) | %30 | ~$6.30 |
| Normal dönem (tam fiyat + küçük indirimler) | %35 | ~$5.50 |
| Sezon indirimleri (%33-50) | %35 | ~$3.70 |
| **Yıllık ağırlıklı ortalama** | | **~$5.00/kopya** |

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

> **Yorum:** Bu rakamlar korkutucu görünebilir. Ancak bu oyunların büyük çoğunluğu pazarlama yapmayan, demo hazırlamayan veya kalitesi düşük projelerdir. Bu projede Steam sayfası lansmantan ~2 ay önce açılır — sektör standardının (6+ ay) altındadır. Bunu telafi eden iki kritik avantaj vardır: **cilalı bir Next Fest demosu** ve **Next Fest ile neredeyse eş zamanlı çıkış**. Steam sayfası ne kadar erken açılırsa wishlist birikimi o kadar yüksek olur, ama kısa sürede kaliteli bir demo + Next Fest katılımı tek başına birçok organik aracı geride bırakabilir. 2 aylık pencerede hedefe ulaşmak zor ama imkansız değildir.

---

## 4. KPI Hedefleri

### Zaman Çizelgesi ve Strateji Notu

Bu projenin pazarlama takvimi sıkışıktır:

| Dönem | Tarih Aralığı | Süre |
|-------|---------------|------|
| Steam sayfası → Next Fest | 15 Nisan → 15 Haziran | ~9 hafta |
| Next Fest → v1.0 çıkış | 15 Haziran → 20 Haziran | 5 gün |
| **Toplam wishlist biriktirme penceresi** | **15 Nisan → 20 Haziran** | **~9.5 hafta** |

**Stratejik durum:** v1.0, Next Fest başladıktan yalnızca 5 gün sonra çıkar. Bu, alışılmadık ama potansiyel olarak avantajlı bir zamanlama yaratır:
- Next Fest boyunca demo oynayanlar, beğenirlerse 5 gün içinde satın alabilir (wishlist → satış dönüşümü çok hızlı olur)
- Dezavantaj: Geleneksel "Next Fest'te wishlist biriktir → haftalarca sonra lansmanda dönüştür" döngüsü uygulanamaz
- Pratik etki: Wishlist rakamları düşük kalır ama doğrudan satış dönüşümü daha yüksek olabilir

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
| **Steam sayfası CTR** | %3-5 | Steamworks | Capsule art ve oyun adının çekiciliği |
| **Steam sayfası ziyaretinden wishlist'e dönüşüm** | %3-6 | Steamworks | Mağaza sayfası kalitesi |

### 4B. Launch KPI'lar (Lansman Haftası — 20 Haziran)

| KPI | Hedef | Ölçüm Yöntemi | Neden Önemli |
|-----|-------|----------------|--------------|
| **İlk hafta satış** | 300-800 kopya | Steamworks | Wishlisten dönüşüm (~%15-20, Next Fest yakınlığı nedeniyle normalden yüksek) + Next Fest doğrudan satış |
| **İlk ay satış** | 700-2,000 kopya | Steamworks | Lansman momentumu + Next Fest kuyruk etkisi |
| **İade oranı** | <%15 | Steamworks | EA için %12-15 normal, üzeriyse alarm |
| **İlk hafta review sayısı** | 5-15 | Steam mağaza sayfası | Erken sosyal kanıt |
| **Rating** | %80+ (Very Positive hedefi) | Steam mağaza sayfası | Kritik eşik: %70 altı = Mixed = ölüm öpücüğü |
| **Eşzamanlı oyuncu zirvesi** | 30-100 | SteamDB | Topluluk büyüklüğünün göstergesi |
| **Medyan oynama süresi** | 3+ saat | Steamworks | İade riski azalır (2 saat üstü), oyuncuyu tutabilme |

### 4C. Post-Launch KPI'lar (İlk 12 Ay)

| KPI | Mütevazi Hedef | Gerçekçi Hedef | İyimser Hedef |
|-----|----------------|----------------|---------------|
| **Toplam satış (12 ay)** | 1,500-3,000 | 3,000-7,000 | 10,000-20,000 |
| **Toplam review sayısı** | 30-60 | 60-200 | 300-700 |
| **Rating** | %75+ (Mostly Positive) | %80+ (Very Positive) | %85+ (Very Positive) |
| **Brüt gelir** | $22K-$45K | $45K-$105K | $150K-$300K |
| **Net gelir (geliştirici payı)** | $7.5K-$15K | $15K-$35K | $50K-$100K |
| **Wishlist biriken (kullanılmamış)** | 2,000+ | 5,000+ | 15,000+ |
| **Haftalık aktif oyuncu** | 100-300 | 300-1,000 | 1,000-5,000 |
| **Medyan oynama süresi** | 5+ saat | 8+ saat | 12+ saat |
| **DLC / güncelleme sonrası satış artışı** | %10-20 | %20-40 | %40-80 |

---

## 5. Başarı Senaryoları

### Senaryo A: Mütevazi Başarı (Medyan Üstü)
> *"Bütçeyi karşıladık, deneyim kazandık, ikinci oyuna yatırım yapabiliriz."*

| Metrik | Değer |
|--------|-------|
| Lansman öncesi wishlist | 1,500-2,500 |
| İlk yıl satış | 1,500-3,000 kopya |
| Net gelir | ~$7,500-$15,000 |
| Review sayısı | 30-60 |
| Rating | %75-79 (Mostly Positive) |
| ROI | **%246-%590** (bütçeye göre) |

**Bu seviyede ne olur:**
- Bütçe fazlasıyla karşılanır
- Steam'de "var olan" bir oyun olur (görünürlük kazanır)
- İkinci oyun için deneyim + portföy + küçük bir bütçe oluşur
- Ekip motivasyonu korunur

### Senaryo B: Gerçekçi Başarı (Üst %25)
> *"Niş bir başarı, küçük ama sadık bir topluluk."*

| Metrik | Değer |
|--------|-------|
| Lansman öncesi wishlist | 2,500-5,000 |
| İlk yıl satış | 3,000-7,000 kopya |
| Net gelir | ~$15,000-$35,000 |
| Review sayısı | 60-200 |
| Rating | %80-85 (Very Positive) |
| ROI | **%590-%1,515** |

**Bu seviyede ne olur:**
- DLC veya devam oyunu ekonomik olarak mantıklı hale gelir
- Küçük bir topluluk oluşur (Discord, Steam Forum)
- Yayıncılar / küçük YouTuber'lar organik olarak oyunu keşfedebilir
- Ekip, oyun geliştirmeyi sürdürülebilir bir aktivite olarak görebilir

### Senaryo C: İyimser Başarı (Üst %5-10)
> *"Nişte tanınırlık, ikinci oyun için ciddi bütçe."*

| Metrik | Değer |
|--------|-------|
| Lansman öncesi wishlist | 5,000-10,000 |
| İlk yıl satış | 10,000-20,000 kopya |
| Net gelir | ~$50,000-$100,000 |
| Review sayısı | 300-700 |
| Rating | %85+ (Very Positive) |
| ROI | **%2,210-%4,510** |

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
| İlk yıl satış | 30,000-50,000+ kopya |
| Net gelir | ~$150,000-$250,000+ |
| Review sayısı | 1,000+ |
| Rating | %90+ (Very Positive / Overwhelmingly Positive) |

> **Not:** Bu senaryo planlanmamalı ama hayal edilebilir. Breakout hit'ler genellikle kalite + zamanlama + şans birleşimidir. İlk oyun için bu senaryoyu "bonus" olarak değerlendirmek sağlıklıdır.

---

## 6. Karşılaştırma Referansları

Bu projeyle benzer ölçekteki ilk oyunların performansları:

| Oyun | Ekip Büyüklüğü | İlk Oyun mu? | Review | Rating | Tahmini Satış | Fiyat |
|------|----------------|-------------|--------|--------|---------------|-------|
| **Unholy Heights** | Küçük (2-3) | Hayır | 1,573 | %90 | ~55K | $3.99 |
| **Monster Care Sim** | Küçük | Evet (EA) | ~549 | %93 | ~19K | $12.99 |
| **Dungeon Inn** | Küçük | Evet (EA) | ~552 | %92 | ~19K | $12.99 |
| **Spirittea** | Küçük (2-3) | Evet | 645 | %85 | ~23K | $19.99 |
| **Bear and Breakfast** | Küçük (~5) | Evet | 3,251 | %90 | ~114K | $19.99 |
| **Minami Lane** | Çok küçük (1-2) | Evet | 5,066 | %97 | ~177K | $4.99 |

> **Gerçekçi beklenti aralığı:** Dungeon Inn / Monster Care Sim seviyesi (500-600 review, ~19K satış) **iyi bir ilk oyun**, Spirittea seviyesi (645 review, ~23K satış) **başarılı** sayılır. Bu projede sıkışık takvim nedeniyle ilk 12 ayda 60-200 review aralığı (3,000-7,000 satış) gerçekçi bir hedef olarak belirlenmiştir. İkinci ve sonraki yıllarda, düzenli güncellemelerle uzun kuyruk satışları bu rakamları artırabilir.

---

## 7. Yatırım Geri Dönüş (ROI) Analizi

### Başabaş Noktası

| Bütçe Senaryosu | Toplam Harcama | Başabaş İçin Gereken Satış | Kopya/Net Gelir |
|-----------------|----------------|---------------------------|-----------------|
| Minimum bütçe | $1,818 | ~364 kopya | $5.00/kopya ile |
| Maksimum bütçe | $2,168 | ~434 kopya | $5.00/kopya ile |

> **Başabaş noktası oldukça düşüktür.** ~400 kopya satışıyla (yaklaşık 12 review'a tekabül eder) tüm nakit giderler karşılanır. Bu, projenin finansal riskinin çok düşük olduğunu gösterir.

### Senaryo Bazlı ROI

| Senaryo | Satış | Net Gelir | ROI |
|---------|-------|-----------|-----|
| Başabaş | ~400 | ~$2,000 | %0 |
| Mütevazi (2K satış) | 2,000 | ~$10,000 | ~%360 |
| Gerçekçi (5K satış) | 5,000 | ~$25,000 | ~%1,050 |
| İyimser (15K satış) | 15,000 | ~$75,000 | ~%3,360 |

---

## 8. Kritik Başarı Faktörleri

### Takvim Kısıtları ve Strateji

Bu projenin takvimi standart indie pazarlama önerilerinden farklıdır:

| Standart Öneri | Bu Projedeki Durum | Strateji |
|----------------|-------------------|----------|
| Steam sayfasını 6+ ay önce aç | ~2 ay önce açılıyor (Nisan ortası) | Kısa sürede yoğun sosyal medya + topluluk çalışması |
| 7,000+ wishlist ile lansmana gir | 2,000-4,000 wishlist hedefleniyor | Next Fest eş zamanlı çıkış ile doğrudan satış dönüşümüne odaklanma |
| Next Fest → birkaç ay sonra çıkış | Next Fest'ten 5 gün sonra çıkış | Demo oynayanların hemen satın alması bekleniyor |
| Uzun süre wishlist biriktir | ~9 hafta pencere | Her haftanın maksimum verimle kullanılması gerekiyor |

### Yapılması Gerekenler (Do)

| # | Aksiyon | Etki | Zamanlama |
|---|---------|------|-----------|
| 1 | Steam sayfasını **Nisan ortasında** aç — trailer + 5 screenshot + açıklama hazır olmalı | İlk günden wishlist biriktirmeye başlama | H9 sonu (~15 Nisan) |
| 2 | Sayfayı açtığı gün **sosyal medyada duyuru** yap (Twitter, Reddit r/indiegaming, TikTok) | İlk hafta wishlist ivmesi | 15 Nisan |
| 3 | Nisan-Haziran arası **haftada 2-3 içerik** paylaş (devlog, GIF, kısa gameplay videosu) | Organik wishlist büyümesi, topluluk oluşturma | Sürekli (9 hafta) |
| 4 | **Steam Next Fest**'e cilalı bir demo ile katıl | En yüksek ROI'li ücretsiz pazarlama + doğrudan satış | 15 Haziran |
| 5 | **Capsule art**'a yatırım yap — mağaza görselleri profesyonel görünmeli | İlk izlenim = tıklama oranı = wishlist | Nisan ortası |
| 6 | v1.0 çıkış gününe özel **lansman indirimi (%10-15)** uygula | Next Fest demo oyuncularının satın alma teşviki | 20 Haziran |
| 7 | Küçük/orta YouTuber ve streamer'lara **review key** gönder | Organik erişim, sosyal kanıt | Lansman haftası |
| 8 | v1.0 sonrası **düzenli güncelleme** yap (2-4 haftada bir) | Uzun kuyruk satışları, topluluk bağlılığı | Çıkış sonrası |

### Yapılmaması Gerekenler (Don't)

| # | Hata | Risk |
|---|------|------|
| 1 | Pazarlamayı lansman haftasına bırakmak | 9 haftalık pencereyi boşa harcamak |
| 2 | Next Fest demo kalitesini ihmal etmek | Bu projenin birincil pazarlama aracı demosudur — düşük kalite demo = düşük satış |
| 3 | İlk yılda %50'den fazla indirim yapmak | Algılanan değeri düşürmek, "bekle indirim gelir" zihniyeti |
| 4 | İlk günden çok fazla özellik sözü vermek | EA'da hayal kırıklığı, negatif review riski |
| 5 | Topluluğu ihmal etmek | Erken destekçileri kaybetmek |
| 6 | Wishlist rakamı düşük diye morali bozmak | 2 aylık pencerede düşük wishlist normaldir — asıl metrik lansman haftası satışıdır |

---

## 9. Özet Karar Tablosu

| Metrik | Minimum Kabul | Birincil Hedef | Uzatmalı Hedef |
|--------|--------------|----------------|----------------|
| **Lansman öncesi wishlist** | 1,500 | 2,500-4,000 | 5,000+ |
| **İlk hafta satış** | 200 | 400-800 | 1,500+ |
| **İlk yıl satış** | 1,500 | 3,000-7,000 | 15,000+ |
| **Review (12 ay)** | 30 | 60-200 | 300+ |
| **Rating** | %75+ | %80+ | %85+ |
| **Net gelir (12 ay)** | $7,500 | $15,000-$35,000 | $75,000+ |
| **Medyan oynama süresi** | 3 saat | 5-8 saat | 10+ saat |
| **Toplam bütçe** | $1,818 | $2,168 | — |
| **Başabaş satış** | ~400 kopya | — | — |

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

*Rapor Sonu — Apartman Projesi, Bütçe ve KPI v2.0*
