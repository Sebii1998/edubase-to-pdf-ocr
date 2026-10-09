# Version 1.7.0 · Windows-Vorschau / Windows preview

[Deutsch](#deutsch) · [English below ↓](#english)

## Deutsch

**Neu in 1.7.0**

- **Adaptive Wartezeit:** Die eingestellte Wartezeit pro Seite (Vorgabe 2 Sekunden)
  ist die maximale zusätzliche Beruhigungszeit nach dem Laden. Vollständig geladene,
  stabile Bild-/SVG-Seiten können früher aufgenommen werden. Unklare Darstellungen
  und Canvas-Seiten behalten die volle Wartezeit; notwendige Lade- und
  Stabilitätsprüfungen können insgesamt länger dauern.
- **Text-OCR während der Aufnahme:** Bei Rückstand und genügend CPU/RAM können
  bis zu vier statt normalerweise bis zu zwei Seiten parallel verarbeitet werden.
  Zurückgestellte Seiten werden bereits während der Aufnahme nachgearbeitet;
  bei anhaltendem Ressourcenmangel übernimmt der normale Export.
- **CUDA-Wiederherstellung:** Nach bereits erfolgreich erkannten Seiten versucht die App,
  einen fehlgeschlagenen CUDA-Prozess höchstens einmal pro Erkennungslauf neu zu starten.
  Fertige Ergebnisse bleiben erhalten. Bei weiteren Problemen werden verfügbare
  Alternativen wie DirectML oder CPU versucht. Stoppen und Zeitlimits lösen keinen Neustart aus.
- Auflösung, Farben, PNG-Komprimierung und OCR-Modelle bleiben unverändert.

- GPU-Formelgruppen über bis zu vier bereits aufgenommene Seiten; ähnlich lange
  Ausschnitte werden gemeinsam verarbeitet. Die ursprüngliche Formel- und
  Seitenreihenfolge bleibt erhalten.
- Optionales **CUDA für NVIDIA RTX**, standardmässig aus und ohne erkannte
  RTX-Karte nicht auswählbar. Separates Zusatzpaket, unverändertes Formelmodell
  und volle FP32-Genauigkeit; Rückfall auf DirectML oder CPU bei Problemen.

- Grafikkarten werden automatisch erkannt und angezeigt; Mathe-OCR bevorzugt die von Windows für hohe Leistung vorgesehene GPU. Das Protokoll nennt die tatsächlich verwendete Karte.
- GPU-Mathe-OCR mit **Standard (10 Formeln)**, **Hoch (20 Formeln)** und **Maximum (30 Formeln)**. Bei Problemen wird die Gruppe automatisch verkleinert; Erkennungsmodelle und Bildqualität bleiben gleich. Der Tempogewinn hängt vom Gerät und den Formeln ab.
- Effizientere Seitenaufnahme in Chrome, Edge und Firefox bei gleicher Auflösung und Farbe.
- Text und erkannte Formeln werden in einem Durchgang in die PDF geschrieben.
- Weniger wiederholte Dateizugriffe; Formel-Begleitdateien nur bei gewähltem PDF-Anhang.
- Zwei Fortschrittsbalken für Aufnahme und OCR, mit getrennten Text-/Mathe-Seitenzählern.
- Die normale Ansicht passt auch direkt nach dem Start ohne Scrollen.

Für dieses App-Update bleiben Mathe-, DirectML- und CUDA-Zusatzpakete unverändert; vorhandene Module funktionieren weiter. CUDA ist optional. AMD und Intel nutzen weiterhin DirectML.

**Edubase-Buchseiten lokal als durchsuchbare PDF speichern.** Für Windows 64 Bit
(Intel/AMD); Python, Texterkennung und Firefox sind enthalten. Installiertes
Edge oder Chrome werden ebenfalls unterstützt.

- **`Edubase-PDF-Windows.zip`** (ca. 237,6 MB) herunterladen, vollständig entpacken und
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

- **Adaptive wait:** The configured per-page wait (default 2 seconds) is the
  maximum additional settling time after loading. Fully loaded, stable image/SVG
  pages can be captured sooner. Uncertain layouts and canvas pages keep the full
  wait; required loading and stability checks can take longer overall.
- **Text OCR during capture:** With a backlog and sufficient CPU/memory, up to
  four pages can run in parallel instead of the usual maximum of two. Queued
  pages are processed while capture continues; the normal export handles pages
  deferred by persistent resource limits.
- **CUDA recovery:** After successfully recognised pages, the app can attempt to restart a failed CUDA
  process at most once per recognition run. Completed results are preserved. Further
  problems cause the app to try available alternatives such as DirectML or CPU. Cancellation
  and timeouts do not trigger a restart.
- Resolution, colours, PNG compression and OCR models are unchanged.

- GPU formula groups span up to four already captured pages and group crops of
  similar estimated length. Original formula and page order are preserved.
- Optional **CUDA for NVIDIA RTX**, off by default and unavailable without a
  detected RTX card. Separate add-on, unchanged formula model and full FP32
  precision; falls back to DirectML or CPU if needed.

- Graphics cards are detected and displayed automatically; maths OCR prefers the GPU Windows selects for high performance. The log identifies the card actually used.
- GPU maths OCR offers **Standard (10 formulas)**, **High (20 formulas)** and **Maximum (30 formulas)**. Groups shrink automatically if needed; recognition models and image quality stay the same. Speed gains depend on your device and formulas.
- More efficient capture in Chrome, Edge and Firefox, preserving resolution and colour.
- Text and recognised formulas are written to the PDF in a single pass.
- Fewer repeated file reads; formula companion files are created only when PDF attachments are selected.
- Two progress bars for capture and OCR, with individual text/math page counters.
- The normal view fits without scrolling immediately after launch.

For this app update, the maths, DirectML and CUDA add-ons are unchanged; existing installations remain compatible. CUDA is optional. AMD and Intel continue to use DirectML.

**Save Edubase book pages as a local, searchable PDF.** For 64-bit Windows
(Intel/AMD); Python, text recognition and Firefox are included. Installed Edge
and Chrome are also supported.

- Download **`Edubase-PDF-Windows.zip`** (about 237.6 MB), extract everything and launch
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
