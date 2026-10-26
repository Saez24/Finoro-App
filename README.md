<p align="center">
  <img src="logo.png" alt="Finoro" width="120">
</p>

<h1 align="center">Finoro</h1>

<p align="center">
  <strong>Dein Haushaltsbuch, auf deinem eigenen Server.</strong><br>
  Einnahmen, Ausgaben, Budgets und Kredite im Blick, im Browser, als App auf dem Handy
  und ganz ohne Cloud.
</p>

---

## Was ist Finoro?

Finoro ist ein Haushaltsbuch, das du selbst betreibst, zum Beispiel auf einem Unraid-Server
zu Hause. Deine Finanzdaten liegen in deiner eigenen Datenbank und nicht bei einem Anbieter.
Jede Person hat ein eigenes Konto und sieht nur ihre eigenen Daten.

## Was die App kann

### Übersicht
- Gesamtvermögen und alle Konten auf einen Blick
- Bilanz für Monat, Woche und Tag
- Diagramme: Ausgaben und Einnahmen nach Kategorie, Fixkosten mit „frei verfügbar“,
  Kontostandsverlauf
- **Anpassbar**: Kacheln ein- und ausblenden und per Ziehen neu anordnen

### Buchungen
- Einnahmen, Ausgaben und Umbuchungen zwischen Konten
- Ansicht nach Tag, Woche, Monat, Quartal oder Jahr, mit laufendem Kontostand
- Sortieren nach Datum, Betrag, Titel, Kategorie oder Art; Liste, kompakt oder ausführlich
- **Wiederkehrende Buchungen** (monatlich, alle 3 Monate, jährlich, mit Enddatum).
  Beim Ändern oder Löschen wählst du „nur diese“ oder „diese und zukünftige“.
- Auf dem Handy: zur Seite wischen für Bearbeiten, Kopieren und Löschen, lange drücken für
  das Aktionsmenü

### Budgets
- Monatliche oder jährliche Limits je Kategorie, mit Anzeige, wie viel noch übrig ist

### Kredite
- Kreditsumme, Zins und Laufzeit eingeben, Finoro berechnet die Rate und legt die
  Ratenbuchungen automatisch an
- Restschuld und Fortschritt („12 von 60 Raten gezahlt“)
- Bestehende Kredite nachtragen und Kredite vorzeitig ablösen

### Konten, Kategorien, Import und Export
- Zahlungs-, Spar- und Kreditkartenkonten; Kategorien für Einnahmen und Ausgaben
- **Import** aus CSV (auch MoneyStats-Export) oder XML, mit Vorschau. Duplikate werden
  übersprungen, fehlende Konten und Kategorien werden angelegt.
- **Export** aller Buchungen als CSV oder XML

### Einstellungen
- Deutsch oder Englisch, hell, dunkel oder automatisch
- **Finanzmonat** mit eigenem Starttag, zum Beispiel vom 20. bis 19., wenn das Gehalt am 20. kommt
- Menüpunkte ausblenden, die du nicht brauchst
- Profil und Passwort ändern, alle Daten oder das ganze Konto löschen

## Auf welchen Geräten?

| | |
| --- | --- |
| **Browser (PC)** | Volle App mit Navigationsleiste links, Rechtsklick- und „…“-Menüs |
| **iPhone / Android (Web-App)** | Im Browser öffnen und „Zum Home-Bildschirm“ hinzufügen. Läuft dann wie eine App im Vollbild, mit Leiste unten und Wischgesten. |
| **Android-App** | Eigene App (Flutter). Speichert lokal auf dem Gerät oder verbindet sich mit deinem Finoro-Server. Optional mit Fingerabdruck-Sperre. |

## Screenshots

> Folgen. Geplante Bilder und Dateinamen: [docs/screenshots/](docs/screenshots/README.md)

<!--
| Übersicht | Buchungen | Kredite |
| --- | --- | --- |
| ![Übersicht](docs/screenshots/uebersicht.png) | ![Buchungen](docs/screenshots/buchungen.png) | ![Kredite](docs/screenshots/kredite.png) |
-->

## Sicherheit und Datenschutz

- Läuft komplett bei dir, ohne Cloud-Dienst, Tracking oder Werbung
- Registrierung mit E-Mail-Bestätigung; Anmeldung über sichere, für Skripte unzugängliche
  Cookies
- Strikte Trennung: Niemand sieht die Daten einer anderen Person, auch kein Admin

## Schnellstart

Finoro läuft als **ein Docker-Container** (`ghcr.io/saez24/finoro`) neben einer
PostgreSQL-Datenbank, hinter einem HTTPS-Reverse-Proxy wie Nginx Proxy Manager. Für Unraid
gibt es ein fertiges Template.

Downloads (Android-App, Web-App als ZIP) gibt es unter
**[Releases](https://github.com/Saez24/Finoro-App/releases)**.

## Anleitungen

- [Server installieren und betreiben](docs/installation.md)
- [Web-App nutzen und als App aufs Handy legen](docs/web.md)
- [Android-App installieren](docs/app.md)
- [Technik und Entwicklung](docs/TECHNIK.md) · [Releases veröffentlichen](docs/releases.md)

## Lizenz

[PolyForm Strict 1.0.0](LICENSE) mit Pflicht-Hinweis „Copyright © 2026 Saez24“: private und
andere nicht-kommerzielle Nutzung, keine Weitergabe, keine Änderungen. Kommerzielle Nutzung
nur mit separater Lizenz — Anfrage per Issue in
[Saez24/Finoro-App](https://github.com/Saez24/Finoro-App/issues).
