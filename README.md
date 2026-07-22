# Fokus-Timer

Ein einfacher Pomodoro-Timer als Single-Page-App (reines HTML/CSS/JS, keine Abhängigkeiten).

## Nutzung

`index.html` im Browser öffnen. Es gibt drei Modi:

- **Fokus 25** – 25 Minuten Arbeitszeit
- **Pause 5** – 5 Minuten kurze Pause
- **Lange Pause 15** – 15 Minuten nach jeder 4. Fokus-Session

Abgeschlossene Sessions und die gesamte Fokuszeit des Tages werden lokal im Browser gespeichert (`localStorage`) und unten in der App angezeigt.

## Features

- Fortschrittsring mit Countdown
- Automatischer Wechsel zwischen Fokus- und Pausenmodus
- Akustisches Signal bei Sessionende
- Hell-/Dunkelmodus passend zu den Systemeinstellungen
