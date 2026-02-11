# Game Design Document — Grandma Left Me a Building

**Versiyon:** 0.2
**Tarih:** 2026-02-10
**Durum:** Taslak (detaylandırılıyor)

---

## 1. Vizyon & Çekirdek Konsept

### Elevator Pitch

> Babaannesinden miras kalan harap bir apartmanı komik, kaotik ve beklenmedik olaylarla dolu bir süreçte ayağa kaldırdığın 2D apartman yönetim simülasyonu. Kiracı bul, isteklerini karşıla, binayı geliştir, kaynaklarını yönet — ve şehrin en saygın ve renkli apartmanını yarat!

### Oyun Kimliği

| Alan | Detay |
|------|-------|
| **Oyun Adı** | Grandma Left Me a Building |
| **Tür** | Apartman Yönetim Simülasyonu (Management Sim) |
| **Platform** | PC (Steam) |
| **Motor** | Unity 2D |
| **Kamera** | 2D dış cephe görünüm (apartman dışarıdan görünür — her katta sağlı sollu 2 daire, balkon ve pencereler ile kiracılar belli olur) |
| **Kontrol** | Mouse — tıklama tabanlı (karakter hareketi yok) |
| **Sanat Stili** | Cartoon / Hand-drawn |
| **Gelir Modeli** | Premium (tek seferlik satın alma) |
| **Oyun Tonu** | Komik & Kaotik — absürt durumlar, abartılı karakterler, beklenmedik olaylar |

### Oyuncu Fantezisi

Oyuncu, dökülen bir binayı adım adım toparlamanın, garip ve absürt yaratık kiracılarla uğraşmanın, sınırlı kaynaklarla en doğru kararları vermenin ve sonunda şehrin en renkli apartmanını kurmanın **tatminini** yaşar.

Temel çekim gücü: **Kaynak yönetimi ve inşa etme hissi.** Oyuncu her gün kısıtlı parayla binayı nasıl geliştireceğine, hangi yaratığı kiracı alacağına, hangi talebi karşılayacağına karar verir. Doğru kararlar verince bina gelişir, saygınlık artar, daha iyi kiracılar gelir — bu döngünün kendisi ödüldür. Buna ek olarak, kiracıları daireler arasında stratejik olarak konumlandırmak (drag-drop ile yer değiştirme) önemli bir katman ekler — kiracıların birbirine göre konumu mutluluğu doğrudan etkiler. Komik olaylar ve absürt yaratıklar bu süreci eğlenceli tutar.

### Benzersiz Satış Noktası (USP)

**"Her gün yeni bir kaos, her kaos yeni bir kahkaha."** Babaannenden kalan apartmanda bir gün bile sıkıcı geçmez. Balkonda uyuyan dev blob, kira gününde ortalıktan kaybolan parlak yaratık, yan yana koydukların kavga edince çöken mutluluk. Her şey kontrolden çıkmak üzereyken doğru hamleyi yapmanın verdiği tatmin, işte bu oyunu bırakılmaz kılan şey. Apartman yönetimi hiç bu kadar absürt, bu kadar kaotik ve bu kadar eğlenceli olmamıştı.

### Design Pillars

Oyunun tüm tasarım kararlarına yön veren temel ilkeler. Bir özellik hiçbir pillar'a hizmet etmiyorsa oyuna girmemeli.

| # | Pillar | Açıklama |
|---|--------|----------|
| 1 | **Komik Kaos** | Her gün beklenmedik, absürt ve güldüren şeyler olur. Oyuncu stres değil eğlence yaşar. |
| 2 | **Stratejik Yerleşim** | Kimi alacağın, nereye koyacağın, kimi çıkaracağın. Her kiracı kararı bir bulmaca. Kiracıların birbirine göre konumu mutluluğu doğrudan etkiler. (Referans: *Is This Seat Taken?* yerleştirme bulmacası, bizim oyunda canlı yönetim sim katmanıyla birleşiyor.) |
| 3 | **Görsel Dönüşüm** | Bakımsız binayı adım adım şehrin en renkli apartmanına çevirmenin tatmini. Her yükseltme binada dışarıdan görünür. |
| 4 | **Kıt Kaynakla Hayatta Kalma** | Para her zaman az. Her harcama bir fedakarlık. Doğru önceliklendirme ödüllendiriliyor. |

### Hedef Kitle

| Özellik | Detay |
|---------|-------|
| **Birincil kitle** | Casual-midcore yönetim/sim oyuncuları (20-35 yaş) |
| **Oyun profili** | Akşam 2-3 saat rahat oturup eğlenceli bir şey oynamak isteyen kişiler |
| **Seven oldukları** | Kaynak yönetimi, bina/tesis geliştirme, komik karakterler, hızlı ilerleme hissi |
| **Sevmedikleri** | Aşırı karmaşık sistemler, cezalandırıcı zorluk, yavaş ilerleme |
| **Benzer oyunlar** | The Tenants, Two Point Hospital, Spiritfarer, House Flipper, Is This Seat Taken? |

### Referans Oyunlar & İlham Kaynakları

| Oyun | Ne alıyoruz | Ne almıyoruz |
|------|-------------|--------------|
| **The Tenants** | Kiracı yönetimi, oda tamir/yenileme, apartman ekonomisi | Gerçekçi ciddi ton, first-person perspektif |
| **Beholder** | Yan kesit apartman görünümü, kiracı gözlemi, olay sistemi | Karanlık politik ton, gözetleme mekaniği |
| **Spiritfarer** | Sıcak atmosfer, karakter ilişkileri, görsel stil ilhamı | Hikaye ağırlıklı yapı, platformer hareket |
| **Two Point Hospital** | Komik ton, absürt olaylar, erişilebilir yönetim mekaniği | 3D perspektif, hastane teması |
| **Is This Seat Taken?** | Karakter yerleştirme bulmacası, komşuluk tercihleri, drag-drop mekaniği | Statik bulmaca yapısı (bizde canlı yönetim sim) |

---

## 2. Konsept ve Hikaye

### Hikaye (Minimal — Sadece Giriş & Arka Plan)

Bir baltaya sap olamayan, babaannesini yıllardır aramayan, hayattan bir beklentisi kalmamış tembel ve karikatürize bir tip: **İlkkan.** Bir gün telefonla aranır. Arayan bir avukattır. Babaannesi vefat etmiştir. Vasiyet olarak İlkkan'a eski aile apartmanını bırakmıştır — apartmanı işletmesi ve **asla satmaması** şartıyla.

Bu sıcak ve eski apartmanı tekrar adam etmek çok zordur. İlkkan hayatında yeni bir amaç bulmuştur. Ama bir apartman yönetmek kolay görünse de, başına geleceklerden habersizdir...

> **Hikaye yaklaşımı:** Hikaye sadece oyunun başlangıcında kısa bir sahne olarak anlatılır. Sonrasında oyunda aktif bir hikaye akışı yoktur. Oyuncu kendi hikayesini gameplay ile yaratır. İlkkan oyun içinde görünür bir karakter değildir — **oyuncu = İlkkan.**

### Kaybetme Koşulu (Lose Condition)

Oyunun tek kaybetme koşulu: **Paranın bitmesi.**

- Para 0₺'a düşerse belediyeden **uyarı** gelir (3 gün süre)
- 3 gün içinde toparlamazsan → **apartman mühürlenir** → Oyun biter
- Oyuncu yeni oyun başlatır veya son kayıttan devam eder

**Sürekli gider baskısı:**
- Çalışan maaşları (günlük)
- Faturalar (haftalık)
- Vergi (30 günde bir — büyük gider)
- Anlık olay masrafları (su baskını, hasar vb.)
- Kiracı yoksa gelir yok ama giderler devam eder

---

## 3. Evren & Tema

### Evren Kararı: Hibrit

Oyun **hibrit bir evren** kullanır: İlkkan gerçek bir insandır, ama apartmana taşınan kiracılar **garip, absürt ve beklenmedik yaratıklardır.** İlkkan başta bunu bilmez — ilk kiracı geldiğinde hem oyuncu hem İlkkan şaşırır. Ama kısa sürede bu "normal" hale gelir ve oyun bunu sorgulamadan kabul eder.

Bu hibrit yaklaşım şunları sağlar:
- **Hikaye tarafı:** İlkkan'ın gerçekçi motivasyonu (miras, zorunluluk) oyuncuya bağlam verir
- **Gameplay tarafı:** Yaratık çeşitliliği sayesinde mekanik farklılıklar yaratılabilir (bir ateş yaratığının oda ihtiyaçları bir buz yaratığından farklıdır)
- **Ton tarafı:** Absürt yaratıklar + gerçekçi apartman problemleri = komik kontrast

### Yaratık Tasarım Felsefesi: Garip & Absürt

Yaratıklar klasik fantezi ırkları (elf, ork) değil, **tuhaf, beklenmedik ve "bu ne ya?" dedirten** ama aynı zamanda sevimli/sempatik varlıklardır.

**Tasarım ilkeleri:**
- Her yaratığın görünüşü onun kişiliğini ve ihtiyaçlarını yansıtır
- Absürt ama tutarlı — her yaratığın kendi mantığı var
- Oyuncuda merak uyandırır: "Acaba bir sonraki kiracı ne olacak?"
- Komik ton: Yaratıkların apartman sorunlarıyla (tesisat, komşu gürültüsü, kira) uğraşması doğal olarak komik

**Örnek yaratık konseptleri** (yer tutucu — detaylar sonra belirlenir):
- Sürekli büyüyen bir yaratık → odası her gün biraz daha küçük gelir
- Her şeyi yiyen bir blob → mobilya tamir masrafları artar ama kira yüksek öder
- Gece parlayan bir yaratık → komşularını rahatsız eder ama geceleri güvenlik sağlar
- Buhar çıkaran sıcak bir yaratık → kışın ısıtma gerekmez ama yazın şikayet patlar

### Temanın Mekaniklere Etkisi

| Mekanik | Gerçekçi Evrende | Hibrit Evrende (Bizim Oyun) |
|---------|-------------------|------------------------------|
| **Kiracı çeşitliliği** | İnsan tipleri (aile, öğrenci, yaşlı) | Yaratık türleri — her biri farklı ihtiyaç/avantaj/sorun |
| **Oda ihtiyaçları** | Standart mobilya | Yaratığa özel gereksinimler (su havuzu, karanlık oda, yüksek tavan) |
| **Olaylar** | Gerçekçi (boru patlaması, komşu kavgası) | Absürt + gerçekçi karışım (yaratık büyüdü odaya sığmıyor + boru patlaması) |
| **Komedi kaynağı** | Durumsal komedi | Yaratık doğası + apartman gerçekliği kontrastı |
| **Emlakçı sistemi** | Normal emlakçı | Yaratık emlakçısı — saygınlık arttıkça daha egzotik/güçlü yaratıklara erişim |

### Dünya Kuralları

- İlkkan'ın dünyasında yaratıkların varlığı **normal karşılanır** — kimse "neden yaratıklar var?" diye sorgulamaz
- Yaratıklar toplumda yaşar, çalışır, kira öder, şikayet eder — tıpkı insanlar gibi
- Oyun bu durumu ciddiye almaz, komik kontrastı kucaklar
- Babaannenin apartmanının eskiden de yaratık kiracıları olup olmadığı bir **hikaye sırrı** olarak kullanılabilir

---

## 4. Temel Mekanikler

### 4.1 Core Loop (Günlük Döngü)

**Sistem:** Tam tur bazlı (turn-based). Oyuncu istediği kadar düşünür, aksiyonlarını yapar, hazır olunca "Günü Bitir" butonuna basar. Zaman baskısı yoktur.

```
  ┌──────────────────────────────────────────────┐
  │              1. GÜN BAŞI                      │
  │  • Günün olayları gösterilir (popup/kart)     │
  │  • Kiracı talepleri ortaya çıkar              │
  │  • Kira gelirleri otomatik toplanır           │
  │  • Varsa faturalar/giderler düşer             │
  └──────────────┬───────────────────────────────┘
                 ▼
  ┌──────────────────────────────────────────────┐
  │           2. AKSİYON FAZI (Serbest)           │
  │  Oyuncu istediği sırada:                      │
  │  • Olaylarda karar verir                      │
  │  • Kiracı taleplerini çözer                   │
  │  • Tamir / yenileme başlatır                  │
  │  • Emlakçıya gider, yeni kiracı seçer         │
  │  • Binayı gezer, durumu kontrol eder          │
  │  Hazır olunca → "Günü Bitir" butonuna basar   │
  └──────────────┬───────────────────────────────┘
                 ▼
  ┌──────────────────────────────────────────────┐
  │              3. GÜN SONU                      │
  │  • Kaynaklar güncellenir (₺, 😊, ⭐)          │
  │  • Tamir/yenileme ilerlemesi güncellenir      │
  │  • Günün özet raporu gösterilir               │
  │  • Sonraki güne geçilir                       │
  └──────────────┬───────────────────────────────┘
                 │
                 └──────────► Yeni güne dön
```

#### Tempo: Zamanla Artan Kaos

Oyun başında sakin, sonlara doğru kaotik. Bu hem öğrenme eğrisini yumuşatır hem de oyunun komik tonunu destekler.

| Oyun Aşaması | Gün Başına Olay | Aktif Kiracı | Örnek |
|--------------|-----------------|--------------|-------|
| **Erken** (Gün 1-15) | 1-2 olay | 1-2 kiracı | Bir boru patlaması + bir kiracı isteği |
| **Orta** (Gün 16-40) | 3-4 olay | 3-5 kiracı | Belediye denetimi + 2 kiracı talebi + komşu kavgası |
| **Geç** (Gün 40+) | 5+ olay | 6+ kiracı | 3 kiracı talebi + yangın + vergi günü + misafir istilası |

> Kaosun artması = komiğin artması. Oyuncu geç oyunda "ne yapacağımı bilemiyorum" hissini yaşamalı ama bu sinir bozucu değil, **eğlenceli** olmalı.

#### Örnek Bir Gün (Orta Oyun — Gün 25)

1. **Gün Başı:** Kira geliri +850₺. Fatura -200₺. 3 olay belirir:
   - Blob kiracı gece yine mobilyayı yemiş (şikayet)
   - 2. kattaki parlayan yaratık komşusunu rahatsız ediyor
   - Belediyeden denetim haberi geldi (3 gün sonra)
2. **Aksiyon Fazı:** Oyuncu serbest:
   - Blob için yeni mobilya alır (-150₺) veya uyarı verir (mutluluk düşer)
   - Parlayan yaratığı üst kata taşır (taşınma masrafı) veya komşuya perde alır
   - Belediye denetimine hazırlanmak için bina dışını boyatmaya karar verir (-300₺)
   - Emlakçıya gidip 3. kat için yeni kiracı adaylarına bakar
   - "Günü Bitir" butonuna basar
3. **Gün Sonu:** Para: 1200₺ → 550₺. Mutluluk: %72 → %68. Saygınlık: %55 → %58. Boya işi %50 tamamlandı.

#### Emlakçı Sistemi

Oyuncu **aktif olarak** emlakçıya gider (apartman dışında bir UI paneli veya ayrı bir ekran).

- Emlakçıda her zaman birkaç kiracı adayı listelenir
- Her adayın **profil kartı** vardır: tür, kira ödeme gücü, özel ihtiyaçlar, potansiyel sorunlar
- Saygınlık arttıkça emlakçıdaki aday havuzu genişler ve kalitesi artar
- Aday listesi birkaç günde bir yenilenir (oyuncu "bu turda beğenmedim" diyebilir)
- Bazı özel/nadir yaratıklar sadece yüksek saygınlıkta açılır

| Saygınlık | Emlakçı Aday Kalitesi |
|-----------|----------------------|
| ⭐ 0-20 | 1-2 aday, düşük kiralı, sorunlu tipler |
| ⭐ 21-50 | 3-4 aday, karma kalite |
| ⭐ 51-80 | 4-5 aday, iyi kiracılar mevcut |
| ⭐ 81-100 | 5-6 aday, nadir/özel yaratıklar açılır |

### 4.2 Kaynak Sistemi

Oyunda **3 ana kaynak** vardır. Fazlası yok — ama bu üçünün birbirine etkisi oyunun stratejik derinliğini yaratır.

#### Kaynaklar

| Kaynak | Aralık | Açıklama |
|--------|--------|----------|
| **Para (₺)** | 0 — ∞ | Ana ekonomik kaynak. Her şeyin bedeli var. |
| **Mutluluk (😊)** | 0 — 100 | Apartmanın genel memnuniyet skoru. Kiracıların ödeme düzenini etkiler. |
| **Saygınlık (⭐)** | 0 — 100 | Apartmanın mahalle itibarı. Emlakçıdaki kiracı kalitesini belirler. |

#### Para (₺) — Detay

| Kazanım Yolları | Harcama Yolları |
|------------------|-----------------|
| Kira gelirleri (ana gelir) | Oda tamir/yenileme |
| Olay ödülleri | Kiracı taleplerini karşılama |
| Özel kiracı bonusları | Faturalar (sabit giderler) |
| | Emlakçı komisyonu |
| | Bina dış cephe/ortak alan |

**Ekonomi dengesi:** Para her zaman kıt. Doğru kararlar verirsen idare edersin ama rahat rahat harcayamazsın. "Bunu mu yapsam şunu mu?" ikilemi sürekli var. Hatalar acı verir ama spiral değil — toparlanma mümkün.

#### Mutluluk (😊) — Detay

Apartmanın genel memnuniyet skoru. **Kiracıların kira ödeme düzenini doğrudan etkiler.**

| Mutluluk | Ödeme Davranışı |
|----------|-----------------|
| 80-100 | Kiracılar gününde öder, bonus şansı |
| 50-79 | Normal ödeme, ara sıra gecikme |
| 25-49 | Sık gecikme, kısmi ödeme, şikayet artışı |
| 0-24 | Ödeme aksatma, taşınma tehditleri, kiracı kaybı riski |

| Artıran | Azaltan |
|---------|---------|
| Kiracı taleplerini karşılamak | Talepleri görmezden gelmek |
| Odalarda iyileştirme yapmak | Bozuk/hasar görmüş odalar |
| Olaylarda kiracı lehine kararlar | Kiracı aleyhine kararlar |
| Ortak alan iyileştirmeleri | Uzun süreli bakımsızlık |

#### Saygınlık (⭐) — Detay

Apartmanın mahalle itibarı. **Emlakçıdaki kiracı havuzunun kalitesini belirler.**

| Saygınlık | Emlakçı Etkisi |
|-----------|---------------|
| 0-20 | Sadece Seviye 1 kiracılar (düşük kira, çok sorun) |
| 21-50 | Seviye 1-2 kiracılar |
| 51-80 | Seviye 1-3 kiracılar (iyi kiracılar mevcut) |
| 81-100 | Seviye 1-4 kiracılar (nadir/özel yaratıklar açılır) |

| Artıran | Azaltan |
|---------|---------|
| Bina dış cephe bakımı | Bakımsız dış görünüm |
| Yüksek mutluluk (dolaylı) | Skandallar, kavgalar |
| Belediye denetimlerini geçmek | Denetimden kalmak |
| Özel etkinlikler/iyileştirmeler | Kiracı şikayetlerinin yayılması |

#### Kaynak İlişki Haritası

```
  Saygınlık ⭐ ──────► Kiracı Kalitesi (Emlakçı)
       │                        │
       │                        ▼
       │               Yüksek Seviye Kiracı
       │                        │
       │                        ▼
       │                 Yüksek Kira Geliri ──► Para ₺
       │                                          │
       │                                          ▼
       │                                  Tamir & İyileştirme
       │                                          │
       ▲                                          ▼
       └──────────────────────────────── Mutluluk 😊
                                                  │
                                                  ▼
                                         Ödeme Düzeni
                                                  │
                                                  ▼
                                            Para ₺ (tekrar)
```

**Döngü özeti:** Saygınlık → iyi kiracı → çok para → iyileştirme → mutluluk → düzenli ödeme → daha çok para → daha fazla iyileştirme → saygınlık artar. **Ama:** Her adımda kaynak harcamak gerekiyor ve olaylar bu döngüyü sürekli bozmaya çalışıyor.

#### Kira Sistemi

Kira miktarı **kiracı seviyesine** bağlıdır, daire kalitesine değil.

| Kiracı Seviyesi | Kira Aralığı | Gerekli Saygınlık | Karakter |
|-----------------|-------------|-------------------|----------|
| **Seviye 1** | 100-200₺ | ⭐ 0+ | Sorunlu, ucuz, çok talep |
| **Seviye 2** | 250-400₺ | ⭐ 21+ | Orta, dengeli |
| **Seviye 3** | 450-650₺ | ⭐ 51+ | İyi, az sorun, iyi öder |
| **Seviye 4** | 700-1000₺ | ⭐ 81+ | Nadir, özel yetenekli, yüksek kira |

> **Not:** Kira rakamları yer tutucudur — oyun dengesi testlerinde ayarlanır. Önemli olan oran ve yapıdır.

### 4.3 Kiracı Yönetimi

Kiracılar oyunun kalbidir. Her kiracı bir **yaratık** olup kendine özgü artıları, eksileri ve talepleri olan bir profildir.

#### Kiracı Tier Sistemi

Her kiracının bir **Tier seviyesi** vardır. Tier, kiracının kalitesini, kira miktarını ve apartmana etkisini belirler.

| Tier | Kira Aralığı | Gerekli ⭐ | Artılar | Eksiler |
|------|-------------|-----------|---------|---------|
| **Tier 1** | 100-200₺ | 0+ | Ucuz, kolay bulunur | Çok talep, düşük kira, üst tierleri mutsuz eder |
| **Tier 2** | 250-400₺ | 21+ | Dengeli, makul kira | Ara sıra sorun çıkarır |
| **Tier 3** | 450-650₺ | 51+ | İyi kira, az sorun | Beklentisi yüksek, istekleri pahalı |
| **Tier 4** | 700-1000₺ | 81+ | Çok iyi kira, özel bonuslar | Çok seçici, kolay mutsuz olur |

#### Kiracı Profil Kartı

Her kiracının emlakçıda ve apartmanda görünen bir profil kartı vardır:

- **Tür:** Yaratık türü (görsel + isim)
- **Tier:** 1-4 arası seviye
- **Kira:** Tier'e göre belirlenen sabit miktar
- **Artılar:** Apartmana pozitif etkiler (örn. "Gece güvenlik sağlar", "Komşularını neşelendirir")
- **Eksiler:** Apartmana negatif etkiler (örn. "Gürültücü", "Mobilya kırar", "Koku yapar")
- **Talepler:** Zaman zaman isteyecekleri şeyler (örn. "Daha sıcak oda istiyor", "Bahçede alan istiyor")

#### Kiracılar Arası Etkileşim

- **Tier uyumsuzluğu:** Düşük tier kiracılar yüksek tier kiracıları mutsuz eder. Bir Tier 4 kiracının yanına Tier 1 kiracı koymak = mutluluk kaybı.
- **Bu etki apartman genelinde hissedilir:** Tier karışımı, genel apartman mutluluğunu etkiler.
- **Stratejik ikilem:** Erken oyunda Tier 1 kiracıları almak zorundasın (saygınlık düşük), ama ilerledikçe onları Tier 2-3 ile değiştirmen gerekir. Tahliye bedeli var.

#### Kiracı Talepleri

Kiracılar belirli aralıklarla **talep** oluşturur. Talepler popup/kart olarak gün başında belirir.

- Her talep karşılanırsa → mutluluk artar
- Görmezden gelinirse → mutluluk düşer, tekrar talep + şikayet
- Üst üste karşılanmayan talepler → kiracı taşınma tehdidi
- Bazı talepler apartman yükseltmeleriyle otomatik karşılanır (örn. fiber optik bağlattıysan "internet yavaş" talebi gelmez)

### 4.4 Apartman Yükseltme Sistemi

> **Önemli:** Bu oyun daire yönetimi değil, **apartman yönetimidir.** Dairelerin içini yönetmiyoruz. Kiracıları dairelere yerleştiriyoruz ve **genel apartmanı** yükseltiyoruz.

#### Yükseltme Kategorileri

| Kategori | Örnek Yükseltmeler | Etki |
|----------|---------------------|------|
| **Dış Cephe** | Boya, cephe kaplama, tabela | ⭐ Saygınlık artışı |
| **Altyapı** | Tesisat yenileme, elektrik, kalorifer | 😊 Mutluluk + daha az arıza olayı |
| **Güvenlik** | Kamera, güvenlik kapısı, yangın alarm | ⭐ Saygınlık + olay koruması |
| **Konfor** | Asansör, fiber optik internet, klima | 😊 Mutluluk + talep azaltma |
| **Ortak Alan** | Bahçe düzenleme, otopark, çamaşırhane | ⭐ + 😊 karma etki |

#### Mahalle Dükkanları

Yükseltmeler **mahalle dükkanlarından** satın alınır. Oyuncu apartmandan çıkıp (UI olarak farklı bir ekran/panel) mahalledeki dükkanlara gider.

| Dükkan | Hizmetler | Örnek |
|--------|-----------|-------|
| **Boyacı** | Boya, cephe işleri | "Apartmanı boyat" — 3 gün, 500₺ |
| **Tesisatçı** | Boru, kalorifer, sıhhi tesisat | "Tesisat yenile" — 2 gün, 400₺ |
| **Elektrikçi** | Elektrik, internet, güvenlik sistemi | "Fiber optik bağlat" — 1 gün, 300₺ |
| **Bahçıvan** | Bahçe, çiçek, dış alan | "Bahçe düzenle" — 4 gün, 350₺ |
| **Mobilyacı** | Ortak alan mobilyaları | "Giriş mobilyası al" — anında, 200₺ |

> Dükkanlar oyun ilerledikçe artabilir veya yeni hizmetler açılabilir.

#### Yükseltme Süresi

Yükseltmeler **anında tamamlanmaz.** Her işin bir süresi vardır (gün bazlı).

- Boyacı çağırdın → 3 gün sonra biter
- Bu sürede boyacı apartmanda görünür (görsel geri bildirim)
- Süre boyunca ilgili alan kullanılamaz veya gürültü olur (mutluluk etkisi)
- Birden fazla iş aynı anda yürütülebilir (para yeterse)

### 4.5 Çalışan Sistemi

Apartmana kalıcı veya geçici **çalışanlar** tutulabilir.

| Çalışan | Maaş (günlük) | Etki |
|---------|---------------|------|
| **Kapıcı** | 50₺/gün | Küçük arızaları otomatik tamir eder, temizlik = mutluluk bonusu |
| **Güvenlikçi** | 75₺/gün | Hırsızlık/vandalizm olaylarını önler, saygınlık bonusu |
| **Bahçıvan** | 40₺/gün | Bahçe bakımı otomatik, dış görünüm bonusu |

> Çalışanlar opsiyoneldir. Para biriktirip çalışan tutmak uzun vadeli yatırımdır — günlük maaş ödersin ama olayları ve talepleri azaltır.

### 4.6 Olay / Karar Sistemi

Her gün rastgele veya hikayeye bağlı olaylar tetiklenir. Olaylar **zincirleme** çalışır — bazı kararların sonuçları günler sonra ortaya çıkar.

#### Olay Tipleri

| Tip | Açıklama | Sıklık |
|-----|----------|--------|
| **Günlük küçük olaylar** | Küçük sorunlar, komik durumlar | Her gün 1-3 |
| **Kiracı talepleri** | Kiracıların istekleri | Kiracı sayısına bağlı |
| **Büyük olaylar** | Ciddi kararlar, zincirleme sonuçlar | Haftada 1-2 |
| **Periyodik olaylar** | Vergi günü, belediye denetimi gibi tekrarlayan olaylar | Sabit aralıklarla (örn. 30 günde bir) |

#### Zincirleme Olay Sistemi

Bazı kararlar hemen sonuç verir, bazıları **birkaç gün sonra** etki eder. Bu, oyuncunun geçmiş kararlarının geri dönmesini sağlar.

**Örnek zincirleme olay:**

```
Gün 12: Blob kiracı "evde parti yapmak istiyor" → İzin ver / Reddet

  ├─ İzin ver →
  │   Gün 12: Mutluluk +5 (blob mutlu)
  │   Gün 13: Komşu şikayeti "gece gürültü oldu" → Özür dile / Görmezden gel
  │   │  ├─ Özür dile → -50₺ tazminat, komşu mutluluğu korunur
  │   │  └─ Görmezden gel → Komşu mutluluğu -10, şikayet devam eder
  │   Gün 15: Belediyeden gürültü uyarısı (saygınlık -3)
  │
  └─ Reddet →
      Gün 12: Blob mutluluğu -5
      Gün 14: Blob gizlice parti yapar → Daha büyük sorun (mutluluk -8, hasar)
```

#### Örnek Olaylar (Hibrit evren uyumlu)

- **Boru patlaması** → Tesisatçıyı çağır (pahalı, 1 gün) / Geçici çözüm (ucuz ama 3 gün sonra tekrar patlar)
- **Kiracılar arası kavga** → Arabuluculuk yap / Taraf tut / Görmezden gel (zincirleme)
- **Belediye denetimi** → 3 gün sonra denetim gelecek. O zamana kadar hazırlan (para harca) veya şansına bırak
- **Vergi günü** → 30 günde bir vergi gelir. Ödenmezse belediye uyarısı → mühürlenme riski
- **Yaratık büyüme krizi** → Sürekli büyüyen kiracı daireye sığmıyor. Büyük daireye taşı / Büyüme ilacı al / Tahliye et
- **Gizemli paket** → Apartmana paket geldi. Aç / Açma / Kiracıya ver (sürpriz sonuçlar)

---

## 5. İçerik & İlerleme Sistemi

### Oyun Yapısı: Sonsuz Sandbox

Oyun **sonsuz sandbox** yapıdadır. Net bir "oyun bitti" ekranı yoktur. Oyuncu istediği kadar devam eder. Ancak ilerleme döngüsü ~**4-6 saatlik** bir "ana döngü" etrafında tasarlanır:

- İlk 4-6 saatte tüm mekanikler açılır, tüm tier'lere erişilir, apartman büyütülür
- Sonrasında oyuncu optimizasyon, farklı kiracı kombinasyonları, yeni olaylar ve bina geliştirmeye devam eder
- Periyodik olaylar (vergi, belediye denetimi) sürekli gerilim yaratır

### İlk Giriş (Onboarding)

1. Avukat telefon sahnesi — kısa, hızlı, hikayeyi kurar
2. Apartmana ilk varış — bina harap, 2 kat, boş daireler
3. İlk mahalle turu — dükkanlar tanıtılır (boyacı, tesisatçı vb.)
4. Emlakçıya ilk ziyaret — ilk kiracıyı seç (tutorial)
5. İlk gün döngüsü — oyuncu serbest bırakılır

### İlerleme Aşamaları

| Aşama | Süre | Kat | Kiracı | Açılan Mekanikler |
|-------|------|-----|--------|-------------------|
| **Başlangıç** | Gün 1-10 (~1 saat) | 2 kat | 1-2 kiracı | Temel döngü, emlakçı, ilk dükkanlar |
| **Erken Oyun** | Gün 11-25 (~1.5 saat) | 2 kat | 3-4 kiracı | Tüm dükkanlar, ilk çalışan, yükseltmeler |
| **Orta Oyun** | Gün 26-50 (~1.5 saat) | 3 kat (ilk kat ekleme) | 5-7 kiracı | Tier 3 kiracılar, zincirleme olaylar, inşaatçı |
| **Geç Oyun** | Gün 50+ (~1+ saat) | 4-5 kat | 8+ kiracı | Tier 4 kiracılar, büyük olaylar, tam kaos |
| **Serbest Oyun** | Sınırsız | Max kat | Sınırsız | Her şey açık, sandbox devam |

### Kat Ekleme Mekaniği

Yeni katlar **inşaatçı dükkanından** (taş ustası) yaptırılır. Bu pahalı bir yatırımdır ve oyunun en büyük milestone'larından biridir.

| Kat | Maliyet | Süre | Gerekli ⭐ | Yeni Daire Sayısı |
|-----|---------|------|-----------|-------------------|
| **3. Kat** | 2000₺ | 5 gün | ⭐ 40+ | +2 daire |
| **4. Kat** | 4000₺ | 7 gün | ⭐ 60+ | +2 daire |
| **5. Kat** | 7000₺ | 10 gün | ⭐ 80+ | +2 daire |

> **İnşaat süresinde:** Gürültü olur (mutluluk düşer), para harcanır ama tamamlandığında büyük saygınlık ve gelir artışı.

**İnşaatçı dükkanı** mahalle dükkanlarına eklenir:

| Dükkan | Hizmetler |
|--------|-----------|
| **Taş Ustası / İnşaatçı** | Yeni kat ekleme, yapısal tamir, çatı onarımı |

### Kilit Açma Sırası (Unlock Sequence)

```
Gün 1:   Emlakçı + Boyacı + Tesisatçı açık
Gün 5:   Elektrikçi açılır
Gün 10:  İlk çalışan tutma hakkı (kapıcı)
Gün 15:  Bahçıvan dükkanı + Mobilyacı açılır
Gün 20:  Güvenlikçi tutma hakkı
Gün 25:  İnşaatçı dükkanı açılır (3. kat mümkün)
Gün 35:  Tier 3 kiracılar emlakçıda görünür (⭐ yeterliyse)
Gün 50:  4. kat mümkün + Tier 4 kiracılar
Gün 65+: 5. kat mümkün + nadir yaratıklar
```

> **Not:** Gün sayıları tahminidir, oyun dengesi testlerinde ayarlanır. Önemli olan sıralama ve akış hissidir.

### Tekrar Oynanabilirlik (Replayability)

Sandbox yapı doğal tekrar oynanabilirlik sağlar, ek olarak:
- **Farklı kiracı kombinasyonları:** Her oyunda farklı yaratıklar deneyebilirsin
- **Rastgele olay sistemi:** Olaylar her oyunda farklı sırada/kombinasyonda gelir
- **Farklı strateji denemeleri:** Hızlı büyüme vs yavaş kalite, düşük tier çok kiracı vs yüksek tier az kiracı

---

## 6. Görsel & Ses Yönü

### Görsel Stil: Basit & Renkli Cartoon

**Referanslar:** Adventure Time, Untitled Goose Game, Pikuniku tarzı — basit çizgiler, canlı renkler, abartılı ifadeler. Üretimi hızlı, komik tona çok uygun.

| Alan | Yaklaşım |
|------|----------|
| **Çizgi stili** | Kalın, temiz outline'lar. Minimal detay, maksimum okunabilirlik |
| **Renk paleti** | Sıcak ve canlı — turuncu, sarı, krem, açık yeşil. Her yaratık türü kendi renk tonunda |
| **Kamera** | 2D yan kesit — apartmanın tüm katları ve daireleri görünür |
| **Perspektif** | Binanın ortadan kesilmiş hali — duvarlar görünmez, iç mekanlar açık |
| **Arka plan** | Basit mahalle silueti, gökyüzü (gece/gündüz değişimi olabilir) |

### Karakter & Yaratık Tasarımı

- **Basit silüetler:** Her yaratık uzaktan bile tanınabilir olmalı (farklı şekil, boyut, renk)
- **Abartılı ifadeler:** Mutlu, kızgın, şaşkın yüz ifadeleri çok büyük ve okunabilir
- **Minimum animasyon karesi:** Idle, mutlu, mutsuz, talep (4 temel durum). Basit ama etkili
- **Komik kontrast:** Absürt yaratıklar normal ev eşyalarıyla etkileşirde (dev blob koltuğa oturmuş, ateş yaratığı terlik giymiş)

### Apartman Görselliği

- **Başlangıçta:** Soluk renkler, çatlak duvarlar, karanlık daireler
- **Yükseltildikçe:** Renkler canlanır, detaylar eklenir, ışıklar yanar
- **Görsel ilerleme hissi:** Oyuncunun yaptığı her yükseltme binada görsel olarak yansır (boya = duvar rengi değişir, bahçe = dışarıda çiçekler çıkar)

### Müzik: Lo-fi & Chill

Oyunun komik görselliğiyle kontrast oluşturan **rahat, modern, sakinleştirici** bir müzik tonu. Oyuncu kaotik olaylarla uğraşırken müzik onu sakin tutar — bu kontrast hem eğlenceli hem rahatlatıcıdır.

| Durum | Müzik Tonu |
|-------|-----------|
| **Normal gameplay** | Lo-fi hip hop / chillhop — yumuşak beat, piyano/gitar loop'ları |
| **Gün başı** | Kısa, neşeli jingle (yeni gün hissi) |
| **Olay anı** | Hafif tempo artışı, ama hâlâ chill — panik değil merak |
| **Gün sonu** | Yavaşlayan, dinlendirici melodi (gün bitti, rahatla) |
| **Emlakçı / Dükkanlar** | Farklı lo-fi varyasyonlar (her mekanın kendi havası) |

### Ses Efektleri

- **UI sesleri:** Yumuşak tıklama, sayfa çevirme, para sesi (tatmin edici)
- **Yaratık sesleri:** Her yaratık türünün basit, komik bir sesi (blob = "şlap", ateş yaratık = "cızz")
- **Olay sesleri:** Boru patlaması, çekiç, boya fırçası — karikatürize ama abartılı değil
- **Genel yaklaşım:** Sesler bilgi verir ve tatmin sağlar, ama dikkat dağıtmaz

---

## 7. UI/UX Tasarımı

### Ana Görünüm: Mahalle

Oyunun tek ana ekranı **mahalle görünümüdür.** 2D yan görünüm, sağa ve sola kaydırılabilir.

```
◄ SOL KAYDIR                                              SAĞ KAYDIR ►

  ┌─────────┐   ┌─────────────────────┐   ┌─────────┐
  │ Komşu   │   │                     │   │ Komşu   │
  │ Apartman │   │   BİZİM APARTMAN   │   │ Apartman │
  │         │   │  (ana oyun alanı)   │   │         │
  │         │   │                     │   │         │
  ├─────────┤   ├─────────────────────┤   ├─────────┤
  │ BOYACI  │   │      GİRİŞ          │   │EMLAKÇI  │
  └─────────┘   └─────────────────────┘   └─────────┘
      ▲                                        ▲
  Tıkla →                                 Tıkla →
  Modal açılır                            Modal açılır
```

- **Merkezde:** Bizim apartman — katlar, daireler, kiracılar görünür
- **Sol/sağda:** Komşu apartmanlar ve altlarında mahalle dükkanları
- **Dükkanlar:** Fiziksel olarak oyun dünyasında var. Tıklayınca **modal** olarak açılır (ekran değişmez, içine girilmez)
- **Kaydırma:** Mouse sürükleme veya ekran kenarlarına gelince otomatik kayma

### Dükkan Modal'ları

Her dükkan tıklandığında ekranın ortasına bir modal pencere açılır. Arka plan kararır. Modal içinde dükkanın hizmetleri listelenir.

| Dükkan | Modal İçeriği |
|--------|---------------|
| **Emlakçı** | Kiracı aday listesi (profil kartları), kabul/red butonları |
| **Boyacı** | Boya hizmetleri, fiyat, süre, "Sipariş Ver" butonu |
| **Tesisatçı** | Tesisat hizmetleri listesi |
| **Elektrikçi** | Elektrik/internet hizmetleri |
| **Bahçıvan** | Bahçe hizmetleri |
| **Mobilyacı** | Ortak alan mobilyaları |
| **Taş Ustası** | Yeni kat ekleme seçeneği (fiyat, süre, gereksinimler) |

### Apartman Etkileşimi

Apartmanın kendi iç görünümü ana oyun alanıdır:

- **Dairelere tıklama:** Kiracı profil kartı açılır (popup)
- **Kiracı talepleri:** Dairenin üstünde ünlem (!) ikonu belirir → tıkla → talep kartı
- **Yükseltme göstergeleri:** Devam eden işler binada görünür (boyacı, tesisatçı animasyonu)
- **Boş daireler:** "Boş" etiketi → tıklayınca emlakçıya yönlendirme

### HUD (Minimal)

Ekranın üst kısmında sürekli görünen minimal bilgi çubuğu:

```
┌─────────────────────────────────────────────────────────┐
│  ₺ 1.250    😊 72/100    ⭐ 55/100    │ GÜN 25 │ ⏭ Günü Bitir │
└─────────────────────────────────────────────────────────┘
```

- **Sol:** Para, Mutluluk, Saygınlık (sayısal)
- **Sağ:** Gün sayısı + "Günü Bitir" butonu
- Mutluluk ve saygınlık çubukları renk değiştirir (yeşil → sarı → kırmızı)

### Olay Gösterimi

Olaylar **popup kartları** olarak gün başında ekranın ortasına gelir:

- Kartın üstünde olay açıklaması (kısa, komik metin)
- Altında 2-3 seçenek butonu
- Oyuncu seçer → anlık veya zincirleme sonuç
- Birden fazla olay varsa sırayla gösterilir (kart destesi gibi)

### Gün Sonu Raporu

"Günü Bitir" butonuna basıldığında kısa bir özet ekranı:

```
┌─────────────────────────────────┐
│         GÜN 25 — ÖZET          │
│                                 │
│  Gelir:    +850₺  (kira)       │
│  Gider:    -350₺  (boyacı, fatura) │
│  Net:      +500₺               │
│                                 │
│  😊 Mutluluk:  72 → 68 (▼4)    │
│  ⭐ Saygınlık: 55 → 58 (▲3)    │
│                                 │
│  [ Sonraki Güne Geç → ]        │
└─────────────────────────────────┘
```

### Etkileşim Modeli

| Eylem | Giriş |
|-------|-------|
| Mahallede gezinme | Mouse sürükleme (sağ-sol) |
| Dükkan açma | Dükkana tıklama |
| Kiracı bilgisi | Daireye / kiracıya tıklama |
| Olay seçimi | Seçenek butonuna tıklama |
| Günü bitirme | HUD'daki butona tıklama |
| Modal kapatma | X butonu veya dışarı tıklama |

> Tüm etkileşimler **sol mouse tıklama** ile yapılır. Sağ tık veya klavye kısayolu gerektirmez. Basit ve erişilebilir.

---

## 8. Teknik Özet

| Alan | Detay |
|------|-------|
| **Motor** | Unity 2D |
| **Dil** | C# |
| **Hedef çözünürlük** | 1920x1080 |
| **Min. sistem** | Düşük sistem gereksinimleri (2D, hafif) |
| **Kayıt sistemi** | Lokal save (JSON) |
| **Hedef platform** | PC — Steam |
| **Hedef FPS** | 60 FPS |

### Ekip

| Rol | Kişi | Sorumluluk |
|-----|------|------------|
| **Game Designer** | 1 | Oyun tasarımı, denge, içerik, olay yazımı |
| **Senior Developer** | 1 | Mimari, core sistemler, araçlar |
| **Junior Developer** | 1 | UI, dükkan sistemi, olay sistemi, save/load |
| **Artist** | 1 | Tüm görseller — karakter, bina, UI, animasyon |

### Temel Teknik Sistemler

| Sistem | Açıklama |
|--------|----------|
| **Gün Döngüsü (Turn Manager)** | Gün başı → aksiyon → gün sonu akışını yöneten state machine |
| **Kaynak Sistemi** | Para, mutluluk, saygınlık takibi + kaynak değişim olayları |
| **Kiracı Sistemi** | Kiracı veritabanı, tier sistemi, talep üreteci, mutluluk hesaplayıcı |
| **Yükseltme Sistemi** | Apartman yükseltme listesi, süre takibi, görsel güncelleme |
| **Olay Sistemi** | Olay veritabanı, rastgele seçim, zincirleme olay takibi |
| **Dükkan Sistemi** | Dükkan modal'ları, hizmet listesi, sipariş yönetimi |
| **UI Sistemi** | HUD, modal'lar, popup kartlar, gün sonu raporu |
| **Save/Load** | JSON tabanlı kayıt — tüm oyun durumu serialize edilir |

---

## 9. Monetizasyon

- **Model:** Premium — tek seferlik satın alma (Steam)
- **DLC potansiyeli:** Yeni yaratık türleri, yeni mahalle dükkanları, ek olay paketleri
- **Oyun içi satın alım yok**
- **Reklam yok**

---

## 10. MVP Kapsam

### Yaklaşım: Tam Deneyim (Küçük)

MVP'de tüm mekanikler mevcut olacak ama küçük ölçekte. Oyuncu kısa ama **tam bir oyun deneyimi** yaşayacak.

### MVP İçerik Kapsamı

| Alan | MVP Kapsamı |
|------|-------------|
| **Apartman** | 2 kat, toplam 4 daire |
| **Kiracı türleri** | 6-8 farklı yaratık (Tier 1-3) |
| **Dükkanlar** | 3 dükkan (Emlakçı + Boyacı + Tesisatçı) |
| **Yükseltmeler** | 5-6 apartman yükseltmesi |
| **Olaylar** | 10-15 olay (5 basit + 5 zincirleme + 2-3 periyodik) |
| **Çalışanlar** | 1 çalışan türü (Kapıcı) |
| **Kat ekleme** | 1 yeni kat eklenebilir (2→3 kat) |

### Must-Have (MVP v1.0)

**Core Loop:**
- [ ] Mahalle görünümü (sağa-sola kayan 2D sahne)
- [ ] Apartman kesit görünümü (2 kat, 4 daire)
- [ ] Gün bazlı tur sistemi (gün başı → aksiyon → gün sonu)
- [ ] "Günü Bitir" butonu + gün sonu raporu
- [ ] Minimal HUD (para, mutluluk, saygınlık, gün sayısı)

**Kiracı Sistemi:**
- [ ] Kiracı profil kartları (tür, tier, artı/eksi, kira)
- [ ] Emlakçı dükkanı — kiracı aday listesi, kabul/red
- [ ] Kiracı talepleri (popup kartlar)
- [ ] Kiracı tahliye mekaniği
- [ ] Tier uyumsuzluğu → mutluluk etkisi

**Kaynak & Ekonomi:**
- [ ] Para (₺) sistemi — gelir/gider takibi
- [ ] Mutluluk (😊) sistemi — ödeme düzeni etkisi
- [ ] Saygınlık (⭐) sistemi — emlakçı kalitesi etkisi
- [ ] Fatura + vergi sistemi (periyodik giderler)
- [ ] Kaybetme koşulu: para = 0 → mühürlenme

**Apartman Yükseltme:**
- [ ] 3 dükkan modal sistemi (emlakçı, boyacı, tesisatçı)
- [ ] Yükseltme satın alma + süre sistemi
- [ ] Yükseltmelerin görsel yansıması

**Olay Sistemi:**
- [ ] 10-15 olay kartı (seçenekler + sonuçlar)
- [ ] Basit zincirleme olaylar (en az 3-5 tane)
- [ ] Vergi günü (30 günde bir)

**Teknik:**
- [ ] Kaydetme / yükleme (JSON)
- [ ] Başlangıç sahnesi (kısa hikaye anlatımı)

### Nice-to-Have (v1.0 sonrası güncellemeler)

- [ ] Ek yaratık türleri (Tier 4 dahil)
- [ ] Ek dükkanlar (elektrikçi, bahçıvan, mobilyacı, taş ustası)
- [ ] Kat ekleme mekaniği (tam sürüm: 2→5 kat)
- [ ] Çalışan sistemi (kapıcı, güvenlikçi, bahçıvan)
- [ ] Mevsim sistemi (kış = kalorifer sorunu vb.)
- [ ] Başarım (achievement) sistemi
- [ ] Daha fazla olay içeriği (25-30 olay)
- [ ] Steam entegrasyonu (bulut save, başarımlar)
- [ ] Ses & müzik (lo-fi soundtrack)
- [ ] Lokalizasyon (EN/TR)
