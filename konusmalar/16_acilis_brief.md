# TRADIA — KONUŞMA #16 AÇILIŞ BRİEFİ

**Açılış tarihi:** 2026-07-10 (Tradia-15 kapanışıyla eş-zamanlı)
**Otorite:** CC-Hafıza (B9) hazırladı, Patron açış
**Referans:** [15_genis_ozet.md](./15_genis_ozet.md) · [ozet.json](../vezir/ozet.json) · Tradia standing v1.7 (19 kural) + B1-B10

---

## 1. AÇILIŞTA İLK 3 DEVİR PROMPT

### PROMPT #1 — CC-BORSA S50 tetik
Basın S43+ çıktısı `02_CC_STATE/basin_reviews_dir` + `basin_cikti/` altında hazır. Borsa S37'de tetik bildirimi aldı (`hafiza_tetik_ccborsa_s37.json`) ama S38-S39 sessiz. **S50'de zorunlu geri bildirim** — yeni symlink yolları okundu mu, ne kadar kayıt okundu, filtre (sirket_eslesme + materyallik∈{yüksek,orta}) uygulandı mı. Sessizse 3. sprint alarmı → VAKA açılır (Standing #7 + B1).

### PROMPT #2 — CC-BASIN S50 çift-tier ilk regres
S38'de haber_semasi v1.2 canonize + `guvenilir_flag` ENUM {yuksek, orta, null} kanona alındı. Basın S47+ emisyonu yeni tanımla akıyor. **S50 kapanışında zorunlu 2 tier ayrı 20-örneklem regres testi:** yuksek tam-doğru % (hedef ≥80), orta tam-doğru % (hedef ≥60), orta yarı-doğru-dahil % (hedef ≥80). Standing #17 uzantısı disiplini — 2 sprint art arda kırılırsa Standing #17 REVİZE.

### PROMPT #3 — CC-TT-AI TTA70 3-karar uygulama raporu
S38'de 3 B9 kararı TT-AI'a iletildi (`hafiza_bildirim_cctt_ai_s38.json`): (1) YAPISAL_TAMAM (C) yolu → Kocaeli 19/19 betimsel-thin sonrası ≥2 yapısal DOLU mahalle yeniden-say; (2) Standing #18 üçlü-anahtar → grounded pipeline ilk kapı; (3) çift-tier guvenilir_flag → yuksek+orta grounded pipeline'da. **TTA70 raporunda beklenen:** ölçüm tablosu v1.2 (yeni kolonlar: YAPISAL_TAMAM · üçlü-anahtar-eksik-reddedilen · guvenilir_flag dağılımı) + Kocaeli %15 walled eşiği güncel yüzde.

---

## 2. BEKLEYEN KARAR KUYRUĞU (5 madde)

| # | Karar | Kaynak | Beklenti |
|---|---|---|---|
| **K2** | Sosyal S150 Madde 1-3 detay | TTA-Sosyal köprü | Sosyal yanıtı bekleniyor |
| **K3** | TT-AI auto kalite-gate v2 | TTA63 | TT-AI TTA70+ önerisi |
| **K4a** | CC-Kitap **isim** kararı | K1 önerisi B#5 "Ekrandaki Ülke — Türkiye'nin 30 Yılı Nasıl Lanse Edildi" | Patron kararı bekleniyor (K2'de ertelendi) |
| **K8** | CC-Kitap TRADİA KÜTÜPHANESİ koleksiyon mimarisi (Cilt I hariç ciltler) | K2'de büyüdü — Patron vizyonu | Patron+Kitap ortak plan (S39+) |
| **K9** | Basın S50 çift-tier ilk regres eşiği ölçümü | S38 karar 3 (KABUL_REVİZE) | Basın S50 raporu |

**Kesintisizlik alarmı:**
- CC-Borsa S37 tetiği 2 sprint sessiz (S38+S39) — 3'te VAKA (S50 zorunlu geri bildirim)

---

## 3. PATRON AÇIK EYLEMLERİ

| # | Eylem | Öncelik | Not |
|---|---|---|---|
| **P1** | `launchctl load` 2 ek plist (14:00 + 21:00 tarama) | 🔥 Standing #19 tamamlanma | Hafıza S39'da script + plist yazacak; Patron `launchctl load` çalıştıracak |
| **P2** | EKAP Bülten manuel indir + drop-klasör | 🔨 Standing #8 rutini | Aralıklı (haftalık) — CC-İhale bekliyor |
| **P3** | TT-HAFIZA disk takıldığında S34-S38 delta yedek | ⏸ Standing #15 | Disk hazır olunca 5-dk delta turu |
| **P4** | Vezir "TRADİA-15 GENİŞ ÖZET" `.pages` → `.md`/`.txt` yapıştırma | 🔥 15_genis_ozet.md bölüm 4 boş | Pages formatı Hafıza tarafından okunamıyor (protobuf .iwa) |
| **P5** | CC-Kitap isim (K4a) kararı | 🟡 K2 sonrası | Grup A/B önerileri + öneri B#5 |

---

## 4. AKTİF SPRINT DURUMLARI (Tradia-16 devir noktası)

| CC | Sprint | Durum | Devir notu |
|---|---|---|---|
| CC-Hafıza | S39 (Standing #19 uygulama) | 🟢 AKTİF | ~/bin/hafiza_tarama.sh script + 2 plist yazılacak |
| CC-Basın | S47+ | 🟢 AKTİF (v1.2 emisyon) | S50 çift-tier regres kritik |
| CC-Borsa | S48? | 🟡 SESSİZ (2 sprint) | S37 tetik yanıtı zorunlu |
| CC-Analiz | S130+ | 🟢 AKTİF | Master 250.193 sabit |
| CC-Sosyal | S159 P2 | 🟢 AKTİF (P2 kesintisiz) | 36/500 → devam; kitap hammadde çift-kopya |
| CC-TT-AI | TTA67+ | 🟢 AKTİF | TTA70 3-karar uygulama raporu bekleniyor |
| CC-İhale | S39+ | 🟢 AKTİF | ihale_takvim v7 dağıtımda (symlink) |
| CC-Site | (rutin) | 🟢 AKTİF | tradiaturkey.com |
| CC-Tic | T115 | 🟢 AKTİF | 527/262 yeşil %100 LAUNCH-TEMİZ |
| **CC-Kitap** | **K2 BİTTİ → K3 aday** | **🟢 AKTİF** | Patron isim kararı + koleksiyon mimarisi K8 |

---

## 5. DİSİPLİN (Standing v1.7)

$0 · V16 dürüst · A04 uydurma-yok · V37 master read-only · V53 ≥2 kaynak · V48 izole · KVKK SERT · S14 ortaklık YASAK · Q38 · **19 kural (#1-#19)** · **Anayasa B1-B10** · K24a çift kanal · Lane · captcha/login/obfuscation bypass YASAK · Telif ≤2 cümle (CC-Kitap için özel) · akan su.

**Yeni disiplinler (Tradia-15 kazanımları):**
- **Standing #16** hafıza panosu (her sprint başı zorunlu)
- **Standing #17** classifier spot-check ≥%80 (canlıya çıkış koşulu)
- **Standing #18** mahalle üçlü-anahtar + ad-bazlı birleşme YASAK
- **Standing #19** toplu-tarama düzeni 09:00/14:00/21:00
- **B10** olacak-takvimi motoru
- **YAPISAL_TAMAM** (C) yolu — walled+Wikipedia-thin çözümü
- **Çift-tier `guvenilir_flag`** yuksek/orta/null + tüketici disiplin

---

## 6. AÇILIŞ RUTİNİ (Tradia-16 ilk 10 dk)

1. **3 URL fetch** (misara-vezir/vezir/ozet.json + hafiza_panosu.md + son sprint kayıtları)
2. **Bekleyen 5 karardan** birini netleştir (öncelik: P4 Vezir metni + K4a isim)
3. **Sessizlik alarmı:** CC-Borsa S37 tetik yanıtı zorunlu (3. sprint)
4. **Standing #19 uygulama** (Hafıza S39): 14:00 + 21:00 launchd
5. **Akan su:** doygunluk→yeni-yol; Sosyal 412 sabit → Fesa yeni; Kitap K3 aday

---

*Tradia-16 açılış brief hazır. CC-Hafıza + Chat Vezir bu brief + 15_genis_ozet.md + ozet.json ile başlayacak.*
