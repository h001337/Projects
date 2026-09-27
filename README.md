# Fokus-Timer

Ein einfacher Pomodoro-Timer als Single-Page-App (reines HTML/CSS/JS, keine Abhängigkeiten).

## Nutzung

`index.html` im Browser öffnen. Es gibt drei Modi:

- **Fokus** – Arbeitszeit
- **Pause** – kurze Pause
- **Lange Pause** – nach jeder n-ten Fokus-Session

Über das Zahnrad-Symbol oben rechts lassen sich Fokuszeit, kurze Pause, lange Pause und das Intervall (nach wie vielen Fokus-Sessions die lange Pause startet) einstellen, z.B. Intervall 3 → 25-5-25-5-25-15.

Abgeschlossene Sessions und die Fokuszeit werden lokal im Browser gespeichert (`localStorage`) – sowohl für heute als auch als Verlauf für die Wochenstatistik.

## Features

- Fortschrittsring mit Countdown
- Automatischer Wechsel zwischen Fokus- und Pausenmodus
- Einstellbare Zeitintervalle (Fokus, Pause, lange Pause, Intervall bis zur langen Pause)
- Wochenstatistik (Sessions & Fokuszeit pro Tag, Mo–So)
- Akustisches Signal bei Sessionende
- Hell-/Dunkelmodus passend zu den Systemeinstellungen

## Datenspeicherung

Es gibt keinen Server/Backend – alles liegt im `localStorage` des Browsers:

- `fokusTimerSettings` – die eingestellten Zeitintervalle
- `fokusTimerHistory` – ein Eintrag pro Tag (`{ "YYYY-MM-DD": { sessions, focusMinutes } }`), daraus werden sowohl "Sessions heute" als auch die Wochenstatistik berechnet
