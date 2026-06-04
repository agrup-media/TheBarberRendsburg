# The Barber Rendsburg

Moderne Website für den Herrenfriseur und Barbershop The Barber Rendsburg.

## Entwicklung

```bash
npm install
npm run dev
```

Die Seite läuft lokal unter `http://localhost:3000`.

## Weitergabe

Die Projekt-ZIP enthält bewusst keine `node_modules` und keinen `.next`-Build-Cache.
Nach dem Entpacken einmal `npm install` ausführen, danach kann die Seite mit
`npm run dev` lokal gestartet oder mit `npm run build` geprüft werden.

## Checks

```bash
npm run lint
npm run typecheck
npm run build
```

## Zentrale Daten

- Stammdaten, Buchung, Adresse und Öffnungszeiten: `data/theBarber/siteConfig.ts`
- Leistungen: `data/theBarber/services.ts`
- Preise: `data/theBarber/pricing.ts`
- Galerie: `data/theBarber/gallery.ts`
- Reviews: `data/theBarber/reviews.ts`

## Buchung

Solange `bookingUrl` leer ist, zeigt die Website "Termin anfragen" sowie Telefon
und Instagram als Kontaktwege. Sobald ein Buchungslink eingetragen wird, wechselt
der zentrale CTA auf "Online Termin buchen".

## Assets

Die Website erwartet echte Salonbilder unter:

- `public/images/the-barber-rendsburg/salon-innenraum-stuehle.jpg`
- `public/images/the-barber-rendsburg/salon-aussenansicht.jpg`
- `public/images/the-barber-rendsburg/salon-lounge.jpg`
- `public/images/the-barber-rendsburg/salon-produkte.jpg`

Fehlende Bilder werden bewusst als vorbereitete Bildplätze dargestellt.
