# TRADIA — KONUŞMA #12 GENİŞ ÖZET
## CİMER Kampanyası + EKAP-Bülten Kırılması + İnsan-Eli Parser Deseni

**Tarih:** 16 Haziran 2026 · **Sıra:** Konuşma #12 · **Disiplin:** $0 · V16 dürüstlük · A04 (uydurma yok) · V37 · KVKK SERT · Q38 · provenance · Lane · akan su

---

## 1. CİMER / 4982 BİLGİ-EDİNME FRAMEWORK (resmî "50 Soruda CİMER" kitapçığından)

- **Tür = "Bilgi edinme"** (Soru 30) — somut istenen belge açıkça yazılır.
- **Konu TAMAMEN metinde** (max 3000 karakter); dosya = yalnız görsel delil. "Başvurum ektedir/dilekçem ektedir" → **reddedilir** (Soru 25).
- **Günde 1 başvuru** (Soru 16 — CİMER'e özgü limit). **15 iş günü** cevap (Soru 36).
- **⚠ Q38 ticari-kullanım kısıtı:** CİMER'den alınan veri/belge ticari amaçla aynen çoğaltılamaz/kullanılamaz; yalnız kaynak göstererek referans/eğitim. **Çözüm (Tradia disiplini):** veriyi YENİDEN YAZ + "VAR" sinyali sun (isim/belge değil) + ticari kartı BAĞIMSIZ-PUBLIC kaynağa oturt (Resmi Gazete/EKAP/VGM).
- **KVKK:** bireysel tapu/malik/parsel-değer = BLOKLU; yalnız toplulaştırılmış (aggregate) istenir.
- **2 başvuru sahibi** (Patron + [2. başvuru sahibi]) — her biri KENDİ kimliğiyle (Soru 19), domain'e bölünür (kopyalama = Soru 11-g hakkın kötüye kullanımı). Şahıs firması = [2. başvuru sahibi]'nın kendisi (3. kimlik değil).
- **Kapsam DIŞI** (Soru 10): dernek, vakıf, şirket, muhtarlık → bunlar için başka kaynak.

## 2. NATIONAL KAPSAM DÜZELTMESİ (kritik ders)

İlk taslak flagship-ilçeye (Antalya Kepez) sıkışmıştı → **TÜM TÜRKİYE'ye** açıldı.
- **Prensip:** Veri TUTULDUĞU seviyede istenir. Merkezi kurum (ÇŞB/TKGM/VGM/Milli Emlak/Ticaret/SPK/OGM) **tek başvuruda ülke-geneli il/ilçe özeti** verir — kurumun mevcut dataset'i olduğundan "aşırı iş yükü" reddine girmez.
- Yalnız belediye yapı ruhsatı yerel → **TÜİK national taban** + öncelikli illerde mahalle-detay.

## 3. DOĞRU KURUM ROUTING

- 15 yüksek-değer taşınmaz ihalesinin **14'ü VGM** (Vakıflar GM — vakıf taşınmaz), **1'i Milli Emlak** — **KİK DEĞİL** (KİK = 4734/EKAP).
- VGM ihaleleri il/ilçe + muhammen + VGM-ilan-ref ile tanımlandı (İKN $0 kaynaklarda yoktu).
- En yüksek: Antalya/Kepez VGM 385.705.000 TL (ilan 1833/1).

## 4. CİMER BAŞVURU TAKVİMİ (national, 10) + HAFIZA TAKİP (S18→S19)

1. TASBİS emlak registry (Ticaret Bak.) ✓ gönderildi
2. **VGM** vakıf taşınmaz ihale winner+bedel (national)
3. **ÇŞB** 6306 riskli alan/rezerv (national — İ36'da $0'da 0 çıkan boşluğu kapatır)
4. **Milli Emlak** Hazine taşınmaz satış sonuç (national)
5. **TKGM** tapu devir adedi (national, aggregate)
6. KİK/EKAP 4734 · 7. SPK değerleme · 8. OGM 2B · 9. belediye ruhsat · 10. raylı/yol

Hafıza S19 = veri-edinme düzen denetçisi: CİMER takvim (gönderim denetim + 15-iş-günü sonuç takip + BEDK itiraz flag) + public-kaynak takip + düzen koru (provenance/lane/KVKK).

## 5. DEVLET VERİ ENVANTERİ PDF

35 veri kalemi · 8 kategori · 24 harita-katmanı. Erişim renk-kodu: 🟢 CİMER ~18 · 🔵 zaten-public ~14 · 🟡 aggregate 3 · 🔴 bloklu 2.
Dürüst sınırlar: bireysel tapu/değer/malik BLOKLU · DBM değer haritası 2026 public gelecek · Q38 ticari-kısıt.

## 6. PUBLIC-KAYNAK GENİŞLEME (12 → 30+)

- **Çevre/risk (harita):** AFAD Deprem Tehlike Haritası · MTA diri fay + heyelan · OGM orman + 2/B · DKMP sulak alan/RAMSAR/ÖÇK · Kültür SİT · ÇŞB doğal SİT/ÇED/CORINE · DSİ taşkın/havza · MGM iklim · MAPEG maden/jeotermal
- **Taşınmaz/değer:** Milli Emlak ilan · TKGM parselsorgu (geometri) · GİB/belediye arsa rayiç + emlak vergi asgari m² · TKGM DBM (gelecek) · Özelleştirme · TOKİ
- **Enerji/arazi:** GES/RES lisans (EPDK) · YEKA/GEPA/REPA atlas (EİGM) · TEİAŞ enerji nakil hattı · BOTAŞ boru
- **Tarım:** arazi sınıfı (mutlak/dikili) · mera · zeytinlik (3573) · büyük ova
- **Şehir:** İBB + büyükşehir açık-veri · data.gov.tr · **Firma:** KAP · SPK · TBB

## 7. ARAZİ-ANLAMA KATMANI (Tradia çekirdek fark)

Bu katmanlar üç işe yarar: (1) **yapılaşma KISITI** (sulak/ÖÇK/kıyı/mutlak-tarım/zeytinlik = inşa edilemez), (2) **disamenity** (ENH hattı/trafo/RES yakını değer düşürür), (3) **fırsat** (GES/RES potansiyel arazi). Endeksa değerler; **Tradia "bu arazide ne VAR, ne yapılabilir" der.**

## 8. GIS-HARVEST PROBE (dürüst — A04)

National GIS/çevre/taşınmaz kaynakları $0-düz-curl'e büyük ölçüde KAPALI: SSL-cert bozuk · SPA · login-redirect · WAF gövde-reset (200-header döner, gövde bot-tespitle kesilir). Sahte HAM üretilmedi. ArcGIS-REST/WMS/WFS endpoint keşfi = ayrı GIS-harvest sınıfı.

## 9. ⭐ EKAP ÜYELİK + BÜLTEN KIRILMASI

- Patron EKAP'a kayıt oldu (kendi adına).
- **Keşif:** EKAP günlük **Kamu İhale Bülteni PDF** (YAPIM ilan + YAPIM_SONUC sonuç) = **İKN + kazanan + sözleşme bedeli + il/ilçe/mahalle**.
- **PUBLIC kayıt → Q38 YOK, ticari kullanılır** (CİMER'den de EPDK'dan da temiz). KVKK: tüzel göster, gerçek kişi → "VAR sinyali + kendi sözcükleri".
- **Vezir-doğrulanmış örnek:** İKN 2026/666770, Sözleşme Bedeli 29.195.000 TRY, Yüklenici, Yapılacağı yer Adana/Pozantı/Dağdibi Mahallesi.
- "İKN bizde yok" sorunu çözüldü (bülten İKN içeriyor).

## 10. ⭐ STANDING METHOD #8: "İNSAN-ELİ + PARSER"

**WAF/server-state engelleri yalnız OTOMASYONA (curl/headless) karşı.** İnsan tarayıcıdan bülteni indirir (bot-değil, WAF açık) → drop-klasöre koyar → İhale yalnız $0 PARSE eder. Çekmek/scrape yok.
- **Headless/fonlama GEREKSİZ** kıldı (EKAP için kesin; çoğu otomasyon-dirençli public kaynak için genel $0 desen).
- `bulten_parser.py` hazır (pypdf 6.10.2 + sabit-etiket regex), self-test PASS. Drop-klasör: `~/tradia_konusmalar/bulten/`. Durum: DROP-BEKLİYOR.

## 11. EPDK / EKAP-KSP DURUM

- **EPDK EPVYS ~%90 haritalandı:** Sorgula buton `j_idt61` · render-hedefi `ozetListelePanel` · il=7 (Antalya) option-parse doğrulandı · DataTable id `elektrikUretimOzetSorguSonucu:list`. Engel: cross-form JSF server-session-state $0-curl 2-aşama POST'ta taşınmıyor → headless VEYA **manuel-export** (Patron: EPVYS sonuç tablosunda "Excel'e Aktar"/"Yazdır" butonu var mı? — kontrol bekliyor).
- **EKAP-KSP** (ASP.NET) public ama ViewState server-side → **bülten deseni çözdü**, KSP-scraping gereksiz.
- **Yan-keşif:** ihale.gov.tr → ekapv2.kik.gov.tr (Angular + token-API) yönleniyor → gelecek $0 yol adayı.

## 12. 6 YEŞİL KANAL (temiz $0)

Resmi Gazete · CSB-e-Devlet · VGM · SGK · DSİ · **EKAP-bülten** (yeni 6.)

## 13. ÜYELİK / MEKANİZMA LİSTESİ

- **Hesap gerekenler:** e-Devlet ✓ · CİMER ✓ · **EKAP ✓** · İBB+büyükşehir açık-veri (API key) · TÜİK mikroveri · TCMB EVDS ✓ · MERSİS · data.gov.tr
- **CİMER-benzeri mekanizmalar:** doğrudan-kurum bilgi-edinme birimi (günde-1 baypas) · BEDK itiraz (reddedilen, 15 gün) · TBMM Dilekçe Komisyonu · Kamu Denetçiliği/Ombudsman (cevap-yok)

---

## 🔑 AÇIK PATRON-AKSİYON (sonraki oturuma taşınır)

1. **Bülten PDF'lerini** `~/tradia_konusmalar/bulten/`'e koy → parser `bulten_yapim.jsonl` üretir (İKN+kazanan+bedel+mahalle).
2. **EPDK EPVYS** sonuç tablosunda Excel/Yazdır butonu kontrol → varsa headless tümüyle gereksiz.
3. **CİMER günde-1 national gönderim** devam (sıra: VGM → ÇŞB 6306 → Milli Emlak → TKGM → ...).
4. **Headless/fonlama muhtemelen GEREKSİZ** — insan-eli+parser deseni çözüyor.

## DİSİPLİN ÖZETİ

$0 · AI-çağrısı 0 · bypass YOK · V16 (dürüstlük; sahte HAM/satır üretilmedi, "yapılamadı" net işaretlendi) · A04 (uydurma yok, eksik=flag) · V37 (master read-only) · KVKK SERT · Q38 (referans/public-dayanak ayrımı) · provenance (bağımsız-public, iç-referans=0 hedef) · Lane (İhale HAM, Analiz skor/harita) · akan su.
