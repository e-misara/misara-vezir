# Misara Vezir — Public Durum Panosu

> Misara Group ajan orkestratörü Vezir'in halka açık, read-only durum aynası.

## Amaç

Asıl repo (`gacbusiness`) **private**. İçinde:
- AI ajan tanımları
- İç stratejik notlar
- Reports/CEO_BRIEF arşivi
- Workflow + secret referansları

bulunur. Bu repo **sadece public-safe JSON** içerir — Claude (üst-akıl) ve
diğer AI tüketicilerin Vezir panosunu okuyabilmesi için.

## Endpoint'ler

GitHub Pages aktive sonrası:

```
https://e-misara.github.io/misara-vezir/vezir/status.json
https://e-misara.github.io/misara-vezir/vezir/ozet.json
https://e-misara.github.io/misara-vezir/vezir/vaka_havuzu.json
https://e-misara.github.io/misara-vezir/vezir/_nerede.json
```

## Güncelleme

Bu repo manuel güncellenir. gacbusiness reposunda
`scripts/sync_to_public.sh` çalıştırılır → buraya kopyalar + push.

## İlke

- **AI çağrısı YOK** — statik JSON pano
- **Asla susmaz** — kredi bitse bile dashboard ayakta
- **Public-safe** — müşteri isim/email/telefon ASLA, sadece rakam ve kamuya açık bilgi

## Lisans / Kapsam

Bu repo Misara Group iç ürünü olarak yayınlanmıştır. Veri Misara'ya aittir.
