# ConsentScan – Anleitung (ca. 15 Minuten, 0 € Startkosten)

## 1. Code auf GitHub (3 Min)
1. Account auf github.com anlegen, oben rechts „New repository“, Name `consentscan`, Create.
2. Auf der Repo-Seite „uploading an existing file“ klicken, ALLE Dateien aus diesem Ordner hineinziehen (inkl. Ordner `public`), „Commit changes“.

## 2. Kostenlos online stellen (5 Min)
1. Auf render.com mit GitHub anmelden.
2. „New +“ → „Web Service“ → dein Repo `consentscan` wählen.
3. Einstellungen: Runtime Node, Build `npm install`, Start `npm start`, Plan Free.
4. Unter „Environment“ eine Variable `APP_PASSWORD` mit einem eigenen Passwort anlegen (schützt deine App vor Fremdnutzung).
5. „Deploy“. Nach 2–3 Minuten bekommst du eine Adresse wie `consentscan.onrender.com`. Fertig, der Live-Scan funktioniert.

Hinweis: Der Gratis-Plan schläft nach 15 Min Inaktivität ein, der erste Aufruf dauert dann ca. 50 Sekunden. Für zahlende Kunden später auf den Starter-Plan (ca. 7 $/Monat) wechseln.

## 3. Bezahlung mit Stripe (5 Min, ohne Code)
1. Konto auf stripe.com anlegen.
2. „Zahlungslinks“ → 3 Links erstellen: 19 €, 49 €, 99 € pro Monat (wiederkehrend).
3. In `public/index.html` die Zeile `const PAY_LINKS=['','','']` mit den drei Links füllen (direkt auf GitHub per Stift-Symbol bearbeiten). Render aktualisiert automatisch.

## 4. Eigene Domain (optional)
Domain bei z. B. Namecheap/IONOS kaufen, in Render unter „Custom Domains“ eintragen.

## Was die App prüft
Tracker (Google Analytics, Meta-Pixel, Fonts, Maps, YouTube, Hotjar), Cookie-Banner, Impressum, Datenschutzerklärung, Formulare, Cookies beim Erstaufruf, HTTPS, HSTS.

## Grenzen
- Prüft den HTML-Quelltext der Startseite, nicht das Nachladen per JavaScript nach Klicks.
- Gespeicherte Kundenscans liegen im Browser. Für Mehrbenutzer-Konten später Supabase ergänzen.
- Kein Rechtsrat. Im Bericht und in den AGB darauf hinweisen.
