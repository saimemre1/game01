# Teknik Roadmap — Apartman

**Versiyon:** 1.0
**Tarih:** 2026-02-10
**Durum:** Aktif

---

## 1. Özet & Kritik Tarihler

### Timeline

```
  16 Şub          ~15 Nis        15 May        15 Haz    20 Haz
    │                │              │              │         │
    ▼                ▼              ▼              ▼         ▼
  ┌─────────────────────────────────────────────────────────────┐
  │ FAZ 1-3          │ FAZ 4       │ FAZ 5 │  FAZ 6            │
  │ Temel + Core +   │ İçerik &   │ DEMO  │  v1.0 Sprint      │
  │ Ana Sistemler    │ Entegrasyon│ TESLİM│  + Demo Polish     │
  └─────────────────────────────────────────────────────────────┘
       9 hafta          3 hafta    1 hafta     5 hafta
                    ▲                       ▲              ▲
                    │                       │              │
              Steam Sayfası           Next Fest       v1.0 Çıkış
                 Açılır              (15 Haz)        (20 Haz)
```

### Kritik Tarihler

| Tarih | Milestone | Not |
|-------|-----------|-----|
| **16 Şubat** | Geliştirme başlangıcı | İlk kodlar yazılır |
| **~15 Nisan** | Steam sayfası açılır | Trailer + 5 screenshot + açıklama |
| **15 Mayıs** | Demo Steam'e gönderilir | Next Fest başvurusu — minimum viable demo |
| **15 Mayıs → 15 Haziran** | Demo güncelleme dönemi | Patch'lerle demo iyileştirilir + v1.0 özellikleri paralel geliştirilir |
| **15 Haziran** | Steam Next Fest başlar | Demo herkese açık |
| **20 Haziran** | v1.0 tam sürüm çıkışı | Full game Steam'de satışa çıkar |

### Ekip & Roller

| Rol | Sorumluluk |
|-----|------------|
| **Game Designer (GD)** | Olay içeriği yazımı, denge ayarı, yaratık profilleri, playtest, Steam sayfası metinleri |
| **Senior Developer (Sr.)** | Mimari, core sistemler (gün döngüsü, kaynak, kiracı), araçlar, performans |
| **Junior Developer (Jr.)** | UI sistemleri, modal'lar, olay kartları, save/load, HUD, entegrasyon |
| **Artist (Art)** | Tüm görseller — apartman, yaratıklar, dükkanlar, UI, animasyonlar, trailer |

---

## 2. Demo Kapsamı (15 Mayıs — Next Fest Gönderimi)

Demo, oyunun core deneyimini gösteren **tam bir döngü**. Ufak tefek eksikler olabilir ama oyuncu "bu oyun ne" sorusunun cevabını net almalı.

### Demo'ya Girecekler

| Alan | Demo Kapsamı |
|------|-------------|
| **Mahalle** | 2D sağa-sola kayan görünüm (apartman + 2 komşu bina + 2 dükkan) |
| **Apartman** | 2 kat, 4 daire — yan kesit görünüm |
| **Dükkanlar** | Emlakçı + Boyacı (modal olarak açılır) |
| **Kiracılar** | 4-5 yaratık türü (Tier 1-2), profil kartları, talepler |
| **Core Loop** | Gün başı → aksiyon → gün sonu (tam tur bazlı) |
| **HUD** | Para (₺) + Mutluluk (😊) + Saygınlık (⭐) + Gün + Günü Bitir |
| **Olaylar** | 5-8 basit olay (anlık sonuç) |
| **Yükseltme** | Boyacı: bina boyama + görsel yansıma (renk değişimi) |
| **Kaybetme** | Para = 0 → uyarı → mühürlenme |
| **Gün sonu** | Özet raporu (gelir/gider/kaynak değişimi) |
| **Ses** | Temel UI ses efektleri (tıklama, para, olay bildirimi) |

### Demo'ya GİRMEYECEKLER (v1.0'a kalacak)

- Save/Load
- Zincirleme olaylar
- 3. dükkan (Tesisatçı)
- Çalışan sistemi (kapıcı)
- Kat ekleme mekaniği
- Onboarding/intro sahnesi
- Tier 3 kiracılar
- Vergi/fatura periyodik sistemi
- Yükseltme süre mekaniği (demo'da boyama anlık olabilir)
- Müzik (placeholder veya sessiz)

---

## 3. v1.0 Kapsamı (20 Haziran — Full Release)

Demo'nun üstüne eklenen özelliklerle tam oyun deneyimi.

### Demo → v1.0 Eklentileri

| Özellik | Açıklama |
|---------|----------|
| **Save/Load** | JSON tabanlı kayıt sistemi — oyunun tam durumu kaydedilir |
| **Tesisatçı dükkanı** | 3. dükkan — tesisat yükseltmeleri (mutluluk + arıza azaltma) |
| **Yükseltme süresi** | İşler gün bazlı sürer (boyacı 3 gün, tesisatçı 2 gün) |
| **Zincirleme olaylar** | 5-7 zincirleme olay (kararlar günler sonra geri döner) |
| **Ek yaratıklar** | +2-3 yaratık türü (Tier 3 dahil). Toplam 6-8 yaratık |
| **Kapıcı** | İlk çalışan — küçük arızaları otomatik tamir, maaşlı |
| **Kat ekleme** | Taş ustası dükkanı — 3. kat yaptırma (2→3 kat, +2 daire) |
| **Onboarding** | Avukat telefon sahnesi → ilk varış → tutorial (ilk kiracı) |
| **Vergi/fatura** | Periyodik giderler — haftalık fatura, 30 günlük vergi |
| **Ses & Müzik** | Lo-fi soundtrack, yaratık sesleri, olay ses efektleri |

---

## 4. Haftalık Roadmap

### Faz 1 — Temel & Mimari (H1-H3: 16 Şub → 8 Mar)

Projenin iskeletini kurmak. Hiçbir şey "güzel" olmak zorunda değil, ama yapı sağlam olmalı.

#### Hafta 1 (16-22 Şub)

| Rol | Görev |
|-----|-------|
| **Sr.** | Unity proje kurulumu, klasör yapısı, Git repo, temel mimari kararları (ScriptableObject vs JSON data) |
| **Jr.** | Unity editör tanıma, GDD okuma, basit UI framework araştırması (Canvas setup) |
| **Art** | Stil rehberi oluşturma: renk paleti, çizgi kalınlığı, karakter ölçeği. İlk apartman dış cephe sketch |
| **GD** | Yaratık profilleri detaylandırma (4-5 yaratık: isim, tier, artı/eksi, talepler, görsel brief) |
| **Teslim:** | Unity projesi çalışır durumda, Git aktif, stil rehberi hazır |

#### Hafta 2 (23 Şub — 1 Mar)

| Rol | Görev |
|-----|-------|
| **Sr.** | Apartman veri modeli (kat, daire, kiracı slot), kaynak sistemi data yapısı (para, mutluluk, saygınlık) |
| **Jr.** | Basit HUD prototipi (3 kaynak göstergesi + gün sayacı), Canvas layout |
| **Art** | Apartman kesit sprite'ı (2 kat, 4 daire — placeholder renklerde). Daireler ayrı ayrı slot olarak |
| **GD** | İlk 5 olay kartı yazımı (metin + seçenekler + kaynak etkileri) |
| **Teslim:** | Ekranda apartman görünür (statik), HUD placeholder çalışır |

#### Hafta 3 (2-8 Mar)

| Rol | Görev |
|-----|-------|
| **Sr.** | Kiracı veri modeli (ScriptableObject: tür, tier, kira, artı/eksi, talepler). Kiracı havuzu (pool) |
| **Jr.** | Dairelere tıklama → popup açma prototipi. Modal sistem altyapısı (açma/kapama/arka plan karartma) |
| **Art** | İlk 2 yaratık sprite'ı (idle + mutlu + mutsuz). Profil kartı UI tasarımı |
| **GD** | Kira değerleri ve ekonomi dengesi ilk taslağı. Tier 1-2 kiracı parametreleri |
| **Teslim:** | Kiracı data modeli çalışır, modal altyapısı hazır, 2 yaratık sprite var |

> **Faz 1 Sonu Deliverable:** Ekranda apartman kesiti var, HUD çalışır (statik değerlerle), dairelere tıklanabilir, modal açılıp kapanır, 2 yaratık sprite hazır.

---

### Faz 2 — Core Loop (H4-H6: 9 Mar → 29 Mar)

Oyunun kalbi burada atıyor. Gün döngüsü + kaynaklar + kira sistemi çalışmalı.

#### Hafta 4 (9-15 Mar)

| Rol | Görev |
|-----|-------|
| **Sr.** | Gün döngüsü state machine (GünBaşı → Aksiyon → GünSonu). Turn Manager sınıfı |
| **Jr.** | "Günü Bitir" butonu + gün geçiş animasyonu/transition. Gün sayacı HUD'da çalışır |
| **Art** | +2 yaratık sprite'ı (toplam 4). Apartman iç detayları (daire mobilyaları, ışıklar) |
| **GD** | +3 olay kartı yazımı (toplam 8). Olay zorluk/sıklık dengesi taslağı |
| **Teslim:** | "Günü Bitir"e basınca yeni güne geçilir, gün sayacı artar |

#### Hafta 5 (16-22 Mar)

| Rol | Görev |
|-----|-------|
| **Sr.** | Kaynak sistemi implementasyonu — para/mutluluk/saygınlık runtime'da çalışır. Kira geliri hesaplama (gün başı otomatik) |
| **Jr.** | HUD'da kaynaklar canlı güncelleniyor. Kaynak değişim animasyonu (+50₺ ↑, -10😊 ↓). Gün sonu raporu ekranı |
| **Art** | Mahalle arka planı (komşu binalar silueti, gökyüzü). İlk dükkan dış cephe tasarımı (emlakçı) |
| **GD** | Playtest — gün döngüsü hissi, kira/gider dengesi. Mutluluk → ödeme davranışı kuralları |
| **Teslim:** | Kaynak sistemi çalışır, kira toplanır, HUD canlı, gün sonu raporu gösterilir |

#### Hafta 6 (23-29 Mar)

| Rol | Görev |
|-----|-------|
| **Sr.** | Kiracı yerleştirme sistemi — daireye kiracı atama, kira başlatma. Mutluluk/saygınlık hesaplama döngüsü |
| **Jr.** | Kiracı profil kartı UI — daireye tıklayınca açılır (tür, tier, kira, artı/eksi). Boş daire göstergesi |
| **Art** | Emlakçı dış cephe finalize. İlk yaratık animasyonları (idle loop, 4 yaratık). **Steam sayfası: logo + ilk mockup screenshot'lar** |
| **GD** | Tier 1 vs Tier 2 deneyim farkı testi. Mutluluk eşik değerleri ayarı. **Steam sayfası açıklama metni taslağı** |
| **Teslim:** | Kiracı daireye yerleşir, kira öder, profil kartı görünür. Steam asset'leri hazırlanmaya başladı |

> **Faz 2 Sonu Deliverable:** Core loop çalışır — gün geçer, kira toplanır, kaynaklar güncellenir, gün sonu raporu gösterilir. Ama henüz kiracı seçme veya olay yok.

---

### Faz 3 — Ana Sistemler (H7-H9: 30 Mar → 19 Nis)

Kiracı seçimi, olaylar ve mahalle görünümü. Oyun burada "oyun" olmaya başlıyor.

#### Hafta 7 (30 Mar — 5 Nis)

| Rol | Görev |
|-----|-------|
| **Sr.** | Emlakçı sistemi — aday havuzu üretimi (saygınlığa göre), aday listesi refresh mekaniği |
| **Jr.** | Emlakçı modal UI — aday kartları listesi, "Kabul" / "Reddet" butonları. Kabul → daireye yerleştir |
| **Art** | 5. yaratık sprite'ı (toplam 5). Boyacı dükkan dış cephe tasarımı. Olay kartı UI tasarımı |
| **GD** | Emlakçı aday havuzu kuralları: saygınlık eşikleri, Tier dağılımı, refresh süresi |
| **Teslim:** | Emlakçıya gidilir, aday listesi görülür, kiracı seçilip daireye yerleştirilir |

#### Hafta 8 (6-12 Nis)

| Rol | Görev |
|-----|-------|
| **Sr.** | Olay sistemi motoru — olay veritabanından rastgele seçim, gün başı tetikleme, kaynak etkisi uygulama |
| **Jr.** | Olay kartı UI — popup kart (metin + 2-3 seçenek butonu), seçim sonrası kaynak gösterimi. Birden fazla olay sıralaması |
| **Art** | Olay kartı görselleri (arka plan, ikonlar). Mahalle scroll sahne düzeni (komşu binalar + dükkanlar yerleşimi) |
| **GD** | 5 olayı sisteme girme (data olarak). Playtest — olay sıklığı ve etki dengesi |
| **Teslim:** | Gün başında olay kartı çıkar, oyuncu seçim yapar, kaynaklar etkilenir |

#### Hafta 9 (13-19 Nis)

| Rol | Görev |
|-----|-------|
| **Sr.** | Kiracı talep sistemi — kiracılar belirli aralıklarla talep oluşturur. Talep karşılama/görmezden gelme mekaniği |
| **Jr.** | Mahalle scroll implementasyonu — kamera sağa sola kayar. Dükkan tıklama → modal. Talep ikonu (!) daire üstünde |
| **Art** | Tüm dükkan cepheler finalize. Kiracı talep ikonları. **Steam sayfası: 5 screenshot + kısa trailer (30s gameplay capture)** |
| **GD** | Kiracı talep listesi oluşturma (tier'e göre). Karşılama maliyetleri + mutluluk etkileri. **Steam sayfası son kontrol** |
| **Teslim:** | Mahalle scroll çalışır, dükkanlar tıklanır, kiracı talepleri gelir. **→ Steam sayfası açılır** |

> **Faz 3 Sonu Deliverable:** Oynanabilir oyun! Emlakçıdan kiracı al, olaylarla uğraş, talepleri karşıla, kaynakları yönet. Mahalle scroll çalışır. Steam sayfası yayında.

---

### Faz 4 — İçerik & Entegrasyon (H10-H12: 20 Nis → 10 May)

Demo kalitesine getirmek. İçerik ekleme, boyacı sistemi, denge, polish.

#### Hafta 10 (20-26 Nis)

| Rol | Görev |
|-----|-------|
| **Sr.** | Yükseltme sistemi altyapısı — yükseltme data modeli, satın alma, apartmana uygulama. Boyacı: renk değişim mekaniği |
| **Jr.** | Boyacı modal UI — hizmet listesi, fiyat, "Sipariş Ver". Yükseltme sonrası apartman sprite değişimi tetikleme |
| **Art** | Apartmanın boyalı/boyasız varyantları (2-3 renk seçeneği). Yükseltme öncesi/sonrası görsel fark |
| **GD** | Boyacı fiyatlandırması. +3 olay yazımı ve sisteme girme (toplam 8). Tahliye mekaniği kuralları |
| **Teslim:** | Boyacıya gidilir, boya seçilir, apartman rengi değişir |

#### Hafta 11 (27 Nis — 3 May)

| Rol | Görev |
|-----|-------|
| **Sr.** | Kaybetme koşulu implementasyonu (para=0 → uyarı → 3 gün → mühürlenme). Tier uyumsuzluğu → mutluluk etkisi |
| **Jr.** | Kaybetme ekranı UI. Kiracı tahliye UI + onay modalı. Genel bug fix ve UI polish |
| **Art** | Mühürlenme görseli. UI polish — buton hover efektleri, tooltip'ler. Kiracı talep karşılama animasyonu |
| **GD** | Tam playtest — 30 dakika demo session testi. Denge ayarları: başlangıç parası, kira değerleri, olay sıklığı |
| **Teslim:** | Kaybetme çalışır. Oyun baştan sona oynanabilir (demo seviyesinde) |

#### Hafta 12 (4-10 May)

| Rol | Görev |
|-----|-------|
| **Sr.** | Demo-spesifik: giriş ekranı (başla butonu), demo sınırlamaları (gün limiti veya serbest?). Performans kontrolü |
| **Jr.** | Ana menü (Yeni Oyun + Çıkış). Temel ses entegrasyonu (UI tıklama sesleri, para sesi, olay sesi). Son bug fix |
| **Art** | Ana menü görseli / arka plan. Logo finalize. Son görsel polish. Eksik sprite'lar tamamlanır |
| **GD** | Final playtest. Demo akış testi (ilk açılış → 15-20 dk oynama). Denge son ayarları |
| **Teslim:** | Demo build-ready. Tüm core özellikler çalışır ve cilalı |

> **Faz 4 Sonu Deliverable:** Demo build'e hazır oyun. Core loop + 2 dükkan + 5 yaratık + 8 olay + boyacı yükseltme + kaybetme + minimal ses.

---

### Faz 5 — Demo Teslim (H13: 11-15 May)

#### Hafta 13 (11-15 May) — DEMO MILESTONE

| Rol | Görev |
|-----|-------|
| **Sr.** | Demo build oluşturma, Steamworks SDK entegrasyonu, build test (farklı bilgisayarlarda) |
| **Jr.** | Son bug fix, Steamworks upload desteği |
| **Art** | Demo store görselleri (capsule image, header image) |
| **GD** | Demo'yu Steam'e gönderme süreci, store sayfası demo butonu aktif etme |

**→ Demo Steam'e gönderilir. Next Fest başvurusu tamamlanır.**

---

### Faz 6 — v1.0 Sprint (H14-H18: 16 May → 20 Haz)

Demo gönderildikten sonra hem demo'yu güncelliyoruz hem v1.0 özelliklerini ekliyoruz.

#### Hafta 14 (16-22 May)

| Rol | Görev |
|-----|-------|
| **Sr.** | Save/Load sistemi (JSON serialize — tüm oyun durumu: kaynaklar, kiracılar, daireler, aktif olaylar, gün sayısı) |
| **Jr.** | Save/Load UI (kaydet butonu HUD'a, yükle seçeneği ana menüye). Tesisatçı modal UI |
| **Art** | Tesisatçı dükkan cephesi. +1-2 yaratık sprite (Tier 3 yaratıklar). Kat ekleme görsel konsepti |
| **GD** | Zincirleme olay ağaçları yazımı (3-5 zincirleme olay). Tesisatçı hizmet listesi ve fiyatlandırma |
| **Teslim:** | Save/Load çalışır. Tesisatçı modal'ı hazır |

#### Hafta 15 (23-29 May)

| Rol | Görev |
|-----|-------|
| **Sr.** | Zincirleme olay motoru — olay sonucunun X gün sonra yeni olay tetiklemesi. Yükseltme süre sistemi (gün bazlı ilerleme) |
| **Jr.** | Tesisatçı yükseltmelerinin görsel yansıması. Süre göstergesi UI (devam eden işler). Demo patch #1 hazırlığı |
| **Art** | Yükseltme animasyonları (boyacı/tesisatçı çalışırken). Kat ekleme inşaat görselleri (iskele, tuğla) |
| **GD** | Zincirleme olayları sisteme girme ve test. Yükseltme süresi denge ayarı. **Demo Patch #1 gönderimi** |
| **Teslim:** | Zincirleme olaylar çalışır. Yükseltme süresi çalışır. Demo güncellendi |

#### Hafta 16 (30 May — 5 Haz)

| Rol | Görev |
|-----|-------|
| **Sr.** | Kat ekleme mekaniği — 3. kat yapım süreci, yeni daire slot'ları, inşaat durumu. Taş ustası dükkan sistemi |
| **Jr.** | Taş ustası modal UI. Çalışan sistemi UI (kapıcı tutma/çıkarma). Onboarding sahnesi (kısa hikaye sequence) |
| **Art** | 3. kat sprite'ları (inşaat hali + tamamlanmış hali). Kapıcı karakter sprite. Onboarding görselleri |
| **GD** | Kat ekleme fiyat/süre dengesi. Kapıcı maaş/fayda dengesi. Onboarding metin yazımı |
| **Teslim:** | Kat ekleme çalışır. Kapıcı tutulabilir. Onboarding sahnesi var |

#### Hafta 17 (6-12 Haz)

| Rol | Görev |
|-----|-------|
| **Sr.** | Periyodik giderler (haftalık fatura, 30 günlük vergi). Son yaratık türleri entegrasyonu. Performans optimizasyonu |
| **Jr.** | Ses & müzik entegrasyonu (lo-fi tracks + yaratık sesleri + olay sesleri). **Demo Patch #2 gönderimi** |
| **Art** | Son yaratık sprite'ları finalize. Vergi/fatura olay kartı görselleri. Genel visual polish |
| **GD** | Tam oyun playtest (baştan sona 4-6 saat). Ekonomi son denge ayarı. Fatura/vergi rakamları |
| **Teslim:** | Tüm v1.0 özellikleri entegre. Ses/müzik var. Demo son güncelleme |

#### Hafta 18 (13-20 Haz) — v1.0 MILESTONE

| Rol | Görev |
|-----|-------|
| **Sr.** | v1.0 build. Kritik bug fix. Steamworks tam entegrasyon (başarımlar opsiyonel) |
| **Jr.** | Son bug fix. Build test. Farklı çözünürlük testi |
| **Art** | Store görselleri güncelleme (v1.0 screenshots). Varsa son görsel eksikler |
| **GD** | v1.0 store sayfası güncelleme. Çıkış duyurusu hazırlığı. Son playtest |

**→ 15 Haziran: Next Fest başlar (demo herkese açık)**
**→ 20 Haziran: v1.0 Steam'de satışa çıkar**

---

## 5. Best Case / Worst Case

### Best Case Senaryo

Demo Faz 4'ün ortasında (H11) build-ready olur. 2 hafta buffer kazanılır.

**Ekstra kazanımlar:**
- Demo'ya sesler/müzik dahil edilir
- Demo'ya basit save/load eklenir
- v1.0'a ek özellikler girer: mevsim sistemi veya başarımlar
- Steam sayfası daha erken açılır (Mart sonu)
- Daha çok playtest zamanı → daha iyi denge

### Worst Case Senaryo

Her faz ~1 hafta kayar. Yetişmeyen özellikler öncelik sırasına göre kesilir.

**Kesilme sırası (en az kritikten en kritiğe):**

| Sıra | Özellik | Etki | Ne olur kesilirse |
|------|---------|------|-------------------|
| 1 | Müzik | Düşük | Sessiz oyun veya free placeholder müzik kullanılır |
| 2 | Onboarding sahnesi | Düşük | Oyuncu direkt oyuna girer, hikaye anlatılmaz |
| 3 | Çalışan sistemi (kapıcı) | Orta | Oyun hâlâ çalışır, bir mekanik katmanı eksik kalır |
| 4 | Kat ekleme | Orta | Oyun 2 katta kalır. Daha kısa ama tam bir deneyim |
| 5 | Tesisatçı dükkanı | Orta-Yüksek | Sadece 2 dükkan (emlakçı + boyacı). Core çalışır ama çeşitlilik azalır |
| 6 | Zincirleme olaylar | Yüksek | Sadece basit olaylar kalır. Oyun daha sığ hisseder |

> **Kural:** Core loop (gün döngüsü + kiracı + kaynaklar + emlakçı + boyacı + basit olaylar + kaybetme) asla kesilmez. Bu oyunun minimum viable product'ıdır.

### "Red Line" — Kesinlikle Yetişmeli

Hem demo hem v1.0 için **kesintiye uğramaması gereken** özellikler:

- Gün döngüsü (turn-based core loop)
- Kaynak sistemi (para/mutluluk/saygınlık)
- Emlakçı + kiracı seçimi
- En az 1 yükseltme dükkanı (boyacı) + görsel yansıma
- En az 5 olay
- En az 4 yaratık türü
- Kaybetme koşulu
- Save/Load (v1.0 için)

---

## 6. Riskler & Önlemler

| Risk | Olasılık | Etki | Önlem |
|------|----------|------|-------|
| **Sanat darboğazı** — tek artist, çok asset | Yüksek | Yüksek | Basit cartoon stil zaten hızlı üretimi destekler. Kritik asset'lere öncelik ver. Gerekirse UI için free asset kit kullan |
| **Olay içeriği gecikmesi** — GD olay yazımında yavaş kalması | Orta | Orta | Olay sistemi data-driven olmalı — GD spreadsheet'te yazar, developer sadece import eder. Paralel çalışma |
| **Unity teknik sorunlar** — beklenmedik engine bug'ları | Düşük | Yüksek | Sr. developer ilk 2 haftada mimariyi sağlam kursun. Haftalık build yapılsın |
| **Denge ayarı sonsuz döngüye girmesi** — "bir sayıyı değiştirince her şey bozuluyor" | Orta | Orta | Ekonomi parametreleri ScriptableObject veya JSON'da olsun — code change gerektirmeden ayarlanabilsin |
| **Steam sayfası gecikme** — trailer/screenshot hazır olmaması | Düşük | Orta | H6'da (Mart sonu) basit gameplay capture yeterli. Profesyonel trailer gerekmez |
| **Ekip motivasyon kaybı** — yoğun tempo, 18 hafta sprint | Orta | Yüksek | Her faz sonunda çalışan build = motivasyon. Haftalık kısa playtest session'ları = herkes oyunu oynar |

---

## Haftalık Kontrol Listesi

Her hafta Cuma günü ekip şu soruları cevaplar:

- [ ] Bu haftanın deliverable'ı tamamlandı mı?
- [ ] Bir sonraki haftayı bloke eden bir şey var mı?
- [ ] Build alınabilir durumda mı? (H4'ten itibaren)
- [ ] Timeline'da kayma var mı? Varsa nerede telafi edilecek?
