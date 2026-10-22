# Studio Goeienaard

De website van Studio Goeienaard, ecologisch tuinontwerp: **[www.goeienaard.nl](https://www.goeienaard.nl)**

De site wordt automatisch gebouwd door GitHub Pages. Pas je een bestand aan en klik je op **Commit changes**, dan staat de wijziging na 1 à 2 minuten online. Je hoeft niets te installeren: alles kan via de GitHub-website.

---

## Teksten aanpassen

Bijna alle teksten staan bovenin de bestanden, tussen de twee regels met `---`. Pas alleen de tekst **na** de dubbele punt aan.

| Pagina | Bestand |
|---|---|
| Homepage | `index.md` (alle blokken, diensten, aanbevelingen en stappen) |
| Werkwijze | `werkwijze.md` (stappen, diensten en tarieven, veelgestelde vragen) |
| Ecologische tuin | `ecologische-tuin.md` (ook de planten onderaan) |
| Over | `over-ons.md` |
| Contact | `contact.md` |
| Projecten (overzicht) | `projecten.md` |
| Ecohoeve | `ecohoeve.md` |
| Algemene voorwaarden en privacy | `algemene-voorwaarden.md` |
| Pagina niet gevonden | `404.html` |

Een bestand aanpassen: open het, klik rechtsboven op het **potloodje**, wijzig de tekst en klik op **Commit changes**.

### Let op bij het aanpassen

- **Inspringing (spaties vooraan) precies laten staan.** Die bepaalt wat bij wat hoort.
- **Een dubbele punt in je tekst?** Zet dan de hele tekst tussen aanhalingstekens, bijvoorbeeld: `intro: "Let op: dit is een voorbeeld"`. Anders raakt de pagina in de war.
- **Lange teksten** staan soms onder `tekst: >-` op de volgende regel, ingesprongen. Dat mag je zo laten.
- Iets mis gegaan? Elke wijziging is terug te draaien via **History** (rechtsboven bij een bestand).

---

## Een project toevoegen

1. **Foto's:** maak een map in `assets/img/projecten/`, bijvoorbeeld `mijn-tuin`, en upload daar de foto's als `01.jpg`, `02.jpg`, enzovoort. `01.jpg` wordt de grote foto bovenaan. Houd foto's onder ±500 kB (maximaal ±2000 pixels breed).
2. **Tekst:** maak in de map `_posts` een nieuw bestand met de datum en een korte naam, bijvoorbeeld `2026-11-01-mijn-tuin.md`. Kopieer de inhoud van een bestaand project en pas die aan:

```yaml
---
title: Naam van de tuin
date: 2026-11-01
permalink: /projecten/mijn-tuin/
plaats: Tilburg
type: Ontwerp achtertuin
samenvatting: Eén of twee zinnen voor de projectkaart.
fotomap: mijn-tuin
bijschriften:
  "01.jpg": "Bijschrift bij de eerste foto"
---

## Over deze tuin

Hier het verhaal van het project.
```

Projecten verschijnen automatisch op de projectenpagina, met de nieuwste bovenaan. Een project tijdelijk verbergen? Zet `published: false` bovenin.

**Aanbeveling koppelen:** in `index.md` kun je onder een aanbeveling `project: /projecten/mijn-tuin/` zetten. De aanbeveling verschijnt dan ook onderaan die projectpagina, en op de homepage linkt hij naar het project.

---

## Afbeeldingen

| Wat | Waar |
|---|---|
| Projectfoto's | `assets/img/projecten/<projectmap>/` |
| Plantenfoto's | `assets/img/planten/` |
| Paginafoto's (homepage, werkwijze, over…) | `assets/img/` |
| Ecohoeve-tekeningen | `assets/img/ecohoeve/` |
| Logo en woordmerk | `assets/img/logo.svg`, `wordmark.svg`, `wordmark-verticaal.svg` |

Een foto vervangen: upload een nieuwe foto met **exact dezelfde bestandsnaam**.

---

## Instellingen

In `_config.yml` staan de gegevens die op meerdere plekken terugkomen: e-mailadres, telefoonnummer, Instagram, de link naar de voorwaarden en de code van het kennismakingsformulier (`formspree`). Pas je daar iets aan, dan verandert het overal op de site.

---

## Hoe het in elkaar zit

- **Hosting:** GitHub Pages, gratis. Het eigen domein staat in het bestand `CNAME`; de DNS loopt via Hostnet.
- **Kennismakingsformulier:** via [Formspree](https://formspree.io). Aanvragen komen per e-mail binnen.
- **Opmaak:** `assets/main.scss`. Kleuren, maten en afrondingen staan als variabelen bovenin de laatste sectie.
- **Paginasjablonen:** `_layouts/` (homepage, pagina, project) en herbruikbare onderdelen in `_includes/` (header, footer, lightbox, formulier, FAQ, diensten).

Liever niet aankomen tenzij je weet wat je doet: `_layouts/`, `_includes/`, `assets/main.scss` en `CNAME`.
