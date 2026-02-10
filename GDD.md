# Game Design Document — Apartman

**Versiyon:** 0.1
**Tarih:** 2026-02-09
**Durum:** Taslak

---

## 1. Oyun Özeti

| Alan | Detay |
|------|-------|
| **Oyun Adı** | Apartman (çalışma adı) |
| **Pitch** | Büyükannesinden miras kalan eski bir apartmanı ayağa kaldırmaya çalışan İlkkan'ın hikayesi — bir apartman yönetim simülasyonu. |
| **Tür** | Management Simulation / Tycoon |
| **Platform** | PC (Steam) |
| **Motor** | Unity |
| **Kamera** | 2D side-view (platformer tarzı kesit görünüm) |
| **Kontrol** | Mouse — tıklama tabanlı (karakter hareketi yok) |
| **Sanat Stili** | Cartoon / Hand-drawn |
| **Gelir Modeli** | Premium (tek seferlik satın alma) |
| **Hedef Kitle** | Yönetim/simülasyon seven casual-midcore oyuncular |

---

## 2. Konsept ve Hikaye

### Kısa Hikaye

Bir baltaya sap olamayan **İlkkan**, bir gün telefonla aranır. Arayan bir avukattır. Yıllardır görüşmediği büyükannesi vefat etmiştir. Vasiyet olarak İlkkan'a eski aile apartmanını bırakmıştır — apartmanı işletmesi ve **asla satmaması** şartıyla.

Etrafta tüm arsalar satılmış, gökdelenler yükselmiştir. Ama bu sıcak ve eski apartmanı tekrar adam etmek çok zordur. İlkkan hayatında yeni bir amaç bulmuştur.

Bir apartman yönetmek kolay görünse de, başına geleceklerden habersizdir. Ve olaylar gelişir...

### Oyuncu Fantezisi

Oyuncu, harap bir binayı adım adım yaşanılır bir yuvaya dönüştürmenin, kiracılarla ilişkiler kurmanın ve mahallede saygınlık kazanmanın tatminini yaşar.

---

## 3. Temel Mekanikler

### 3.1 Core Loop (Günlük Döngü)

```
  ┌──────────────────────────────────────────────┐
  │                 GÜN BAŞI                      │
  │         Yeni olaylar & kiracı talepleri        │
  └──────────────┬───────────────────────────────┘
                 ▼
  ┌──────────────────────────────────────────────┐
  │              AKSİYON FAZÍ                     │
  │  • Kiracı taleplerini çöz                     │
  │  • Tamir / yenileme yap                       │
  │  • Olaylarda karar ver                        │
  │  • Kira topla / harcama yap                   │
  └──────────────┬───────────────────────────────┘
                 ▼
  ┌──────────────────────────────────────────────┐
  │               GÜN SONU                        │
  │  Kaynaklar güncellenir (Para, Mutluluk,       │
  │  Saygınlık). Sonraki güne geçilir.            │
  └──────────────┬───────────────────────────────┘
                 │
                 └──────────► Yeni güne dön
```

### 3.2 Kaynak Sistemi

| Kaynak | Açıklama | Kazanım | Harcama |
|--------|----------|---------|---------|
| **Para (₺)** | Ana ekonomik kaynak | Kira gelirleri, etkinlikler | Tamir, yenileme, mobilya, faturalar |
| **Mutluluk (😊)** | Kiracıların genel memnuniyeti | Talepleri çözmek, iyileştirmeler | İhmal, kötü kararlar, olaylar |
| **Saygınlık (⭐)** | Apartmanın mahalle itibarı | İyi yönetim, dış görünüm | Skandallar, bakımsızlık |

- **Mutluluk düşerse:** Kiracılar şikayet eder, taşınma tehdidi, kira ödememezlik.
- **Saygınlık düşerse:** Yeni kiracı bulmak zorlaşır, belediye baskısı artar.
- **Para biterse:** Tamir yapılamaz, faturalar ödenmez → kısır döngü.

### 3.3 Kiracı Yönetimi

- **Kiracı kabul:** Başvuran kiracılar arasından seçim (her kiracının profili, ödeme gücü, karakter özellikleri).
- **Kira toplama:** Her gün/hafta otomatik veya tıklamalı kira geliri.
- **Şikayet çözme:** Kiracılar sorun bildirir → oyuncu çözüm seçer.
- **Tahliye:** Sorunlu kiracıları çıkarma (mutluluk/saygınlık etkisi).

### 3.4 Bina Tamir ve Geliştirme

- **Oda tamiri:** Hasar görmüş odaları onarma.
- **Yenileme:** Mobilya, boya, tesisat yükseltme.
- **Ortak alan iyileştirme:** Merdiven, giriş, çatı, bahçe.
- **Yeni kat ekleme:** Bina büyütme (ileri seviye).

### 3.5 Olay / Karar Sistemi

Her gün rastgele veya hikayeye bağlı olaylar tetiklenir. Oyuncu seçim yapar, her seçimin kaynaklara etkisi vardır.

**Örnek olaylar:**
- Boru patlaması → Hemen tamir et (pahalı) / Geçici çözüm (ucuz ama mutluluk düşer)
- Komşu kavgası → Arabuluculuk yap / Taraf tut / Görmezden gel
- Belediye denetimi → Hazırlık yap (para) / Şansına bırak (risk)
- Gökdelen şirketi teklif → Satmayı reddet (hikaye gereği) ama baskı artar

---

## 4. Oyun Akışı

### İlk Giriş (Onboarding)
1. Avukat telefon sahnesi (hikaye anlatımı)
2. Apartmana ilk varış — bina harap durumda
3. İlk oda tamiri (tutorial)
4. İlk kiracı kabul (tutorial)
5. İlk gün döngüsü — oyuncu serbest bırakılır

### İlerleme
- **Erken oyun:** 1-2 kiracı, temel tamir, para sıkıntısı.
- **Orta oyun:** 4-6 kiracı, olay çeşitliliği artar, bina genişler.
- **Geç oyun:** Dolu apartman, büyük olaylar, gökdelen baskısı dorukta.

---

## 5. Görsel Yön

- **Stil:** Cartoon / hand-drawn, sıcak ve samimi çizgiler.
- **Kamera:** Binanın yan kesit görünümü — her oda/daire görünür (platformer kesiti).
- **Renk paleti:** Sıcak tonlar (turuncu, sarı, krem) — gökdelenler soğuk gri/mavi tonlarla kontrast.
- **Karakter tasarımı:** Abartılı, karikatürize kiracı tipleri.

---

## 6. Teknik Özet

| Alan | Detay |
|------|-------|
| **Motor** | Unity 2D |
| **Dil** | C# |
| **Hedef çözünürlük** | 1920x1080 |
| **Min. sistem** | Düşük sistem gereksinimleri (2D, hafif) |
| **Kayıt sistemi** | Lokal save (JSON veya binary) |

---

## 7. Monetizasyon

- **Model:** Premium — tek seferlik satın alma (Steam).
- **DLC potansiyeli:** Yeni hikaye bölümleri, yeni bina tipleri (gelecek planı).
- **Oyun içi satın alım yok.**
- **Reklam yok.**

---

## 8. MVP Kapsam

### Must-Have (v1.0)
- [ ] Apartman kesit görünümü (3-4 kat)
- [ ] Gün bazlı tur sistemi
- [ ] Kiracı kabul / tahliye mekaniği
- [ ] Temel oda tamir / yenileme
- [ ] Para, mutluluk, saygınlık kaynakları
- [ ] 10-15 temel olay / karar
- [ ] Basit hikaye akışı (başlangıç + son)
- [ ] Kaydetme / yükleme

### Nice-to-Have (sonraki güncellemeler)
- [ ] Yeni kat ekleme mekaniği
- [ ] Kiracı ilişkileri / diyalog sistemi
- [ ] Mevsim sistemi (kış = kalorifer sorunu vb.)
- [ ] Başarım (achievement) sistemi
- [ ] Steam Workshop desteği (mod)
- [ ] Çoklu bina yönetimi
