# v1.8.0 – Finale Version

[Deutsch](#deutsch) · [English](#english)

## Deutsch

**Update der finalen Version: PDF-Werkzeuge und einfachere Bedienung.**

- **PDFs zusammenfügen…:** mindestens zwei PDFs auswählen, die Reihenfolge mit
  den Pfeilen anpassen und über **Zusammenfügen & speichern…** als neue Datei speichern.
  Seiten, vorhandener Text und Formel-Suchschichten bleiben erhalten. Keine neue OCR;
  Originale und bestehende Zieldateien werden nicht überschrieben. Pause und Stopp
  sind verfügbar; ein zuvor geladener OCR-Auftrag bleibt erhalten.
- **Protokoll kopieren:** alle bisherigen Meldungen mit Uhrzeit in die Zwischenablage
  kopieren, auch bei eingeklapptem Protokoll und während einer Verarbeitung.
  Die Meldungen folgen der aktuell gewählten Oberflächensprache.
- **Erweiterte Einstellungen / Performance-Einstellungen:** neue Beschriftung
  für die vorhandenen Aufnahme-, CPU-, GPU- und CUDA-Einstellungen.

**Ebenfalls in 1.8.0: eigene PDF vom PC mit OCR verarbeiten.**

- **Eigene PDF auswählen…** schaltet automatisch in den PDF-Modus. Kein Browser,
  keine Edubase-Anmeldung und keine Bildschirmaufnahme nötig.
- Text-OCR läuft für die gewählten Seiten. Mathe-OCR läuft zusätzlich nur,
  wenn **Mathe & Formeln erkennen** aktiviert ist.
- **PDF mit OCR verarbeiten** erstellt eine neue PDF mit unsichtbarem Suchtext.
  Die Originaldatei bleibt unverändert; vorhandene Ausgabedateien werden nicht überschrieben.
- Originalseiten, Vektorgrafiken und vorhandener Text bleiben erhalten.
  Bei bereits durchsuchbaren PDFs können beim Kopieren oder Extrahieren doppelte
  Textstellen entstehen.
- Seitenbereich, Pause, Stopp und Fortsetzen funktionieren auch für eigene PDFs.
  **Neuer Auftrag** wechselt zurück zur bisherigen Edubase-Aufnahme.
- Mathe-, GPU- und CUDA-Zusatzpakete bleiben unverändert. Bereits eingerichtete
  Module können weiterverwendet werden; kein erneuter Download nötig.

**Starten:** [Windows-App herunterladen](https://github.com/Sebii1998/edubase-to-pdf-ocr/releases/download/v1.8.0/Edubase-PDF-Windows.zip)
→ ZIP vollständig entpacken → **Edubase-PDF.exe** öffnen.
Der Download ist ca. **241,7 MB** gross. Python, Text-OCR mit Deutsch/Englisch,
PDFium und Firefox sind enthalten. Installiertes Edge oder Chrome kann für
Edubase weiterhin verwendet werden.

[Anleitung](https://github.com/Sebii1998/edubase-to-pdf-ocr/blob/main/docs/ANLEITUNG.md)
· [Webseite](https://sebii1998.github.io/edubase-to-pdf-ocr/)

## English

**Final release update: PDF tools and easier controls.**

- **Merge PDFs…:** select at least two PDFs, reorder them using the arrows and
  choose **Merge & save…** to save a new file. Pages, existing text and formula
  search layers are retained. No new OCR runs; originals and existing destination
  files are not overwritten. Pause and stop are available; a previously loaded
  OCR job is kept.
- **Copy log:** copy all messages collected so far, including timestamps, to the
  clipboard, even while the log is collapsed or a job is running. Messages follow
  the current interface language.
- **Advanced settings / Performance settings:** clearer label for the existing
  capture, CPU, GPU and CUDA settings.

**Also in 1.8.0: process a PDF from your PC with OCR.**

- **Select your own PDF…** switches to PDF mode automatically. No browser,
  Edubase sign-in or screen capture is needed.
- Text OCR runs for the selected pages. Maths OCR runs only when
  **Recognise maths & formulas** is enabled.
- **Process PDF with OCR** creates a new PDF with invisible searchable text.
  Your original file stays unchanged; existing output files are not overwritten.
- Original pages, vector graphics and existing text are preserved. Copying or
  extracting text from an already searchable PDF can produce duplicates.
- Page ranges, pause, stop and resume also work for your own PDFs.
  **New job** returns to the existing Edubase capture mode.
- Maths, GPU and CUDA add-ons remain unchanged. Keep using installed modules;
  there is no need to download them again.

**Get started:** [Download the Windows app](https://github.com/Sebii1998/edubase-to-pdf-ocr/releases/download/v1.8.0/Edubase-PDF-Windows.zip)
→ extract the entire ZIP → open **Edubase-PDF.exe**.
The download is about **241.7 MB**. Python, German/English text OCR, PDFium and
Firefox are included. Installed Edge or Chrome can still be used for Edubase.

[English website](https://sebii1998.github.io/edubase-to-pdf-ocr/en/)

## Optionale Zusatzpakete / Optional add-ons

Die unveränderten Pakete werden weiter aus v1.7.0 geladen. Am einfachsten erfolgt
die Einrichtung über die entsprechenden Knöpfe in der App.

The unchanged packages continue to download from v1.7.0. The easiest way to
install them is through the setup buttons in the app.

- [Mathe / Maths OCR · ca. 575 MB](https://github.com/Sebii1998/edubase-to-pdf-ocr/releases/download/v1.7.0/Edubase-Mathe-OCR-Windows.zip)
- [GPU / DirectML · ca. 23 MB](https://github.com/Sebii1998/edubase-to-pdf-ocr/releases/download/v1.7.0/Edubase-GPU-OCR-Windows.zip)
- [CUDA / NVIDIA RTX · ca. 1,68 GB](https://github.com/Sebii1998/edubase-to-pdf-ocr/releases/download/v1.7.0/Edubase-CUDA-OCR-Windows.zip)

## SHA256

`Edubase-PDF-Windows.zip` · 241723287 bytes

```text
d3cb94aa09daa03497ad43442f41903fd3f24ba3574709de91023f54a27273c9
```

[SHA256SUMS.txt](https://github.com/Sebii1998/edubase-to-pdf-ocr/releases/download/v1.8.0/SHA256SUMS.txt)

Windows 64 Bit / 64-bit Windows (Intel/AMD). Die App ist nicht digital signiert.
The app is not digitally signed.
