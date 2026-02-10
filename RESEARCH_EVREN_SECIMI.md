# Evren Seçimi Araştırma Raporu
## Apartman Oyunu — Gerçekçi İnsan Evreni mi, Fantezi Canavar Evreni mi?

| Alan | Detay |
|------|-------|
| **Rapor Versiyonu** | 1.0 |
| **Tarih** | 2026-02-09 |
| **Proje** | Apartman (çalışma adı) |
| **Hazırlayan** | Proje Ekibi |
| **Durum** | Taslak — Karar bekleniyor |

---

## Araştırma Sorusu

> "Apartman yönetim simülasyonu oyunumuz gerçekçi bir insan evreninde mi yoksa fantezi/canavar evreninde mi geçmeli?"

Bu karar şu alanları doğrudan etkiler:
- **Pazar konumlandırması** — Rakiplerden nasıl ayrışacağız?
- **Sanat üretim maliyeti** — Referans mı kullanacağız, sıfırdan mı tasarlayacağız?
- **Hedef kitle** — Kim bu oyunu satın alacak?
- **Ticari potansiyel** — Hangi tema daha çok satış getirir?

---

## 1. Veri Kaynakları ve Güvenilirlik

Bu raporun dayandığı tüm veri kaynakları ve güvenilirlik seviyeleri:

| Kaynak | Tür | Güvenilirlik | Erişim | Not |
|--------|-----|-------------|--------|-----|
| [Steam Store](https://store.steampowered.com/) | Resmi mağaza verileri | ⭐⭐⭐ Yüksek | Ücretsiz | Review sayısı ve oranı en güvenilir public veri |
| [SteamDB](https://steamdb.info/) | Oyuncu sayıları, fiyat geçmişi | ⭐⭐⭐ Yüksek | Ücretsiz | Steam API'den direkt çeker, gerçek zamanlı |
| [VG Insights](https://vginsights.com/) | Satış tahmini, gelir analizi | ⭐⭐⭐ Yüksek | Ücretli (kısıtlı ücretsiz) | Boxleiter yöntemi + iç veritabanı |
| [SteamSpy](https://steamspy.com/) | Sahip sayısı tahminleri | ⭐⭐ Orta | Ücretsiz | 2018 gizlilik değişikliğinden sonra doğruluk düştü |
| [Gamalytic](https://gamalytic.com/) | Satış/gelir tahmini | ⭐⭐⭐ Yüksek-Orta | Ücretli (kısıtlı ücretsiz) | Review ratio derinlemesine analizi var |
| [Steam250](https://steam250.com/) | Puan bazlı sıralama | ⭐⭐⭐ Yüksek | Ücretsiz | Ranking ve karşılaştırma için ideal |
| [How To Market A Game](https://howtomarketagame.com/) | Endüstri analizi | ⭐⭐⭐ Yüksek | Ücretsiz blog | Chris Zukowski'nin veriye dayalı analizleri |
| [Gamedeveloper.com](https://www.gamedeveloper.com/) | Endüstri makaleleri | ⭐⭐⭐ Yüksek | Ücretsiz | GDC bağlantılı, uzman yazarlar |
| Reddit (r/tycoon, r/BaseBuildingGames) | Oyuncu tartışmaları | ⭐⭐ Orta | Ücretsiz | Anekdotal ama oyuncu hissiyatını yansıtır |
| Wikipedia / Basın | Satış rakamları | ⭐⭐ Orta | Ücretsiz | Doğrulanmış rakamlar güvenilir, tahminler değişken |

### Satış Tahmini Yöntemi

Bu raporda satış tahminleri için **Boxleiter Yöntemi** kullanılmıştır:

> **Steam Review Sayısı × 30-50 = Tahmini Toplam Satış**

- Bu çarpan türe, fiyata ve görünürlüğe göre değişir ([Gamalytic detaylı analizi](https://gamalytic.com/blog/a-deep-dive-into-the-steam-review-ratio))
- Niş oyunlarda çarpan daha düşük (~20-30), viral oyunlarda daha yüksek (~50-70) olabilir
- Bu raporda **×35 orta tahmin** kullanılmıştır (aksi belirtilmediği sürece)

---

## 2. Pazar Haritası — Rakip Analizi

### 2A. Gerçekçi Tema — Apartman / Bina Yönetim Oyunları

| Oyun | Review | Rating | Fiyat | Tahmini Satış | Tema Detayı | Steam Linki |
|------|--------|--------|-------|---------------|-------------|-------------|
| **The Tenants** | 7,377 | %79 Mostly Positive | $19.99 | ~258K | Kiracı yönetimi, daire renovasyonu | [Steam](https://store.steampowered.com/app/1009560/The_Tenants/) |
| **Project Highrise** | 4,661 | %85 Very Positive | $19.99 | ~163K | Gökdelen yönetimi (SimTower varisi) | [Steam](https://store.steampowered.com/app/423580/Project_Highrise/) |
| **News Tower** | 3,821 | %94 Overwhelmingly Positive | $24.99 | ~134K | Gazete binası + SimTower melez | [Steam](https://store.steampowered.com/app/1649950/News_Tower/) |
| **Landlord's Super** | 1,434 | %82 Very Positive | $19.99 | ~50K | 1980'ler İngiltere, mülk tamiri | [Steam](https://store.steampowered.com/app/1127840/Landlords_Super/) |
| **Small Spaces** | 824 | %89 Very Positive | EA | ~29K | Apartman iç tasarım | [Steam](https://store.steampowered.com/app/3151380/Small_Spaces/) |
| **Mad Tower Tycoon** | 435 | %77 Mostly Positive | $14.99 | ~15K | Gökdelen inşa | [Steam](https://store.steampowered.com/app/910880/Mad_Tower_Tycoon/) |
| **Constructor Plus** | 424 | %89 Very Positive | $14.99 | ~15K | Mülk inşa + rakip yarışı | [Steam](https://store.steampowered.com/app/898800/Constructor_Plus/) |
| **Landlord Simulator** | 10 | %20 Mostly Negative | $4.99 | <1K | Temel kiracı yönetimi (başarısız) | [Steam](https://store.steampowered.com/app/803310/Landlord_Simulator/) |

**Distopik Varyant:**

| Oyun | Review | Rating | Fiyat | Tahmini Satış | Tema Detayı | Steam Linki |
|------|--------|--------|-------|---------------|-------------|-------------|
| **Beholder** | 2,995 | %81 Very Positive | $9.99 | ~105K | Totaliter rejimde apartman gözetimi | [Steam](https://store.steampowered.com/app/475550/Beholder/) |
| **Beholder 2** | 1,015 | %82 Very Positive | $14.99 | ~36K | Devlet binası gözetimi | [Steam](https://store.steampowered.com/app/761620/Beholder_2/) |
| **Beholder 3** | 406 | %68 Mixed | $14.99 | ~14K | Seri devamı (düşüş) | [Steam](https://store.steampowered.com/app/1570070/Beholder_3/) |

### 2B. Fantezi / Canavar Tema — Yönetim Oyunları

| Oyun | Review | Rating | Fiyat | Tahmini Satış | Tema Detayı | Steam Linki |
|------|--------|--------|-------|---------------|-------------|-------------|
| **Lobotomy Corporation** | 46,349 | %94 Overwhelmingly Positive | $24.99 | ~1.6M | SCP-tarzı canavar yönetim tesisi | [Steam](https://store.steampowered.com/app/568220/Lobotomy_Corporation__Monster_Management_Simulation/) |
| **Against the Storm** | 17,915 | %95 Overwhelmingly Positive | $29.99 | ~627K | Fantezi şehir yönetimi (kunduz, kertenkele, insan) | [Steam](https://store.steampowered.com/app/1336490/Against_the_Storm/) |
| **Unholy Heights** | 1,573 | %90 Very Positive | $3.99 | ~55K | Şeytan'ın canavar apartmanı (**en yakın rakip**) | [Steam](https://store.steampowered.com/app/249330/Unholy_Heights/) |
| **War for the Overworld** | 6,265 | %85 Very Positive | $29.99 | ~219K | Dungeon Keeper varisi | [Steam](https://store.steampowered.com/app/230190/War_for_the_Overworld/) |
| **Dungeon Inn** | ~500+ | %92 Very Positive | EA | ~18K | Zindan ağzında han yönetimi | [Steam](https://store.steampowered.com/app/2552310/Dungeon_Inn/) |
| **Bloody Hell Hotel** | — | — (henüz çıkmadı) | TBD | — | Vampir otel yönetimi | [Steam](https://store.steampowered.com/app/2055770/Bloody_Hell_Hotel/) |
| **Drosoph Hotel** | az | — | $7.99 | <1K | Korku oteli yönetimi (terk edilmiş) | [Steam](https://store.steampowered.com/app/717020/Drosoph_Hotel/) |

### 2C. Tema Komedisiyle Öne Çıkan Yönetim Oyunları (Referans)

| Oyun | Review | Rating | Tahmini Satış | Tema Detayı | Steam Linki |
|------|--------|--------|---------------|-------------|-------------|
| **Two Point Hospital** | 30,000+ | %90 Very Positive | ~1M+ | Komik kurgusal hastalıklar + hastane | [Steam](https://store.steampowered.com/app/535930/Two_Point_Hospital/) |
| **Prison Architect** | 40,000+ | %90 Very Positive | ~4M+ | Stilize hapishane yönetimi | [Steam](https://store.steampowered.com/app/233450/Prison_Architect/) |

---

## 3. Tema Bazlı Karşılaştırma

### Sayısal Karşılaştırma

| Metrik | Gerçekçi Tema (8 oyun) | Fantezi/Canavar Tema (6 oyun) |
|--------|------------------------|-------------------------------|
| **Toplam oyun sayısı** | 8+ (doygun) | 6 (az, özellikle apartman nişinde 1) |
| **Ortalama review sayısı** | ~2,385 | ~12,100 |
| **Ortalama rating** | %78 | %91 |
| **En yüksek tahmini satış** | ~258K (The Tenants) | ~1.6M (Lobotomy Corp) |
| **En yüksek tahmini gelir** | ~$5M (The Tenants) | ~$49M (Lobotomy Corp) |

### Pazar Doygunluğu

```
Gerçekçi Apartman/Bina Yönetimi:
████████████████████ 8+ oyun — DOYGUN

Fantezi Bina/Apartman Yönetimi:
██                   1 oyun (Unholy Heights, 2013) — NEREDEYSE BOŞ

Fantezi Otel/Han Yönetimi:
██████               3-4 oyun — ORTA

Canavar Yönetimi (genel):
████████             3-4 oyun — ORTA
```

### Kritik Bulgu

**"Canavar apartman yönetimi" nişinde yalnızca 1 oyun var: Unholy Heights (2013).** Bu oyun $3.99 fiyat noktasında, ~5 saatlik bir oyun ve %90 pozitif review'a sahip. Modern üretim değerleriyle bu nişe giren büyük bir rakip bulunmuyor. Bu, klasik bir **mavi okyanus** fırsatıdır.

---

## 4. Vaka Çalışmaları

### Vaka 1: Project Highrise — Gerçekçi Temanın Sınırları

| Alan | Detay |
|------|-------|
| **Oyun** | Project Highrise |
| **Tema** | Gerçekçi modern gökdelen yönetimi |
| **Satış** | ~200K-500K kopya ([SteamSpy](https://steamspy.com/app/423580)) |
| **Rating** | %85 (Very Positive), Metacritic 73 |
| **DLC** | 5 genişleme paketi (Las Vegas, Miami, Tokyo, London, Berlin) |

**Ne oldu:** SimTower'ın ruhani varisi olarak çıktı. Gaming Trend "SimTower'ın olması gereken oyun" dedi ve 90/100 verdi. Solid bir oyundu ama "breakout hit" olamadı.

**Tema etkisi:** Gerçekçi tema oyuna güvenilirlik kattı ama **Steam mağazasında görünürlüğünü sınırladı**. "Bir gökdelen yönet" pitch'i doğru kitleyi çekti ama viral büyüme yaratamadı. 5 DLC çıkarmak zorunda kalmaları, organik büyümenin sınırlı olduğunu gösteriyor.

**Ders:** Gerçekçi tema, niş bir kitleyi güvenilir şekilde çeker ama tavan düşüktür.

---

### Vaka 2: Two Point Hospital — Absürd Temanın Ticari Gücü

| Alan | Detay |
|------|-------|
| **Oyun** | Two Point Hospital |
| **Tema** | Komik/karikatür — kurgusal absürd hastalıklar |
| **Satış** | ~1M kopya PC, 5M+ toplam oyuncu ([Wikipedia](https://en.wikipedia.org/wiki/Two_Point_Hospital)) |
| **Gelir** | ~$9.4M brüt Steam geliri ([Steam Revenue Calculator](https://steam-revenue-calculator.com/app/535930/two-point-hospital)) |
| **Devam** | Two Point Campus — 2 haftada 1M oyuncu |

**Ne oldu:** Theme Hospital'ın ruhani varisi. "Ampul kafalılık" (lightbulb-headed patients), "8-bitten" (pikselleşmiş hastalar), "kübizm" gibi absürd hastalıklarla doluydu. Oyuncular ve basın bu absürdlüğe bayıldı.

**Tema etkisi:** Gerçekçi bir hastane simülasyonu olsaydı, bu kadar konuşulmazdı. **Absürd tema 3 kritik avantaj sağladı:**
1. **Viral paylaşılabilirlik** — "Bak hastamın kafası ampul!" içerikleri sosyal medyada yayıldı
2. **Sınırsız tasarım alanı** — Gerçek hastalıklarla sınırlı kalmadılar
3. **Marka kimliği** — Anında tanınabilir, benzersiz bir görünüm

**Ders:** Yönetim simülasyonlarında komik/absürd tema, gerçekçi temaya kıyasla çok daha yüksek ticari tavan sunar.

**Kaynak:** [Two Point Hospital — Wikipedia](https://en.wikipedia.org/wiki/Two_Point_Hospital)

---

### Vaka 3: Lobotomy Corporation — Canavar Yönetiminin $49M Potansiyeli

| Alan | Detay |
|------|-------|
| **Oyun** | Lobotomy Corporation |
| **Tema** | SCP-tarzı canavar yönetim tesisi |
| **Satış** | 1M+ kopya (Ocak 2023 itibarıyla) |
| **Gelir** | ~$49.1M brüt tahmin ([Steam Revenue Calculator](https://steam-revenue-calculator.com/app/568220/lobotomy-corporation-or-monster-management-simulation)) |
| **Franchise** | Library of Ruina, Limbus Company (franchise doğurdu) |
| **Rating** | %94 Overwhelmingly Positive |

**Ne oldu:** Güney Koreli indie stüdyo Project Moon'un ilk oyunu. SCP Foundation ve Cabin in the Woods'tan ilham alarak "abnormality" adı verilen canavarları yönettiğiniz bir tesis simülasyonu yarattı. Oyuncular canavarları "içerir", çalışanları yönetir, enerji toplar.

**Tema etkisi:** **Canavar teması bu oyunun var olma sebebiydi.** Gerçekçi bir tema ile bu oyun yapılamazdı. Canavar çeşitliliği:
- Sınırsız yaratık tasarımı → sürekli yeni içerik
- Her canavarın benzersiz hikayesi → lore derinliği
- Tehlike ve gizem → oyuncu bağlılığı

**Ders:** "Canavar yönetimi" konsepti tek başına $49M gelir ve bir franchise yaratabilir — **doğru uygulandığında**.

**Kaynak:** [Lobotomy Corporation — Steam](https://store.steampowered.com/app/568220/Lobotomy_Corporation__Monster_Management_Simulation/)

---

### Vaka 4: Unholy Heights — Direkt Rakip, Büyük Boşluk

| Alan | Detay |
|------|-------|
| **Oyun** | Unholy Heights |
| **Tema** | Şeytan bir apartman yöneticisi, kiracılar canavar |
| **Satış** | ~55K kopya (tahmin) |
| **Fiyat** | $3.99 (sık indirim: $1.99) |
| **Rating** | %90 Very Positive |
| **Süre** | ~5 saat |
| **Çıkış** | 2013 |

**Ne oldu:** Japon geliştirici Petit Depotto'nun oyunu. Şeytan bir apartman binasını canavar-only konut olarak işletir. 20+ canavar türü, kira toplama, mobilya satın alma, ve binaya saldıran kahramanlara karşı kiracılarınızı savunma.

**Tema etkisi:** "Canavar apartman" konsepti eleştirmenler tarafından "harika bir temel konsept" olarak övüldü. %90 pozitif review, bu konseptin oyuncuları memnun ettiğini kanıtlar. **Ancak:**
- Çok düşük fiyat noktası ($3.99) → gelir tavanı düşük
- Kısa oyun süresi (5 saat) → derinlik eksikliği
- 2013 yapımı → modern üretim değerleri yok
- Tower defense melez → saf yönetim sim değil

**Ders:** "Canavar apartman yönetimi" konsepti %90 review ile kanıtlanmış bir konsepttir, ama **hiç kimse bunu modern, derin bir yönetim simülasyonu olarak yapmamıştır.** Bu niş 2013'ten beri neredeyse dokunulmamış durumda.

**Kaynak:** [Unholy Heights — Steam](https://store.steampowered.com/app/249330/Unholy_Heights/)

---

### Vaka 5: Against the Storm — Benzersiz Fantezi Açının Etkisi

| Alan | Detay |
|------|-------|
| **Oyun** | Against the Storm |
| **Tema** | Fantezi şehir yönetimi — sürekli yağmur dünyası, kunduzlar + kertenkeleler + insanlar |
| **Satış** | 1M+ kopya Steam'de ([VGChartz](https://www.vgchartz.com/article/460494/against-the-storm-sales-top-1-million-units-on-steam/)) |
| **Rating** | %95 Overwhelmingly Positive |
| **Ödüller** | Taipei Game Show Best Design 2024, DICE nomination |

**Ne oldu:** Klasik şehir yönetimi + roguelite döngüsünü birleştirdi. "Sürekli yağmur yağan bir dünyada farklı ırkların (kunduz, kertenkele, insan) yerleşim yerlerini kur" pitch'iyle çıktı.

**Tema etkisi:** Gerçekçi bir şehir yönetimi olsaydı, Cities: Skylines'ın gölgesinde kaybolurdu. **Fantezi tema 2 kritik avantaj sağladı:**
1. **Rakiplerden tam ayrışma** — "Kunduz+kertenkele şehir yönetimi" diye başka oyun yok
2. **Mekanik özgürlük** — Farklı ırkların farklı ihtiyaçları = daha zengin gameplay

**Ders:** Yönetim simülasyonlarında benzersiz bir fantezi açısı, kalabalık bir türde bile 1M+ satışa ulaşabilir. Anahtar: "Generic fantezi" değil, **spesifik ve alışılmadık fantezi**.

**Kaynak:** [Against the Storm — Steam](https://store.steampowered.com/app/1336490/Against_the_Storm/)

---

## 5. Pazar Trendleri (2024-2026)

### Simülasyon Pazarı Büyüklüğü

| Yıl | Pazar Değeri | Kaynak |
|-----|-------------|--------|
| 2024 | $3.53 milyar | [Verified Market Research](https://www.verifiedmarketresearch.com/product/simulation-game-market/) |
| 2032 (tahmin) | $26.18 milyar | [Global Growth Insights](https://www.globalgrowthinsights.com/market-reports/simulation-game-market-102402) |
| CAGR | ~%28-34 | Kaynaklara göre değişir |

### İndie Oyun Pazarı

| Yıl | Pazar Değeri | Kaynak |
|-----|-------------|--------|
| 2025 | $4.85 milyar | [Mordor Intelligence](https://www.mordorintelligence.com/industry-reports/indie-game-market) |
| 2031 (tahmin) | $10.83 milyar | [Mordor Intelligence](https://www.mordorintelligence.com/industry-reports/indie-game-market) |
| CAGR | %14.32 | — |

### 2025-2026 Öne Çıkan Trendler

1. **Simülasyon, Steam'de #2 en popüler tür** (2025) — Narrative/Horror'dan sonra, 1000+ review'a ulaşan oyunlar arasında
   - Kaynak: [How To Market A Game — 2025 Analizi](https://howtomarketagame.com/2026/01/27/what-the-hell-happened-in-2025/)

2. **İndie oyunlar Steam gelirinin %48'ini oluşturuyor** (2024 ilk 9 ay) — Tarihte ilk kez AA/AAA gelir seviyesine yaklaştı
   - Kaynak: [Game World Observer](https://gameworldobserver.com/2024/10/16/indie-games-revenue-steam-vs-aaa-titles-vg-insights)

3. **"Cozy management" yükselen kategori** — Başarılı "cozy" oyunların çoğunluğu aslında management sim
   - Kaynak: [How To Market A Game — Crafty Buildy Guide](https://howtomarketagame.com/2025/07/02/crafty-buildy-strategy-simulation-buyers-guide/)

4. **"İş simülasyonu" trendi** — Supermarket Simulator ve Schedule I öncülüğünde, "bir işi simüle et" oyunları patlama yaşıyor
   - Kaynak: [How To Market A Game — 2025](https://howtomarketagame.com/2026/01/27/what-the-hell-happened-in-2025/)

5. **Steam'de yılda 14,000+ yeni oyun** — Farklılaşma her zamankinden daha kritik
   - Kaynak: [VG Insights — 2024 Global Report](https://vginsights.com/insights/article/global-indie-games-market-report-2024)

6. **Generic fantezi "terk edilmesi gereken" temalar listesinde** — Ama **benzersiz fantezi açıları listede değil**
   - Kaynak: [Gamedeveloper — 10 Themes to Abandon](https://www.gamedeveloper.com/business/10-themes-commercial-indies-should-abandon)

---

## 6. Üretim Etkisi Analizi

### Gerçekçi İnsan Evreni

| Faktör | Değerlendirme |
|--------|---------------|
| **Referans malzemesi** | Bol — gerçek apartman fotoğrafları, YouTube videoları |
| **Sanat üretim hızı** | Hızlı — referansla çalışma kolay |
| **Karakter çeşitliliği** | Sınırlı — insanlar birbirine benzeyebilir |
| **"Sıradan görünme" riski** | Yüksek — The Tenants, Project Highrise ile karışabilir |
| **Hikaye esnekliği** | Orta — gerçekçilik kurallarıyla sınırlı |
| **Asset yeniden kullanımı** | Kolay — mobilya, duvar, zemin standart |

### Fantezi Canavar Evreni

| Faktör | Değerlendirme |
|--------|---------------|
| **Referans malzemesi** | Az — sıfırdan tasarım gerekir |
| **Sanat üretim hızı** | Yavaş — her canavar benzersiz tasarlanmalı |
| **Karakter çeşitliliği** | Sınırsız — 100 farklı canavar türü mümkün |
| **"Sıradan görünme" riski** | Çok düşük — pazarda benzeri neredeyse yok |
| **Hikaye esnekliği** | Çok yüksek — kuralları siz koyarsınız |
| **Asset yeniden kullanımı** | Zor — her tür canavar için ayrı asset |

### İndie Ekipler İçin Art Style Karşılaştırması

> "Stilize grafikler daha az kaynakla üretilebilir, daha düşük donanımda çalışır ve oyunu daha geniş bir kitleye açar. Stardew Valley, Hollow Knight ve Darkest Dungeon gibi oyunlar kısmen benzersiz sanat stilleriyle kalabalık pazarda öne çıktığı için büyük hit oldu."
> — Kaynak: [N-iX Game Studio](https://gamestudio.n-ix.com/realistic-vs-stylized-art-in-video-game-development/)

**Sonuç:** Cartoon/hand-drawn stiliniz her iki evren için de uygundur. Ama **fantezi evreni, cartoon stille çok daha iyi eşleşir** — gerçekçi bir evren cartoon stilde "ucuz" görünebilirken, fantezi evren cartoon stilde "kasıtlı ve şirin" görünür.

---

## 7. Karar Matrisi

Her kriter 1-10 arasında puanlanmıştır. Puanların gerekçeleri aşağıda açıklanmıştır.

| Kriter | Ağırlık | Gerçekçi İnsan | Gerekçe (Gerçekçi) | Fantezi Canavar | Gerekçe (Fantezi) |
|--------|---------|----------------|---------------------|-----------------|---------------------|
| **Pazar boşluğu** | %25 | 3/10 | 8+ gerçekçi rakip var (The Tenants, Project Highrise vb.) | 9/10 | Yalnızca 1 rakip (Unholy Heights, 2013) — neredeyse boş pazar |
| **Oyuncu tercihi** | %20 | 6/10 | Kanıtlanmış talep var ama "wow" etkisi yok | 8/10 | Unholy Heights %90 review, Lobotomy Corp %94 — canavar yönetimi sevilir |
| **Rakip performansı** | %20 | 5/10 | En iyi rakip ~$5M (The Tenants) — orta tavan | 9/10 | Lobotomy Corp ~$49M, Against the Storm 1M+ satış — çok yüksek tavan |
| **Üretim fizibilitesi** | %15 | 8/10 | Referans bol, asset üretimi hızlı | 5/10 | Her canavar sıfırdan tasarlanmalı, daha fazla sanat çalışması |
| **Farklılaşma gücü** | %10 | 3/10 | "Bir apartman yönetim oyunu daha" riski | 9/10 | "Canavar apartman yönetimi" — benzersiz, akılda kalıcı pitch |
| **Trend yönü** | %10 | 6/10 | İş simülasyonu trendi destekler | 8/10 | "Cozy + quirky" management trend, benzersiz tema Steam'de öne çıkar |

### Toplam Ağırlıklı Skor

**Gerçekçi İnsan Evreni:**
(3×0.25) + (6×0.20) + (5×0.20) + (8×0.15) + (3×0.10) + (6×0.10) = 0.75 + 1.20 + 1.00 + 1.20 + 0.30 + 0.60 = **5.05 / 10**

**Fantezi Canavar Evreni:**
(9×0.25) + (8×0.20) + (9×0.20) + (5×0.15) + (9×0.10) + (8×0.10) = 2.25 + 1.60 + 1.80 + 0.75 + 0.90 + 0.80 = **8.10 / 10**

```
Gerçekçi İnsan:  ██████████░░░░░░░░░░  5.05/10
Fantezi Canavar:  ████████████████████  8.10/10
                                        △ +3.05 fark
```

---

## 8. Öneri ve Analiz

### Ana Bulgular — Nedensellik Analizi

#### Bulgu 1: Fantezi canavar evreni pazar boşluğu açısından çok üstün

**Veri:** Gerçekçi apartman/bina yönetim nişinde 8+ aktif oyun varken, canavar apartman yönetimi nişinde yalnızca 1 oyun (Unholy Heights, 2013) var.

**Neden bu önemli:** Bir pazarda rakip sayısı arttıkça, yeni girenin dikkat çekme maliyeti üstel olarak artar. 8 rakipli bir pazarda öne çıkmak, 1 rakipli bir pazara kıyasla çok daha fazla pazarlama bütçesi ve kalite gerektirir. Kalabalık bir pazarda "ortalama" bir oyun kaybolurken, boş bir pazarda "iyi" bir oyun doğal keşfedilebilirlik kazanır.

**Nedensellik:** Pazar boşluğu → Düşük rekabet → Daha yüksek organik görünürlük → Daha düşük müşteri edinme maliyeti → Daha yüksek ROI

---

#### Bulgu 2: Fantezi/benzersiz temalar yönetim simülasyonlarında daha yüksek gelir tavanı yaratır

**Veri:**
- Lobotomy Corporation (canavar yönetimi): ~$49M gelir
- Two Point Hospital (absürd karikatür): ~$9.4M gelir
- Against the Storm (fantezi şehir): 1M+ satış
- Project Highrise (gerçekçi bina): ~$4-10M gelir (tahmin)
- The Tenants (gerçekçi apartman): ~$5M gelir (tahmin)

**Neden bu önemli:** Fantezi/benzersiz temalı oyunların gelir tavanı, gerçekçi temalı oyunlara kıyasla **5-10x daha yüksek**. Bu fark, oyun kalitesi dışında doğrudan tema seçimiyle açıklanabilir.

**Nedensellik:** Benzersiz tema → Sosyal medyada paylaşılabilirlik → Viral büyüme potansiyeli → Daha geniş kitleye ulaşım → Daha yüksek toplam gelir. Gerçekçi tema ise doğası gereği "screenshot'lanabilir" değildir — bir apartman screenshot'ı viral olmaz, ama "3 boynuzlu bir canavar kiracının mutfak sorunu" viral olur.

---

#### Bulgu 3: "Canavar apartman" konsepti oyuncu tarafından kanıtlanmış

**Veri:** Unholy Heights %90 pozitif review'a sahip. Eleştirmenler "temel konsept harika" demiş. Ancak oyun $3.99 fiyat noktasında, 5 saat uzunluğunda ve 2013 yapımı.

**Neden bu önemli:** %90 pozitif review, konseptin oyuncuları memnun ettiğinin kanıtıdır. Düşük satış ($3.99 × ~55K = ~$220K gelir), konseptin başarısızlığını değil, **uygulamanın yetersizliğini** gösterir. Modern bir yapımla, derin mekaniklerle ve uygun fiyat noktasıyla bu konsept çok daha fazla gelir üretebilir.

**Nedensellik:** Kanıtlanmış konsept + modern uygulama + boş pazar = yüksek başarı olasılığı

---

#### Bulgu 4: Cartoon/hand-drawn stil fantezi evreniyle daha iyi eşleşir

**Veri:** İndie başarı hikayeleri (Stardew Valley, Hollow Knight, Darkest Dungeon) stilize sanatla öne çıkmış. N-iX araştırması stilize sanatın indie ekipler için daha düşük maliyetli ve daha farklılaştırıcı olduğunu gösteriyor.

**Neden bu önemli:** Cartoon stilinde gerçekçi bir apartman çizdiğinizde, oyuncu "neden gerçekçi değil?" diye sorar. Cartoon stilinde bir canavar apartmanı çizdiğinizde, oyuncu "ne kadar şirin!" der. **Sanat stili ve evren seçimi uyumlu olmalıdır.**

**Nedensellik:** Cartoon stil + fantezi evren = tutarlı estetik → Oyuncu beklentisiyle uyum → Daha yüksek memnuniyet

---

#### Bulgu 5: Üretim maliyeti dezavantajı, diğer avantajlarla telafi edilir

**Veri:** Fantezi temanın en büyük dezavantajı üretim maliyeti — her canavar sıfırdan tasarlanmalı. Gerçekçi temada referans bolluğu üretimi hızlandırır.

**Ama:** Bu dezavantaj 3 şekilde telafi edilir:
1. Canavar tasarımları **yeniden kullanılabilir** — bir canavar türü birden fazla kiracı olarak görünebilir
2. Stilize/cartoon art **zaten referansa daha az bağımlı** — sıfırdan çizmek bu stilde doğal
3. Üretim hızı dezavantajı, **pazar avantajıyla** (boş niş, yüksek gelir tavanı) fazlasıyla karşılanır

---

### Risk Analizi

| Risk | Gerçekçi Tema | Fantezi Tema |
|------|--------------|--------------|
| **Pazarda kaybolma** | YÜKSEK — 8+ rakip arasında görünmezlik | DÜŞÜK — benzersiz konsept |
| **Hikayenin zayıflaması** | DÜŞÜK — İlkkan'ın hikayesi gerçekçi evrene uygun | ORTA — hikayeyi fantezi evrene adapte etmek gerekir |
| **Üretim gecikmesi** | DÜŞÜK — referans bol | ORTA — canavar tasarımları zaman alır |
| **Gelir beklentisini karşılayamama** | ORTA — tavan ~$5M civarı | DÜŞÜK — tavan çok daha yüksek, boş niş |
| **Oyuncu beklentisi uyumsuzluğu** | DÜŞÜK — bilinen format | DÜŞÜK — Unholy Heights %90 ile konsepti kanıtlamış |

---

### Hibrit Seçenek: "Gerçekçi Hikaye + Fantezi Kiracılar"

Bir üçüncü yol da mümkündür:

> İlkkan gerçek bir insan. Şehir gerçekçi. Ama büyükannenin apartmanı sıradan bir apartman değilmiş — kiracıları canavarlar, yaratıklar ve doğaüstü varlıklardır. İlkkan bunu bilmeden devralmıştır.

Bu hibrit yaklaşım:
- **Hikaye bağlamını korur** — İlkkan'ın "hayatta amaç bulma" teması aynen kalır
- **Fantezi avantajlarını kazanır** — benzersiz kiracılar, viral potansiyel, boş niş
- **Komedi potansiyeli yaratır** — "sıradan bir adam canavarları yönetmeye çalışıyor" doğal komedi kaynağı
- **Two Point Hospital etkisi** — absürd durum + yönetim simülasyonu = kanıtlanmış başarı formülü

---

### Nihai Öneri

**Fantezi canavar evreni (tercihen hibrit yaklaşımla) önerilir.**

Gerekçe özeti:
1. Karar matrisinde **8.10 vs 5.05** — net fark
2. Pazar **neredeyse boş** — 2013'ten beri ciddi rakip yok
3. Gelir tavanı **5-10x daha yüksek** (vaka çalışmaları kanıtı)
4. Konsept **%90 pozitif review** ile oyuncu tarafından kanıtlanmış
5. Cartoon sanat stiliyle **doğal uyum**
6. Hibrit yaklaşım, İlkkan'ın hikayesini korurken tüm avantajları kazandırır

**Tek koşul:** Generic "orta çağ fantezisi" tuzağına düşmemek. Tema **spesifik ve alışılmadık** olmalı: "Bir apartmanda canavarlarla birlikte yaşamak" — bu kadar özgün olması yeterli.

---

## 9. Kaynakça

### Steam Oyun Sayfaları

| Oyun | Link |
|------|------|
| The Tenants | [store.steampowered.com/app/1009560](https://store.steampowered.com/app/1009560/The_Tenants/) |
| Project Highrise | [store.steampowered.com/app/423580](https://store.steampowered.com/app/423580/Project_Highrise/) |
| News Tower | [store.steampowered.com/app/1649950](https://store.steampowered.com/app/1649950/News_Tower/) |
| Landlord's Super | [store.steampowered.com/app/1127840](https://store.steampowered.com/app/1127840/Landlords_Super/) |
| Small Spaces | [store.steampowered.com/app/3151380](https://store.steampowered.com/app/3151380/Small_Spaces/) |
| Mad Tower Tycoon | [store.steampowered.com/app/910880](https://store.steampowered.com/app/910880/Mad_Tower_Tycoon/) |
| Constructor Plus | [store.steampowered.com/app/898800](https://store.steampowered.com/app/898800/Constructor_Plus/) |
| Landlord Simulator | [store.steampowered.com/app/803310](https://store.steampowered.com/app/803310/Landlord_Simulator/) |
| Beholder | [store.steampowered.com/app/475550](https://store.steampowered.com/app/475550/Beholder/) |
| Beholder 2 | [store.steampowered.com/app/761620](https://store.steampowered.com/app/761620/Beholder_2/) |
| Beholder 3 | [store.steampowered.com/app/1570070](https://store.steampowered.com/app/1570070/Beholder_3/) |
| Unholy Heights | [store.steampowered.com/app/249330](https://store.steampowered.com/app/249330/Unholy_Heights/) |
| Lobotomy Corporation | [store.steampowered.com/app/568220](https://store.steampowered.com/app/568220/Lobotomy_Corporation__Monster_Management_Simulation/) |
| Against the Storm | [store.steampowered.com/app/1336490](https://store.steampowered.com/app/1336490/Against_the_Storm/) |
| War for the Overworld | [store.steampowered.com/app/230190](https://store.steampowered.com/app/230190/War_for_the_Overworld/) |
| Dungeon Inn | [store.steampowered.com/app/2552310](https://store.steampowered.com/app/2552310/Dungeon_Inn/) |
| Bloody Hell Hotel | [store.steampowered.com/app/2055770](https://store.steampowered.com/app/2055770/Bloody_Hell_Hotel/) |
| Two Point Hospital | [store.steampowered.com/app/535930](https://store.steampowered.com/app/535930/Two_Point_Hospital/) |
| Prison Architect | [store.steampowered.com/app/233450](https://store.steampowered.com/app/233450/Prison_Architect/) |
| Monster Care Simulator | [store.steampowered.com/app/3288270](https://store.steampowered.com/app/3288270/Monster_Care_Simulator/) |

### Veri Araçları

| Araç | Link | Güvenilirlik |
|------|------|-------------|
| SteamDB | [steamdb.info](https://steamdb.info/) | Yüksek |
| SteamSpy | [steamspy.com](https://steamspy.com/) | Orta |
| VG Insights | [vginsights.com](https://vginsights.com/) | Yüksek |
| Gamalytic | [gamalytic.com](https://gamalytic.com/) | Yüksek-Orta |
| Steam250 | [steam250.com](https://steam250.com/) | Yüksek |
| Steam Revenue Calculator | [steam-revenue-calculator.com](https://steam-revenue-calculator.com/) | Orta |

### Endüstri Makaleleri ve Analizler

| Makale | Kaynak | Link |
|--------|--------|------|
| 10 Themes Commercial Indies Should Abandon | Gamedeveloper.com | [Link](https://www.gamedeveloper.com/business/10-themes-commercial-indies-should-abandon) |
| Realistic vs Stylized Art in Video Games | N-iX Game Studio | [Link](https://gamestudio.n-ix.com/realistic-vs-stylized-art-in-video-game-development/) |
| Art Styles in Indie vs AAA Games | Pixune | [Link](https://pixune.com/blog/art-styles-in-indie-games-vs-aaa-games/) |
| What the Hell Happened in 2025? | How To Market A Game | [Link](https://howtomarketagame.com/2026/01/27/what-the-hell-happened-in-2025/) |
| The Cycle of a Hit Genre | How To Market A Game | [Link](https://howtomarketagame.com/2025/11/12/the-cycle-of-a-hit-genre/) |
| Crafty Buildy Strategy Simulation Guide | How To Market A Game | [Link](https://howtomarketagame.com/2025/07/02/crafty-buildy-strategy-simulation-buyers-guide/) |
| Deep Dive into Steam Review Ratio | Gamalytic | [Link](https://gamalytic.com/blog/a-deep-dive-into-the-steam-review-ratio) |
| How to Do Market Research for Indie Games | Gamalytic | [Link](https://gamalytic.com/blog/dow-to-do-market-research-for-your-indie-game) |
| Steam Sales Estimation Methodology | VG Insights | [Link](https://vginsights.com/insights/article/steam-sales-estimation-methodology-and-accuracy) |

### Pazar Raporları

| Rapor | Kaynak | Link |
|-------|--------|------|
| Simulation Game Market | Verified Market Research | [Link](https://www.verifiedmarketresearch.com/product/simulation-game-market/) |
| Simulation Game Market Size 2032 | Global Growth Insights | [Link](https://www.globalgrowthinsights.com/market-reports/simulation-game-market-102402) |
| Indie Games Revenue on Steam | Game World Observer | [Link](https://gameworldobserver.com/2024/10/16/indie-games-revenue-steam-vs-aaa-titles-vg-insights) |
| Indie Game Market | Mordor Intelligence | [Link](https://www.mordorintelligence.com/industry-reports/indie-game-market) |
| Indie Game Market 2033 | SkyQuest | [Link](https://www.skyquestt.com/report/indie-game-market) |
| Business Simulation Games Market | Verified Market Reports | [Link](https://www.verifiedmarketreports.com/product/business-simulation-games-market/) |
| Global Indie Games Market Report 2024 | VG Insights | [Link](https://vginsights.com/insights/article/global-indie-games-market-report-2024) |
| 2025 Indie Game Trends | Accio | [Link](https://www.accio.com/business/2025-indie-game-trends) |
| 12 Indie Game Trends for 2025 | Medium (DM Johnston) | [Link](https://dmjohnston.medium.com/12-indie-game-trends-for-2025-46d02f36f0e3) |

### Wikipedia ve Referans

| Konu | Link |
|------|------|
| Two Point Hospital | [Wikipedia](https://en.wikipedia.org/wiki/Two_Point_Hospital) |
| Prison Architect | [Wikipedia](https://en.wikipedia.org/wiki/Prison_Architect) |
| Fallout Shelter | [Wikipedia](https://en.wikipedia.org/wiki/Fallout_Shelter) |
| Steam Spy | [Wikipedia](https://en.wikipedia.org/wiki/Steam_Spy) |
| SimTower | [Wikipedia](https://en.wikipedia.org/wiki/SimTower) |

### Oyun Listeleri ve Karşılaştırmalar

| Kaynak | Link |
|--------|------|
| Best Management Games 2026 — PCGamesN | [Link](https://www.pcgamesn.com/best-management-games) |
| Best Tycoon Games — High Ground Gaming | [Link](https://www.highgroundgaming.com/best-tycoon-games/) |
| Best Management Sims — PC Gamer | [Link](https://www.pcgamer.com/the-best-management-sims-on-pc/) |
| Best Fantasy Management Games — Game Rant | [Link](https://gamerant.com/best-fantasy-management-games/) |
| Property Management Simulation Games — Zeevou | [Link](https://zeevou.com/blog/property-management-simulation-games/) |
| Top Simulation Games — DMG Podcast | [Link](https://www.dmggamingpodcast.com/blog/top-simulation-games-for-building-management-skills/) |

---

*Rapor Sonu — Apartman Projesi, Evren Seçimi Araştırması v1.0*
