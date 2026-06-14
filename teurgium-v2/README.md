# Teurgium — Website v2 (Sprint 1–3)

**Branch:** `teurgium-v2-sprint3`  
**Commit tag:** `feat: teurgium-v2-sprint3-complete`

## Stack
Vanilla HTML/CSS/JS — zero dependencji, zero npm, single-file SPA.  
Obrazy jako `./images/img_XX.jpg` — podmień na CDN/S3 w obiekcie `IMGS{}`.

## Sekcje strony głównej
| # | Sekcja | Uwagi |
|---|--------|-------|
| 1 | **Hero** | Full-height, zdjęcie bg, gradient overlay, tekst + 2x CTA |
| 2 | **CategoryGrid** | Max 3 kolumny, kafle ze zdjęciem 200px, duże nazwy 18px |
| 3 | **WhyUsSection** | 6 kart USP, max 3 kolumny, ikona w zielonym kwadracie |
| 4 | **GalleryIrregular** | 12-col nieregularny grid — gi1 duże (7col/2row), gi2-gi6 małe |
| 5 | **PromotionsSlider** | Auto-rotate 4.5s, pill dot z animacją width |
| 6 | **HowToOrderSteps** | Outlined numeracja 01–04 (-webkit-text-stroke) |
| 7 | **ReviewsSection** | 3 karty, gwiazdki |
| 8 | **ContactSection** | Dane + formularz |

## System RFQ (5 kroków)
1. Produkty — lista wybranych, add/remove
2. Parametry — kolor, faktura, format, ilość, termin
3. Macierz — rows=parametry, cols=produkty
4. Dane kontaktowe + walidacja
5. Potwierdzenie + reset

## 2 własne zmiany autora (Claude)
**[#1] Footer 3-kolumnowy** (`bg #064E3B`) — logo, lista kategorii, kontakt + CTA.

**[#2] Step numbers outlined** (`-webkit-text-stroke: 2px #1D9E75`) — numery 01-04 jako konturowe cyfry.

## TODO dla TRAE / Codex
- [ ] Dodać `images/img_01–img_16.jpg` (z D:\projekty 2026\teurgium.com\images)
- [ ] Podmienić `./images/img_XX.jpg` na URL CDN w obiekcie `IMGS{}`
- [ ] `POST /api/inquiries` endpoint z payloadem `{ items[], client{} }`
- [ ] Email trigger (Resend / Mailgun)
- [ ] Google Maps embed
- [ ] Google Reviews widget
- [ ] CMS dla PRODUCTS[] i GALLERY_DATA[]
- [ ] SEO meta, OG tags, JSON-LD LocalBusiness
- [ ] Analytics GA4 / Plausible
