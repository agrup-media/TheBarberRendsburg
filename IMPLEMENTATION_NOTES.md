# Implementation Notes

## Richtung

Die Website wurde als heller, freundlicher und professioneller Friseur-/Barber-Auftritt neu aufgebaut. Der Entwurf nutzt Creme, Beige, Holzbraun und Dunkelgruen mit ruhigen Flaechen, feinen Linien und klarer Typografie.

## Struktur

- `data/theBarber/siteConfig.ts`: zentrale Stammdaten, Buchungslink, Adresse, Oeffnungszeiten und Rating
- `data/theBarber/services.ts`: Leistungen
- `data/theBarber/pricing.ts`: Preisplatzhalter
- `data/theBarber/gallery.ts`: erwartete Salonbilder
- `data/theBarber/reviews.ts`: Review-Platzhalter
- `src/components/sections/*`: einzelne Website-Sektionen
- `src/components/layout/*`: Header und Footer
- `src/components/ui/*`: wiederverwendbare UI-Bausteine

## Buchungslogik

`bookingUrl` ist aktuell leer. Die Website zeigt deshalb "Termin anfragen" sowie Telefon- und Instagram-Aktionen. Sobald `bookingUrl` in `data/theBarber/siteConfig.ts` gesetzt wird, wechselt der zentrale CTA auf "Online Termin buchen".

## Bewertungen

Die Bewertung `4,7 von 5 Sternen bei Google` wird nur unten im Bewertungsbereich prominent angezeigt. Im Hero erscheint sie nur klein und dezent. Da keine echten Rezensionstexte lokal vorliegen, verwendet `data/theBarber/reviews.ts` klar erkennbare Platzhalter.

## SEO

Gesetzt sind:

- Titel: `The Barber Rendsburg – Herrenfriseur & Barbershop`
- Description: `Herrenhaarschnitt, Fade, Bartpflege und Konturen bei The Barber Rendsburg – seit 2021 an der Schiffbrücke 2.`
- Open Graph Titel und Beschreibung
- HairSalon JSON-LD mit sicheren Daten: Name, Adresse, Telefon, Instagram und Oeffnungszeiten

Die Google-Aggregate-Rating-Daten werden nicht im JSON-LD ausgegeben, solange kein sauberer Review-Count und keine freigegebene Quelle vorliegen.

## Accessibility

- Semantische Headings
- sichtbare Fokuszustaende
- zugaengliche mobile Navigation
- Alt-Texte und Bildplatzhalter
- `prefers-reduced-motion` fuer Animationen

## Drittanbieter

Keine automatisch ladenden Google-Maps-iframes, keine Instagram-Embeds und keine externen Hotlinks fuer Bilder.

## Hero-Bilder

Die zwei Hero-Motive wurden gegen lokale Facebook-Dateien und oeffentlich
abrufbare Instagram-Embed-Dateien geprueft. Auf Wunsch werden nun die beiden
breiten Facebook-Motive fuer den Hero verwendet, weil Motiv und Ausschnitt fuer
den Vollbild-Hero besser passen:

- `hero-salon-stuehle-facebook.jpg`: `960x540`
- `hero-salon-laden-facebook.jpg`: `960x540`
- vorherige Datei `hero-salon-stuehle.jpeg`: `1179x1179`
- vorherige Datei `hero-salon-laden.jpeg`: `1179x904`
- Instagram `CMCe0ewgsmb`: `480x480`
- Instagram `CNcrOq0A98n`: `720x377`
- lokaler Facebook-Kandidat fuer das zweite Motiv: `960x540`

Es wurde keine kuenstliche Hochskalierung vorgenommen.
