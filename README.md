<h1 align="center">Edubase to PDF + OCR</h1>

<p align="center">
  <strong>Dein Buch. Lokal als durchsuchbare PDF.</strong><br>
  <sub>Your book. A local, searchable PDF.</sub>
</p>

<p align="center">
  <a href="https://sebii1998.github.io/edubase-to-pdf-ocr/"><img src="docs/images/website-de.svg" alt="Webseite öffnen – Download, Anleitung und Screenshots an einem Ort" width="820"></a>
</p>

<p align="center">
  <strong><a href="https://sebii1998.github.io/edubase-to-pdf-ocr/">Webseite öffnen</a> · <a href="https://sebii1998.github.io/edubase-to-pdf-ocr/en/">Visit the English website</a> · <a href="https://www.youtube.com/watch?v=0XhHn8oYu90">▶ YouTube-Tutorial</a></strong>
</p>

<p align="center">
  <a href="https://github.com/Sebii1998/edubase-to-pdf-ocr/releases/tag/v1.8.0"><img src="https://img.shields.io/badge/Version-1.8.0-4163ad?style=flat-square" alt="Version 1.8.0"></a>
  <img src="https://img.shields.io/badge/Windows-64--bit-263246?style=flat-square" alt="Windows 64-bit">
  <img src="https://img.shields.io/badge/Sprache-DE%20%2F%20EN-263246?style=flat-square" alt="Deutsch und English">
</p>

<p align="center">
  <a href="#deutsch">Deutsch</a> · <strong><a href="#english">English below ↓</a></strong>
</p>

---

## Deutsch

**Edubase to PDF + OCR** hilft dir, Edubase-Buchseiten als **durchsuchbare PDF** lokal zu speichern. So kannst du deine Lernunterlagen offline nutzen und langfristig in deinem persönlichen Archiv aufbewahren – auch wenn der Edubase-Reader später verändert oder eingestellt wird.

Nach deiner Anmeldung im Edubase-Reader nimmt die Windows-App die angezeigten Seiten des ausgewählten Buches automatisch als Bilder auf. Daraus erstellt sie auf deinem PC eine PDF und ergänzt mit Texterkennung (OCR) durchsuchbaren Text. Die aufgenommenen Buchseiten werden dabei nicht auf GitHub hochgeladen.

Automatische Titelerkennung, einstellbare Buchseitennummerierung und optionale Mathe-Erkennung ergänzen den Export.

**Neu in 1.8.0 – Finale Version:** Mit **Eigene PDF auswählen…** kannst du jetzt auch eine PDF von deinem PC mit Text-OCR verarbeiten. Mathe-OCR läuft nur, wenn du sie zusätzlich aktivierst. Die App wechselt automatisch in den PDF-Modus; dafür sind kein Browser und keine Aufnahme nötig. Die Originaldatei bleibt unverändert. Die bisherige Edubase-Aufnahme bleibt erhalten.

> **Für persönlichen Gebrauch und Archivierung:** Speichere nur Inhalte, auf die du zugreifen und die du speichern darfst. Das Projekt ist nicht für unerlaubte Weitergabe, Piraterie oder andere rechtswidrige Zwecke bestimmt.

<p>
  <a href="https://github.com/Sebii1998/edubase-to-pdf-ocr/releases/download/v1.8.0/Edubase-PDF-Windows.zip"><img src="docs/images/download-de.svg" alt="Windows-App herunterladen" width="340"></a>
</p>

[ZIP · ca. 241,7 MB](https://github.com/Sebii1998/edubase-to-pdf-ocr/releases/download/v1.8.0/Edubase-PDF-Windows.zip) · [Alle Downloads](https://github.com/Sebii1998/edubase-to-pdf-ocr/releases/tag/v1.8.0)

**Windows 64 Bit (Intel/AMD).** Python, Texterkennung und Firefox sind enthalten.
Installiertes Edge oder Chrome werden ebenfalls unterstützt.

> Die fertige App findest du über den Download oben. **Code → Download ZIP** und **Source code** enthalten nur die öffentliche Dokumentation.

### Video-Anleitung

<p align="center">
  <a href="https://www.youtube.com/watch?v=0XhHn8oYu90"><img src="docs/images/tutorial-thumbnail.png" alt="Edubase als PDF mit OCR – YouTube-Tutorial starten" width="820"></a><br>
  <a href="https://www.youtube.com/watch?v=0XhHn8oYu90"><img src="docs/images/tutorial-de.svg" alt="Tutorial auf YouTube ansehen · 2:32 Minuten · Deutsch" width="820"></a>
</p>

<details>
<summary><strong>App-Oberfläche ansehen</strong></summary>

<p align="center">
  <a href="site/assets/app-de.png"><img src="site/assets/app-de.png" alt="Edubase to PDF + OCR – deutsche Oberfläche mit Seitenauswahl und PDF-Export" width="820"></a>
</p>

</details>

### Edubase: In drei Schritten starten

1. **Entpacken:** ZIP vollständig entpacken und **`Edubase-PDF.exe`** starten.
2. **Buch öffnen:** **Browser öffnen** → bei Edubase anmelden → Buch in der **Einzelseitenansicht** öffnen.
3. **Drei Seiten testen:** Reader-Seiten **1–3** wählen, **Vorschau** prüfen und **Aufnehmen + OCR-PDF** starten.

Deine PDF liegt standardmässig unter **`Dokumente/Edubase-PDF`**. Lesbarkeit und Textsuche prüfen;
danach über **Neuer Auftrag** einen grösseren Bereich oder das ganze Buch aufnehmen.
Während der Aufnahme nicht selbst blättern.

### Eigene PDF mit OCR verarbeiten

1. **Eigene PDF auswählen…** anklicken. Die App zeigt die Seitenzahl und wählt zunächst alle Seiten aus; bei Bedarf den Bereich einschränken.
2. **Textsprache** einstellen. Text-OCR läuft immer; **Mathe & Formeln erkennen** nur bei Bedarf aktivieren.
3. **PDF mit OCR verarbeiten** starten. Das Ergebnis ist eine neue PDF; deine Originaldatei bleibt unverändert.

Der PDF-Modus braucht keinen Browser und keine Edubase-Anmeldung. Die ursprünglichen Seiten bleiben erhalten und werden um unsichtbaren Suchtext ergänzt. Vorhandener Text kann beim Kopieren oder Extrahieren dadurch doppelt vorkommen. **Neuer Auftrag** wechselt zurück zur Edubase-Aufnahme.

> **Leistung wählen:** Unter **Erweiterte Einstellungen → OCR-Leistung** nutzt **Automatisch** ein funktionierendes GPU-Modul für Mathe-OCR. Die App erkennt Grafikkarten und bevorzugt die von Windows für hohe Leistung vorgesehene GPU; das Protokoll zeigt die tatsächlich verwendete Karte. **CPU – maximale Leistung** verarbeitet Textseiten passend zu CPU und Arbeitsspeicher parallel. Für Mathe-OCR auf der GPU stehen **Standard (10 Formeln)**, **Hoch (20 Formeln)** und **Maximum (30 Formeln)** zur Wahl. Grössere Gruppen brauchen mehr Grafikspeicher und sind nicht auf jedem Gerät schneller. Bildqualität und Erkennungsmodelle bleiben gleich. Formelgruppen werden über bis zu vier bereits aufgenommene Seiten gefüllt; ähnlich lange Ausschnitte werden gemeinsam verarbeitet.

| Funktion | Das bringt sie dir |
| --- | --- |
| **PDF + OCR** | Buchseiten mit durchsuchbarem Text; Verarbeitung lokal auf deinem PC. |
| **Eigene PDF** | PDF vom PC mit Text-OCR und optionaler Mathe-OCR verarbeiten; das Original bleibt erhalten. |
| **Flexible Aufnahme** | Seitenbereich wählen, pausieren oder bereits aufgenommene Seiten exportieren. |
| **Buchseitennummern** | Einstellen, welche Reader-Seite der gedruckten Buchseite 1 entspricht. |
| **Mathe optional** | Formeln durchsuchen; LaTeX-Anhang separat wählbar. |

> **Am Schluss bleibt nur die PDF.** Nach erfolgreichem Export werden Arbeitsbilder und Zwischendateien gelöscht – auch bei einem Teilexport. Möchtest du später fortsetzen, aktiviere **vor dem Export** unter **Erweiterte Einstellungen → Arbeitsbilder behalten** den Haken.

<details>
<summary><strong>Aufnahme, Fortsetzen und Sprache</strong></summary>

- **Wartezeit:** Die eingestellten 2 Sekunden sind standardmässig die maximale zusätzliche Beruhigungszeit nach den Ladeprüfungen. Vollständig geladene, stabile Bild- oder SVG-Seiten können früher fertig sein. Bei Canvas oder unbekannter Darstellung bleibt die volle Wartezeit; notwendige Lade- und Stabilitätsprüfungen können die Gesamtzeit pro Seite verlängern.
- **Text-OCR während der Aufnahme:** Üblicherweise laufen bis zu zwei Seiten parallel, bei Rückstand und genügend CPU/RAM bis zu vier. Wartende Seiten werden schon während der Aufnahme abgearbeitet; bei knappen Ressourcen erfolgt die restliche OCR beim Export.
- **Ganzes Buch:** Vor **Browser öffnen** den Haken **Ganzes Buch automatisch aufnehmen** setzen. Beim Start ist er ausgeschaltet.
- **Früher fertig:** **Stoppen → Bisherige Seiten als PDF** exportiert bereits aufgenommene Seiten.
- **Fortsetzen:** Nach Stopp oder Fehler bleiben Arbeitsdateien erhalten. Über **Aufnahme fortsetzen…** den Auftrag wieder öffnen.
- **Deutsch / English:** Auswahl oben rechts; die App startet immer auf Deutsch. Die kleinen **ⓘ** erklären die Funktionen.
- **Buchzählung:** Der eingestellte Versatz passt die PDF-Seitenlabels an. Unnummerierte Einschübe werden damit nicht automatisch erkannt.

</details>

<details>
<summary><strong>Mathe & Formeln erkennen – optional</strong></summary>

**Mathe-OCR einrichten** lädt das Zusatzmodul (ca. 575 MB).
Danach **Mathe & Formeln erkennen** aktivieren.

**GPU verwenden** beschleunigt ausschliesslich Mathe-OCR. **GPU-Modul einrichten**
lädt das DirectML-Modul für geeignete Intel-, AMD- und NVIDIA-Grafik.
Bei GPU-Problemen übernimmt die CPU. Im Modus **Automatisch** wird eine eingerichtete,
unterstützte GPU ebenfalls genutzt; sonst bleibt CPU-Reserve.

**NVIDIA RTX – optionales CUDA:** Unter **Erweiterte Einstellungen** zuerst
**CUDA-Modul einrichten**, danach **CUDA verwenden (NVIDIA RTX)** anwählen.
Die Auswahl ist nur bei erkannter NVIDIA-RTX-Karte möglich und standardmässig aus.
Das separate CUDA-Modul hält Formelmerkmale während der Erkennung im Grafikspeicher.
Hat CUDA bereits Formelseiten erfolgreich erkannt und fällt später aus, versucht die App
die CUDA-Erkennung pro Lauf höchstens einmal neu zu starten. Fertige Ergebnisse bleiben
erhalten. Bei Startproblemen oder erneutem Erkennungsfehler werden verfügbare Alternativen
bis hin zu DirectML und CPU versucht. Stoppen und Zeitlimits lösen keinen Neustart aus.
AMD und Intel verwenden weiterhin DirectML und nutzen ebenfalls die neuen Formelgruppen.
Der tatsächliche Tempogewinn hängt von GPU und Buch ab.

Erkannte Formeln werden als **unsichtbarer Suchtext** ergänzt; das Seitenbild bleibt unverändert.
Mit **Strg+F** z. B. nach `σ` oder `F/A` suchen. Komplexe Formeln werden vereinfacht;
Treffer hängen von Erkennung und PDF-Programm ab.

**LaTeX-Dateien zusätzlich als PDF-Anhang** ist separat wählbar und standardmässig aus.
Der Anhang enthält LaTeX und Seitenzuordnung zum Weiterverwenden und ist für Strg+F nicht nötig.
Ergebnisse prüfen; die App löst keine Aufgaben.

Die Mathe-, GPU- und CUDA-Zusatzpakete bleiben unverändert auf Version 1.7.0; bereits eingerichtete Module kannst du weiterverwenden.

[Mathe-Zusatzmodul herunterladen](https://github.com/Sebii1998/edubase-to-pdf-ocr/releases/download/v1.7.0/Edubase-Mathe-OCR-Windows.zip)

</details>

**[Ausführliche Anleitung](docs/ANLEITUNG.md)** · [Fehler melden](https://github.com/Sebii1998/edubase-to-pdf-ocr/issues) · [Webseite](https://sebii1998.github.io/edubase-to-pdf-ocr/)

*Windows-App ohne digitale Signatur. Unabhängiges Projekt.*

---

## English

<p align="center">
  <a href="https://sebii1998.github.io/edubase-to-pdf-ocr/en/"><img src="docs/images/website-en.svg" alt="Visit the English website – downloads, instructions and screenshots in one place" width="820"></a>
</p>

**[Visit the English website](https://sebii1998.github.io/edubase-to-pdf-ocr/en/)**

**Edubase to PDF + OCR** helps you save Edubase book pages locally as **searchable PDFs**. Keep your learning materials available offline and in your personal archive, even if the Edubase Reader changes or is discontinued in the future.

After you sign in to the Edubase Reader, the Windows app automatically captures the displayed pages of your selected book as images. It creates a PDF on your PC and uses optical character recognition (OCR) to add searchable text. The captured book pages are not uploaded to GitHub.

Automatic title detection, configurable PDF page labels and optional maths recognition complete the export.

**New in 1.8.0 – Final release:** Use **Select your own PDF…** to process a PDF from your PC with text OCR. Maths OCR runs only when you enable it. The app switches to PDF mode automatically; no browser or capture is needed. The original file stays unchanged. Edubase capture remains available.

> **For personal use and archiving:** Only save content you can access and are permitted to save. This project is not intended for unauthorised sharing, piracy or other unlawful purposes.

<p>
  <a href="https://github.com/Sebii1998/edubase-to-pdf-ocr/releases/download/v1.8.0/Edubase-PDF-Windows.zip"><img src="docs/images/download-en.svg" alt="Download the Windows app" width="340"></a>
</p>

[ZIP · about 241.7 MB](https://github.com/Sebii1998/edubase-to-pdf-ocr/releases/download/v1.8.0/Edubase-PDF-Windows.zip) · [All downloads](https://github.com/Sebii1998/edubase-to-pdf-ocr/releases/tag/v1.8.0)

**64-bit Windows (Intel/AMD).** Python, text recognition and Firefox are included.
Installed Edge and Chrome are also supported.

> Get the app using the download above. **Code → Download ZIP** and **Source code** contain only the public documentation.

### Video tutorial

<p align="center">
  <a href="https://www.youtube.com/watch?v=0XhHn8oYu90"><img src="docs/images/tutorial-thumbnail.png" alt="Edubase to PDF with OCR – watch the YouTube tutorial in German" width="820"></a><br>
  <a href="https://www.youtube.com/watch?v=0XhHn8oYu90"><img src="docs/images/tutorial-en.svg" alt="Watch on YouTube · 2:32 · German on-screen explanations" width="820"></a>
</p>

<details>
<summary><strong>View the app interface</strong></summary>

<p align="center">
  <a href="site/assets/app-en.png"><img src="site/assets/app-en.png" alt="Edubase to PDF + OCR – English interface with page selection and PDF export" width="820"></a>
</p>

</details>

### Edubase: Get started in three steps

1. **Extract:** Extract the entire ZIP and launch **`Edubase-PDF.exe`**. Select **English** at the top right.
2. **Open your book:** **Open browser** → sign in to Edubase → open your book in **single-page view**.
3. **Test three pages:** Select Reader pages **1–3**, check the **Preview** and click **Capture + OCR PDF**.

Your PDF is saved to **`Documents/Edubase-PDF`** by default. Check readability and text search,
then use **New job** to capture a larger range or the whole book.
Do not turn pages manually while capturing.

### Process your own PDF with OCR

1. Click **Select your own PDF…**. The app shows its page count and selects all pages; narrow the range if needed.
2. Set the **Text language**. Text OCR always runs; enable **Recognise maths & formulas** only if needed.
3. Start **Process PDF with OCR**. The result is a new PDF; your original file stays unchanged.

PDF mode needs no browser or Edubase sign-in. Original pages are retained and invisible searchable text is added. If text already exists, copying or extracting it can produce duplicates. **New job** returns to Edubase capture.

> **Choose performance:** Under **Advanced settings → OCR performance**, **Automatic** uses a working GPU module for maths OCR. The app detects graphics cards and prefers the GPU Windows selects for high performance; the log identifies the card actually used. **CPU – maximum performance** processes text pages in parallel according to your CPU and available memory. GPU maths OCR offers **Standard (10 formulas)**, **High (20 formulas)** and **Maximum (30 formulas)**. Larger groups need more graphics memory and are not faster on every device. Image quality and recognition models stay the same. Formula groups draw from up to four already captured pages and group crops of similar estimated length.

| Feature | What it does |
| --- | --- |
| **PDF + OCR** | Book pages with searchable text, processed locally on your PC. |
| **Your own PDF** | Process a local PDF with text OCR and optional maths OCR; keep the original file. |
| **Flexible capture** | Choose a page range, pause or export the pages already captured. |
| **Book page labels** | Set which Reader page contains printed book page 1. |
| **Optional maths** | Search recognised formulas; choose LaTeX attachments separately. |

> **Only the PDF remains.** Working images and temporary files are deleted after a successful export, including partial exports. To resume later, enable **Advanced settings → Keep working images before exporting**.

<details>
<summary><strong>Capture, resume and language</strong></summary>

- **Wait time:** The default 2 seconds are the maximum additional settling time after loading checks. Fully loaded, stable image or SVG pages can finish earlier. Canvas or unfamiliar page formats retain the full wait; mandatory loading and stability checks can make the total time per page longer.
- **Text OCR during capture:** Usually up to two pages run in parallel, increasing to four when a backlog grows and CPU/RAM allow. Queued pages are processed while capture continues; with limited resources, remaining OCR runs during export.
- **Whole book:** Enable **Capture the entire book automatically** before clicking **Open browser**. This option starts switched off.
- **Finish early:** **Stop → Saved pages to PDF** exports the pages already captured.
- **Resume:** Stopping or an error preserves the working files. Open the job using **Resume capture…**.
- **German / English:** Switch at the top right; every launch starts in German. The small **ⓘ** icons explain the controls.
- **Book numbering:** The selected offset adjusts PDF page labels. It does not automatically detect unnumbered inserts.

</details>

<details>
<summary><strong>Recognise maths & formulas – optional</strong></summary>

**Set up math OCR** downloads the add-on (about 575 MB).
Then enable **Recognise maths & formulas**.

**Use GPU** accelerates math OCR only. **Set up GPU module** downloads the DirectML
module for compatible Intel, AMD and NVIDIA graphics. GPU failures fall back to
CPU. **Automatic** also uses a configured, compatible GPU; otherwise it leaves CPU headroom.

Recognised formulas are added as **invisible searchable text**; the page image stays unchanged.
Use **Ctrl+F** for e.g. `σ` or `F/A`. Complex formulas are simplified; results depend
on recognition and the PDF viewer.

**NVIDIA RTX – optional CUDA:** In **Advanced settings**, choose **Set up CUDA
module**, then enable **Use CUDA (NVIDIA RTX)**. This option is off by default and
only selectable when an NVIDIA RTX card is detected. The separate module keeps
formula features in graphics memory during recognition. If CUDA has completed formula
pages and later fails, the app attempts to restart CUDA recognition at most once per
run, preserving completed results. Startup problems or a repeated recognition failure
trigger available alternatives, including DirectML and CPU. Stop and timeouts do not
trigger a restart. AMD and Intel continue to use DirectML and benefit from the same new formula groups. Actual speed depends on
your GPU and book.

**Also attach LaTeX files to the PDF** is a separate option, off by default.
Attachments contain LaTeX and page references for reuse and are not needed for Ctrl+F.
Check the results; the app does not solve exercises.

Maths, GPU and CUDA add-ons remain unchanged at version 1.7.0; you can keep using modules already installed.

[Download the maths add-on](https://github.com/Sebii1998/edubase-to-pdf-ocr/releases/download/v1.7.0/Edubase-Mathe-OCR-Windows.zip)

</details>

**[Full guide (German)](docs/ANLEITUNG.md)** · [Report an issue](https://github.com/Sebii1998/edubase-to-pdf-ocr/issues) · [English website](https://sebii1998.github.io/edubase-to-pdf-ocr/en/)

*Unsigned Windows app. Independent project.*

---

<p align="center">
  <a href="LICENSE">MIT License</a> · <a href="THIRD_PARTY_NOTICES.md">Third-party notices</a> · <a href="#edubase-to-pdf--ocr">↑ Nach oben / Back to top</a>
</p>
