# Umschlag-Seriendruck

Webapp zum Bedrucken von Briefumschlägen als Seriendruck. Adressen aus `.ods`, `.xlsx`, `.xls`, `.csv`, `.odt` und `.docx`.
Zusätzlich lassen sich normale PDF-Dateien drucken (alle Seiten, ungerade/gerade Seiten für manuellen Duplexdruck, Seitenbereiche).
Alles läuft lokal im Browser, es werden keine Daten hochgeladen.

## Auf GitHub Pages veröffentlichen
1. Auf github.com ein neues Repository anlegen (z. B. `umschlag-seriendruck`).
2. „Add file“ → „Upload files“ und `index.html` sowie `README.md` hochladen, dann „Commit changes“.
3. „Settings“ → „Pages“ → Source: „Deploy from a branch“, Branch `main`, Ordner `/ (root)` → „Save“.
4. Nach ca. einer Minute ist die App unter `https://BENUTZERNAME.github.io/umschlag-seriendruck/` erreichbar.

Die App lädt die Bibliotheken JSZip und SheetJS von cdnjs.cloudflare.com, dafür ist beim ersten Aufruf Internet nötig.
Alternativ lässt sich `index.html` auch direkt per Doppelklick lokal im Browser öffnen.

## Hinweis zu Druckereinstellungen
Browser können Papierzufuhr (z. B. manueller Schacht) und Duplex nicht selbst am Drucker einstellen. Die App zeigt dazu eine Erinnerung an; die Einstellung selbst wählen Sie im Druckdialog.
Für manuellen Einzug gibt es den Einzeldruck: Pro Klick wird genau ein Umschlag gedruckt.

## Drucker immer auf A4
Unter „Gedruckt wird auf“ kann „A4-Blatt“ gewählt werden. Die App legt den Umschlag dann gedreht und positioniert auf eine A4-Seite, der Drucker muss nie umgestellt werden. Lage und Korrekturwerte per Probedruck anpassen.
