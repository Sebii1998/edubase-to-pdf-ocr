# v1.8.0 – Finale Version

[Deutsch](#deutsch) · [English](#english)

## Deutsch

**Deine Unterlagen. Durchsuchbar, zusammengefügt und bereit zum Lernen.**

- **Eigene PDFs durchsuchbar machen:** Wähle eine PDF von deinem PC und starte die
  Texterkennung. Mathe-OCR kannst du bei Bedarf zuschalten. Die App erkennt den
  PDF-Modus automatisch – alles lokal, ohne Browser oder Edubase-Anmeldung.
- **PDFs zusammenfügen:** Kombiniere mehrere Dokumente in deiner gewünschten
  Reihenfolge zu einer neuen PDF. Seiten und vorhandener Suchtext bleiben erhalten.
  Die Originaldateien bleiben unverändert.
- **Mathe-OCR auf deinen PC abstimmen:** Nutze CPU, GPU oder optional CUDA für
  NVIDIA RTX. Unter **Erweiterte Einstellungen / Performance-Einstellungen** wählst
  du für die GPU bis zu **10, 20 oder 30 Formeln pro Gruppe**. Grössere Gruppen
  brauchen mehr Grafikspeicher; das Tempo hängt von deinem PC und den Formeln ab.
  Bildqualität und Erkennungsmodelle bleiben gleich.

**Aktualisiert am 10. Oktober 2026: gezieltere CUDA-Wiederherstellung.**

Bei schweren CUDA-Fehlern wie Fehler 715 startet die App die Mathe-Erkennung in
einem neuen Prozess mit höchstens **10 Formeln pro Gruppe**. Scheitert dieselbe
Seitengruppe erneut, übernimmt eine verfügbare Alternative wie DirectML oder CPU.
Bei weiteren Seiten kann die App CUDA wieder versuchen. Pro Mathe-Durchlauf sind
höchstens **drei zusätzliche CUDA-Starts** erlaubt. Fertige Ergebnisse bleiben erhalten.
Stoppen und Zeitlimits lösen keinen Neustart aus.

Die bewährte **Edubase-Aufnahme** bleibt vollständig erhalten. Seitenbereich,
Pause, Stopp und Fortsetzen stehen auch für eigene PDFs bereit. **Neuer Auftrag**
wechselt zurück zur Aufnahme. Bereits eingerichtete Mathe-, GPU- und CUDA-Module
kannst du weiterverwenden.

Bei eigenen PDFs bleiben die Originalseiten, Vektorgrafiken und vorhandener Text
erhalten; OCR ergänzt unsichtbaren Suchtext. Bereits durchsuchbare PDFs können
beim Kopieren oder Extrahieren doppelte Textstellen liefern. Prüfe OCR-Ergebnisse.

**Loslegen:** [Windows-App herunterladen](https://github.com/Sebii1998/edubase-to-pdf-ocr/releases/download/v1.8.0/Edubase-PDF-Windows.zip)
→ ZIP vollständig entpacken → **Edubase-PDF.exe** öffnen.
Der Download ist ca. **241,7 MB** gross. Python, Text-OCR mit Deutsch/Englisch,
PDFium und Firefox sind enthalten. Installiertes Edge oder Chrome kannst du für
Edubase ebenfalls verwenden.

[Anleitung](https://github.com/Sebii1998/edubase-to-pdf-ocr/blob/main/docs/ANLEITUNG.md)
· [Webseite](https://sebii1998.github.io/edubase-to-pdf-ocr/)

## English

**Your documents. Searchable, combined and ready to study.**

- **Make your own PDFs searchable:** Select a PDF from your PC and start text
  recognition. Add maths OCR when you need it. The app switches to PDF mode
  automatically – all locally, without a browser or Edubase account.
- **Merge PDFs:** Bring several documents together in the order you choose and
  save a new PDF. Pages and existing searchable text are retained.
  Your original files stay unchanged.
- **Tune maths OCR for your PC:** Use CPU, GPU or optional CUDA for NVIDIA RTX.
  Under **Advanced settings / Performance settings**, choose up to **10, 20 or
  30 formulas per group** for GPU processing. Larger groups need more graphics
  memory; speed depends on your PC and formulas. Image quality and recognition
  models stay the same.

**Updated on 10 October 2026: improved CUDA recovery.**

After a fatal CUDA error such as error 715, the app restarts maths recognition in
a new process with up to **10 formulas per group**. If the same page group fails
again, an available alternative such as DirectML or CPU takes over. The app can try
CUDA again on further pages, with at most **three additional CUDA starts** per maths
OCR run. Completed results are kept. Stop and timeouts do not trigger a restart.

**Edubase capture** remains fully available. Page ranges, pause, stop and resume
also work for your own PDFs. **New job** returns to capture mode. Keep using your
installed maths, GPU and CUDA modules.

Your own PDFs retain their original pages, vector graphics and existing text;
OCR adds invisible searchable text. Copying or extracting text from an already
searchable PDF can produce duplicates. Please check OCR results.

**Get started:** [Download the Windows app](https://github.com/Sebii1998/edubase-to-pdf-ocr/releases/download/v1.8.0/Edubase-PDF-Windows.zip)
→ extract the entire ZIP → open **Edubase-PDF.exe**.
The download is about **241.7 MB**. Python, German/English text OCR, PDFium and
Firefox are included. You can also use installed Edge or Chrome for Edubase.

[English website](https://sebii1998.github.io/edubase-to-pdf-ocr/en/)

## Optionale Zusatzpakete / Optional add-ons

Die unveränderten Pakete werden weiter aus v1.7.0 geladen. Am einfachsten erfolgt
die Einrichtung über die entsprechenden Knöpfe in der App.

The unchanged packages continue to download from v1.7.0. The easiest way to
install them is through the setup buttons in the app.

- [Mathe / Maths OCR · ca. 575 MB](https://github.com/Sebii1998/edubase-to-pdf-ocr/releases/download/v1.7.0/Edubase-Mathe-OCR-Windows.zip)
- [GPU / DirectML · ca. 23 MB](https://github.com/Sebii1998/edubase-to-pdf-ocr/releases/download/v1.7.0/Edubase-GPU-OCR-Windows.zip)
- [CUDA / NVIDIA RTX · ca. 1,68 GB](https://github.com/Sebii1998/edubase-to-pdf-ocr/releases/download/v1.7.0/Edubase-CUDA-OCR-Windows.zip)

Mit **Archiv** gekennzeichnete Dateien gehören zu früheren Builds. Für die aktuelle
Version lade **Edubase-PDF-Windows.zip** und die zugehörige **SHA256SUMS.txt**.

Files labelled **Archiv** belong to earlier builds. For the current version, use
**Edubase-PDF-Windows.zip** and its **SHA256SUMS.txt**.

## SHA256

`Edubase-PDF-Windows.zip` · 241726899 bytes

```text
0ff11c6e782a0ad00c6e9b96aedad0e6c195cee23f3dc490d81b4d387041807b
```

[SHA256SUMS.txt](https://github.com/Sebii1998/edubase-to-pdf-ocr/releases/download/v1.8.0/SHA256SUMS.txt)

Windows 64 Bit / 64-bit Windows (Intel/AMD). Die App ist nicht digital signiert.
The app is not digitally signed.
