# Behördenfax – Publii-Projekt

Webseite für [behoerdenfax.de](https://behoerdenfax.de): eine Satire-Aktion des [eGovernment Podcasts](https://egovernment-podcast.com). Mitarbeitende von Behörden schicken ihren Digitalisierungs-Frust per Fax an **08142 6553738** (auch aus dem EPVPN unter 3468). Die Zuschriften werden anonymisiert in den sozialen Medien geteilt und im Podcast besprochen; jedes Fax bekommt eine persönliche Antwort.

Gebaut mit dem Static-CMS [Publii](https://getpublii.com) und einem Theme auf Basis des Design Systems [KERN-UX](https://kern-ux.de).

## Inhalt

| Pfad | Beschreibung |
|---|---|
| `themes/behoerdenfax-kern/` | Publii-Theme (KERN-UX 2.8.2, Fira Sans, orangener Akzent aus dem Logo) |
| `content/` | Text für die Startseite |
| `LICENSE` | EUPL-1.2 |
| `NOTICE.md` | Drittkomponenten und Lizenzhinweise |

## Einrichtung in Publii

1. Ordner `themes/behoerdenfax-kern` in den Publii-Ordner `themes/` kopieren (macOS: `~/Documents/Publii/themes/`) und Publii neu starten.
2. In der Seite unter *Site settings → Current theme* „behoerdenfax-kern“ über *Install and use* auswählen und speichern.
3. Unter *Theme* Faxnummer, Hinweistext, Podcast-Link und Social-Links prüfen.
4. Veröffentlichen, z. B. über GitHub Pages (*Server → GitHub Pages*).

## Theme-Aufbau

- `assets/css/main.css` wird von Publii zu `style.css` kompiliert. Sie wird aus `assets/scss/kern.min.css` und `assets/scss/behoerdenfax.css` zusammengesetzt (Schriften als Data-URI eingebettet).
- Der Ordner `assets/scss/` wird von Publii nicht ausgeliefert und enthält die Quellen. Änderungen am Design macht man in `behoerdenfax.css` und baut `main.css` danach neu.
- Hell- und Dunkelmodus kommen von KERN-UX. Der Button im orangen Bereich hat feste Farben.

## Status

Das Theme wurde in Publii eingerichtet, die Vorschau ist aber noch nicht abschließend geprüft.

## Lizenz

Veröffentlicht unter der [EUPL-1.2](LICENSE). Enthaltene Komponenten stehen unter kompatiblen Lizenzen, siehe [NOTICE.md](NOTICE.md).
