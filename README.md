# Lens Text – GitHub Pages OCR

Eine statische, Google-Lens-inspirierte Webseite, die ein Bild im Browser nimmt und daraus editierbaren Text extrahiert.

## Features

- Drag & Drop oder Dateiauswahl
- Bild aus der Zwischenablage einfügen
- OCR im Browser mit Tesseract.js
- Deutsch, Englisch, Deutsch + Englisch, Französisch und Spanisch
- Fortschrittsanzeige
- Erkannter Text ist editierbar
- Text kopieren und als `.txt` speichern
- Responsive Layout für Desktop und Smartphone
- Keine eigene Server-/Backend-API erforderlich

## GitHub Pages

Die Datei `index.html` muss im Veröffentlichungsordner liegen. GitHub Pages kann direkt aus einem Branch und dem Repository-Root veröffentlichen.

1. Repository erstellen oder ein bestehendes Repository verwenden.
2. `index.html` hochladen.
3. In **Settings → Pages** die Quelle **Deploy from a branch** wählen.
4. Branch (z. B. `main`) und Ordner `/ (root)` auswählen und speichern.

Tesseract.js wird per jsDelivr eingebunden, die Sprachdaten werden bei Bedarf ebenfalls aus dem CDN geladen. Die zu erkennende Bilddatei wird vom Frontend direkt an den Browser-Worker übergeben; diese Webseite enthält keinen eigenen Upload-Endpunkt.
