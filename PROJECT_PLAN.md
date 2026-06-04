# Projektplan: The Barber Rendsburg

## Tech-Stack

- Next.js App Router
- TypeScript
- Tailwind CSS
- Komponentenbasierte Sections
- Zentrale Datenstruktur unter `data/theBarber`

## Ordnerstruktur

```text
data/theBarber/
  siteConfig.ts
  services.ts
  pricing.ts
  gallery.ts
  reviews.ts
src/
  app/
  components/
    layout/
    sections/
    ui/
  lib/
public/images/the-barber-rendsburg/
```

## Designrichtung

- heller, freundlicher Friseur-/Barber-Auftritt
- Creme, Beige, Holzbraun und Dunkelgruen
- ruhige Karten, dezente Schatten, feine Linien
- leicht hochwertig, aber nicht dramatisch
- keine grellen Effekte und keine schwere dunkle Inszenierung

## Sektionen

1. Header
2. Hero
3. Salon-Intro
4. Leistungen
5. Preise
6. Galerie
7. Warum The Barber?
8. Termin anfragen
9. Kontakt & Öffnungszeiten
10. Bewertungen
11. Footer

## Buchung

`bookingUrl` ist leer. Deshalb zeigt die Website Termin-Anfrage, Telefon und Instagram. Sobald der Link gesetzt ist, wechselt die Logik auf Online-Buchung.

## Preise

Es werden keine Preise erfunden. Alle Leistungen zeigen dezent `Preis folgt`.

## Reviews

Die Google-Bewertung wird unten vor dem Footer prominent gezeigt. Rezensionstexte sind nur Platzhalter, bis echte öffentliche Bewertungen oder eine Kundenfreigabe vorliegen.

## Assets

Der Zielordner ist `public/images/the-barber-rendsburg/`. Echte Salonbilder und Logo-Quelle fehlen aktuell noch und sind in `ASSET_REQUEST.md` beschrieben.

## SEO

Metadata und HairSalon JSON-LD sind gesetzt. Aggregate-Rating wird nicht im JSON-LD ausgegeben, solange Review-Anzahl und Quelle nicht sauber belegt sind.
