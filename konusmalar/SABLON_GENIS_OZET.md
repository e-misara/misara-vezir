# TRADİA-<N> · GENİŞ ÖZET (ŞABLON)

**Amaç:** Bu şablon, yeni konuşma-turlarının geniş özetlerinin tek biçimli üretilmesi için.
**Kaynak referans:** `15_genis_ozet.md` (Tradia-15 kapanış — kanonik format).
**Standing:** Vezir kanonu #47 (aday) — "Her kısım kapanışında bu şablon zorunlu."

**KA-01 kararı (2026-08-27):** Şablon yazılmadan geniş özet üretme.
Şablon 5 bölümden oluşur — hiçbiri boş bırakılamaz (varsa "yok" yazılır, atlanmaz).

---

## Ana Meta (dosya üstü)

```
**Kısım:** Tradia-<N>
**Tarih aralığı:** YYYY-MM-DD → YYYY-MM-DD
**Süre:** <kaç sprint · kaç iş günü>
**Devir noktası:** <önceki kısım no> → <bu kısım no> → <sonraki kısım no>
**Kaynak tutanaklar:** `misara-vezir/konusmalar/tam_tutanak/<tarih>_<konu>.md` (linkli)
**Disiplin:** $0 · V16 dürüst · Standing v1.X · KVKK #31 v1.Y · S14 ortaklık YASAK
```

---

## 1. ANA İŞ (Bu kısımda ne yapıldı)

### 1.1 · Ana sprintler
- **Sprint X — <ad>** [1 satır özet]
- **Sprint Y — <ad>** [1 satır özet]

### 1.2 · Kim ne başlattı
- **CC-<ad>** [ne başladı]
- **CC-<ad>** [ne bitti]

### 1.3 · Kim ne devretti
- **<devir 1>** → hangi CC'ye
- **<devir 2>** → hangi CC'ye

---

## 2. KİLİTLENEN KARARLAR

Format tablo (5 sütun zorunlu):

| # | Karar | Kim aldı | Tarih | Nerede yazılı |
|---|---|---|---|---|
| 1 | <karar metni> | Patron / Üst Akıl / CC | YYYY-MM-DD | `dosya-yol` veya `Standing #X` |

**"Karar bozuldu" alt-tablo (varsa):**

| Karar | Bozuldu-tarih | Neden bozuldu |
|---|---|---|

---

## 3. RAKAMLAR (Kaynaklı)

**Kural:** Her rakamın YANINDA kaynak dosya (Standing #45).

| Metrik | Değer | Kaynak | Tarih |
|---|---|---|---|
| Havuz SORGU-01 | ... | `~/tradia_sorgu/tradia_sorgu.db` | YYYY-MM-DD |
| Beykoz kayıt | 325.186 | `pano/ozet-w35.json` | 2026-08-27 |
| ... | ... | ... | ... |

**"Şüpheli/Bozuk rakam" alt-tablo:**

| Metrik | Değer | Neden şüpheli | Doğrusu |
|---|---|---|---|
| Beykoz kayıt (eski) | 363.582 | Basın etiket bozuk | 325.186 (v2r) |

---

## 4. AÇIK KALANLAR (Bu kısım kapanırken çözülmeyen)

Format tablo:

| # | Açık iş | Kim sorumlu | Öncelik (1-3) | Sonraki kısıma devir |
|---|---|---|---|---|
| 1 | <iş> | CC-<ad> / Patron | 1 | evet/hayır |

---

## 5. SONRAKI KISIMA DEVİR

### 5.1 · Hazırlık paketi (bir sonraki kısım açılırken okunacak)
- 3-URL fetch: [`pano/ozet-wN.json`](url) · [`kanon/INDEKS.md`](url) · [`konusmalar/<N+1>_acilis_brief.md`](url)
- **Kanonik sabit panel:** (sayılar tabloyla)
- **Aktif CC listesi:** (sprint no + durum)

### 5.2 · Bekleyen Patron kararları
- <karar 1>
- <karar 2>

### 5.3 · Vezir dürüst-not (A04)
- Yapılamayan · nedeni
- Kaynak-boşluğu
- Kayıt-tutmayanlar

---

## Standing İlişkisi

- **Standing #35+#36+#38** — Vezir push disciplini
- **Standing #43** — dürüst düzeltmeler
- **Standing #45** — kanon: kaynak-yanı rakam · pano tek-komut yayın
- **Standing #47 (aday)** — bu şablon zorunlu

---

*Şablon · Vezir KA-01 · 2026-08-27 · Bu şablona uymayan geniş-özet KANON DIŞI kabul edilir.*
