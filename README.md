# FlashBox — Dokumentation

Öffentliche Rechts- und Datenschutzseiten für die FlashBox-App, ausgeliefert über GitHub
Pages: **https://markono-code.github.io/FlashBox-Docs/**

Die Seiten sind aus den Store-Einträgen und aus der App verlinkt (Profil → Über & Hilfe, und
die Zeile unter «Konto erstellen»). Die Seite zur Kontolöschung ist Pflicht für Google Play
und den App Store; sie muss ohne Login und ohne installierte App erreichbar bleiben.

## Seiten

| Datei | URL | Inhalt |
|---|---|---|
| `index.html` | `/` | Übersicht |
| `privacy-policy.html` | `/privacy-policy.html` | Privacy Policy (Englisch) |
| `datenschutzerklaerung.html` | `/datenschutzerklaerung.html` | Datenschutzerklärung (Deutsch) |
| `terms.html` | `/terms.html` | Terms of Use (Englisch) |
| `nutzungsbedingungen.html` | `/nutzungsbedingungen.html` | Nutzungsbedingungen (Deutsch) |
| `licenses.html` | `/licenses.html` | Lizenzen der verwendeten Bibliotheken, Schriften und Icons |
| `delete-account/index.html` | `/delete-account/` | Kontolöschung, zweisprachig |

**Die Dateinamen sind Schnittstelle.** Die App öffnet genau diese URLs; eine Seite umzubenennen
bricht den Link in jeder ausgelieferten Version.

Die Sprachfassungen sind getrennte Seiten, kein JavaScript-Umschalter: Rechtstexte stehen
unter einer eigenen, zitierbaren URL und sind ohne JS vollständig lesbar.

## Aufbau

```
FlashBox-Docs/
├── assets/
│   ├── css/docs.css     # das gesamte Design, eine Datei
│   ├── js/docs.js       # nur Theme-Umschalter und Jahreszahl
│   └── img/             # App-Icon und Favicon
├── index.html
├── privacy-policy.html · datenschutzerklaerung.html
├── terms.html · nutzungsbedingungen.html
├── licenses.html
└── delete-account/index.html
```

Kein Build, keine Abhängigkeiten. Eine Datei im Browser öffnen ist die ganze
Entwicklungsschleife. Veröffentlicht wird der Branch `main`, Wurzelverzeichnis.

## Was der Text behauptet, muss stimmen

Die Seiten beschreiben, was die App tatsächlich tut. Ändert sich in FlashBox etwas davon,
gehört die Seite im selben Zug angepasst (und das Datum oben):

- ein neuer Dienstleister oder ein neues SDK (heute: Supabase, Resend, Firebase
  Crashlytics, die Sprachdienste des Geräts, Google Fonts unter Android) → Datenschutz
- eine neue Berechtigung (heute: Mikrofon, Internet) → Datenschutz
- etwas Neues, das gespeichert wird, oder eine Aufnahme, die das Gerät verlässt → Datenschutz
- eine andere Art der Kontolöschung (heute: sofort, in der App, ohne Karenzfrist) → Datenschutz
  und Kontolöschung
- eine neue Bibliothek, Schrift oder ein neuer Datensatz → Lizenzen
- Bezahlfunktionen, oder Inhalte anderer Lernender (Stapel von Lehrpersonen) → Nutzungsbedingungen

Die Texte sind ohne anwaltliche Prüfung entstanden.

## Design-Familie

Diese Site gehört zur Design-Familie von markono.dev, Tap2Card-Docs und Ausgetrunken-Docs.
Kanonische Beschreibung: `MarkoNoDev/docs/DESIGN_FAMILY.md` in `Claude-Projects`. Die
Akzentfarben stammen aus FlashBox' `Color.kt`.
