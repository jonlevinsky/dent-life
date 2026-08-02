# Dent&Life — Dentální laboratoř

**URL:** https://laborator-dentlife.cz  
**Doména:** `laborator-dentlife.cz`  
**Repozitář:** `J:\dent&life`

Webová prezentace **dentální laboratoře Dent&Life** s pobočkami v Benešově a Praze. Specializuje se na fixní a snímatelnou protetiku, metalokeramiku, celokeramiku a implantátové práce.

## Struktura projektu

`J:/dent&life`:

| Soubor / složka | Popis |
|---|---|
| `index.html` | Hlavní one-page web (všechny sekce) — 3633 řádků |
| `admin.html` | Administrace recenzí (heslo: `admin`) |
| `dentlife_data.json` | Data pro sekce Vybavení a Reference |
| `equipment_manager.py` | Tkinter GUI editor vybavení a referencí |
| `test.html` | Testovací HTML fragment referencí |
| `data/config.json` | Konfigurace (maintenance mode) |
| `data/reviews.json` | Recenze zákazníků |
| `data/reviews.xml` | XML export recenzí |
| `files/res/` | Obrázky, loga, SVG, videa |
| `files/res/reference/` | Fotky referenčních prací (ref-01 až ref-05) |
| `files/res/video/` | Hero video (hero.mp4, hero-mobile.mp4, poster) |
| `files/res/svg/` | SVG varianty loga (light/dark, stacked) |
| `.vscode/settings.json` | Nastavení editoru |

## Features

### Responzivita

Breakpointy: 1024px, 768px, 640px. Header přechází z transparentního na bílý (blur) při scrollu. Mobilní hamburger menu.

### Animace

- **Intersection Observer** — staggered reveal sekcí a karet (120ms zpoždění)
- **Cross-fade obrázků** — v About sekci (10s interval)
- **Custom scrollbar** — vlastní scroll thumb s drag & drop
- **Hover efekty** — karty (translate, shadow, icon color)
- **prefers-reduced-motion** — plná podpora

### Gallery Modal

Fullscreen prohlížení referencí, navigace šipkami a swipe, klávesové zkratky, vodoznak.

### Map Modal

Google Maps iframe, focus trap, tlačítko "Navigovat".

### SEO

Schema.org (Dentist, MedicalBusiness, VideoObject, WebSite, WebPage, ImageObject), Open Graph, Twitter Cards, geo tagy.

### Maintenance mode

Přes `data/config.json`. Při aktivaci se zobrazí custom zpráva.

### Image handling

Shimmer loading, lazy loading, error fallback placeholder.

## Editor vybavení (`equipment_manager.py`)

Tkinter GUI pro správu `dentlife_data.json`:

- Drag & drop řazení položek
- Inject HTML přímo do `index.html`
- Auto-save do JSON

### Vybavení

| # | Název | Klíčové vlastnosti |
|---|---|---|
| 01 | CAD/CAM systém | 5-osé frézování, Exocad |
| 02 | Keramická pec | Ivoclar, programovatelné křivky |
| 03 | Stereomikroskop | 40× zvětšení, LED |
| 04 | 3D skener | 5 µm rozlišení |

### Reference

| Index | Název | Soubor |
|---|---|---|
| 0 | Metalokeramické korunky | `ref-01.jpg` |
| 1 | Celokeramické můstky | `ref-02.jpg` |
| 2 | Implantátové práce | `ref-03.jpg` |
| 3 | Snímatelné protézy | `ref-04.jpg` |

## Odkazy

- **Web:** https://laborator-dentlife.cz
- **Admin:** https://laborator-dentlife.cz/admin.html
- **Email:** dentlife@email.cz
- **Telefon:** +420 608 547 489 (Praha), +420 723 159 128 (Benešov)
- **Portfolio autora:** https://levinskyj.art
