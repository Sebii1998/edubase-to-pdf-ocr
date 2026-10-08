# Version 1.7.0 · Windows-Vorschau / Windows preview

[Deutsch](#deutsch) · [English below ↓](#english)

## Deutsch

**Neu in 1.7.0**

- Grafikkarten werden automatisch erkannt und angezeigt; Mathe-OCR bevorzugt die von Windows für hohe Leistung vorgesehene GPU. Das Protokoll nennt die tatsächlich verwendete Karte.
- GPU-Mathe-OCR mit **Standard (5 Formeln)**, **Hoch (10 Formeln)** und **Maximum (20 Formeln)**. Bei Problemen wird die Gruppe automatisch verkleinert; Erkennungsmodelle und Bildqualität bleiben gleich. Der Tempogewinn hängt vom Gerät und den Formeln ab.
- Effizientere Seitenaufnahme in Chrome, Edge und Firefox bei gleicher Auflösung und Farbe.
- Text und erkannte Formeln werden in einem Durchgang in die PDF geschrieben.
- Weniger wiederholte Dateizugriffe; Formel-Begleitdateien nur bei gewähltem PDF-Anhang.
- Zwei Fortschrittsbalken für Aufnahme und OCR, mit getrennten Text-/Mathe-Seitenzählern.
- Die normale Ansicht passt auch direkt nach dem Start ohne Scrollen.

Mathe- und GPU-Zusatzpakete sind unverändert; vorhandene Module funktionieren weiter.

**Edubase-Buchseiten lokal als durchsuchbare PDF speichern.** Für Windows 64 Bit
(Intel/AMD); Python, Texterkennung und Firefox sind enthalten. Installiertes
Edge oder Chrome werden ebenfalls unterstützt.

- **`Edubase-PDF-Windows.zip`** herunterladen, vollständig entpacken und
  **`Edubase-PDF.exe`** starten. Zuerst drei Seiten aufnehmen und die PDF prüfen.
- **Deutsch / English** oben rechts auswählen; die App startet immer auf Deutsch.
- Nach erfolgreichem Export bleibt standardmässig **nur die PDF**. Zum späteren
  Fortsetzen vor dem Export **Arbeitsbilder behalten** aktivieren.
- Optional **Mathe-OCR einrichten** in der App wählen. Das Zusatzpaket
  **`Edubase-Mathe-OCR-Windows.zip`** ergänzt erkannten Formeltext für Strg+F
  (z. B. `σ` oder `F/A`), bei unverändertem Seitenbild. Komplexe Formeln werden
  vereinfacht; Ergebnisse prüfen.
- **LaTeX-Dateien zusätzlich als PDF-Anhang** separat anwählen, falls gewünscht.
  Standardmässig aus; für Strg+F nicht nötig.

- Die normale Ansicht passt sich der Fensterhöhe an. Zusätzlicher Inhalt wird erst
  bei geöffneten erweiterten Einstellungen oder geöffnetem Protokoll gescrollt.
- Chrome und Edge passen den Reader ausserhalb einer Aufnahme an die Fenstergrösse
  an. Die hohe Aufnahmeauflösung bleibt erhalten.

Diese Windows-Vorschau ist **nicht digital signiert**.
[Anleitung, Bilder und Downloads](https://github.com/Sebii1998/edubase-to-pdf-ocr/blob/main/README.md)

---

## English

**New in 1.7.0**

- Graphics cards are detected and displayed automatically; maths OCR prefers the GPU Windows selects for high performance. The log identifies the card actually used.
- GPU maths OCR offers **Standard (5 formulas)**, **High (10 formulas)** and **Maximum (20 formulas)**. Groups shrink automatically if needed; recognition models and image quality stay the same. Speed gains depend on your device and formulas.
- More efficient capture in Chrome, Edge and Firefox, preserving resolution and colour.
- Text and recognised formulas are written to the PDF in a single pass.
- Fewer repeated file reads; formula companion files are created only when PDF attachments are selected.
- Two progress bars for capture and OCR, with individual text/math page counters.
- The normal view fits without scrolling immediately after launch.

The maths and GPU add-on packages are unchanged; existing installations remain compatible.

**Save Edubase book pages as a local, searchable PDF.** For 64-bit Windows
(Intel/AMD); Python, text recognition and Firefox are included. Installed Edge
and Chrome are also supported.

- Download **`Edubase-PDF-Windows.zip`**, extract everything and launch
  **`Edubase-PDF.exe`**. Test three pages first and check the PDF.
- Select **Deutsch / English** at the top right; every launch starts in German.
- Successful exports leave **only the PDF** by default. Enable **Keep working
  images** before exporting if you want to resume later.
- For optional formulas, choose **Set up math OCR** in the app. The
  **`Edubase-Mathe-OCR-Windows.zip`** add-on adds recognised formula text for Ctrl+F
  (e.g. `σ` or `F/A`), keeping the page image unchanged. Complex formulas are
  simplified; check the results.
- Select **Also attach LaTeX files to the PDF** separately if wanted.
  Off by default; not needed for Ctrl+F.

- The normal view adapts to the window height. Scrolling is only needed for extra
  content when advanced settings or the log are expanded.
- Chrome and Edge fit the reader to the window outside capture. High-resolution
  capture is preserved.

This Windows preview is **not digitally signed**.
[Instructions, screenshots and downloads](https://github.com/Sebii1998/edubase-to-pdf-ocr/blob/main/README.md#english)

