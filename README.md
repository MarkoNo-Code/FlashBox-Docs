# FlashBox — Dokumentation

Öffentliche Rechts- und Datenschutzseiten für die FlashBox-App, gedacht für GitHub Pages
unter **https://markono-code.github.io/FlashBox-Docs/** (noch nicht veröffentlicht).

Die Seiten werden aus den Store-Einträgen und aus der App verlinkt. Die Seite zur
Kontolöschung ist Pflicht für Google Play und den App Store; sie muss ohne Login und ohne
installierte App erreichbar bleiben.

## Seiten

| Datei | URL | Inhalt |
|---|---|---|
| `index.html` | `/` | Übersicht |
| `privacy-policy.html` | `/privacy-policy.html` | Privacy Policy (Englisch) |
| `datenschutzerklaerung.html` | `/datenschutzerklaerung.html` | Datenschutzerklärung (Deutsch) |
| `delete-account/index.html` | `/delete-account/` | Kontolöschung, zweisprachig |

Die beiden Sprachfassungen sind getrennte Seiten, kein JavaScript-Umschalter: Rechtstexte
stehen unter einer eigenen, zitierbaren URL und sind ohne JS vollständig lesbar.

Kein Build, keine Abhängigkeiten. Eine Datei im Browser öffnen ist die ganze
Entwicklungsschleife.

## Was der Text behauptet, muss stimmen

Die Datenschutzerklärung beschreibt, was die App tatsächlich tut. Ändert sich in FlashBox
etwas davon, gehört die Seite im selben Zug angepasst (und das Datum oben):

- ein neuer Dienstleister oder ein neues SDK (heute: Supabase, Resend, Firebase
  Crashlytics, die Sprachdienste des Geräts, Google Fonts unter Android)
- eine neue Berechtigung (heute: Mikrofon, Internet)
- etwas Neues, das gespeichert wird, oder eine Aufnahme, die das Gerät verlässt
- eine andere Art der Kontolöschung (heute: sofort, in der App, ohne Karenzfrist)

## Design-Familie

Diese Site gehört zur Design-Familie von markono.dev, Tap2Card-Docs und Ausgetrunken-Docs.
Kanonische Beschreibung: `MarkoNoDev/docs/DESIGN_FAMILY.md` in `Claude-Projects`. Die
Akzentfarben stammen aus FlashBox' `Color.kt`.
