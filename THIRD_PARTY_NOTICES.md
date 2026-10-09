# Hinweise zu Drittprojekten

## Michael Beutler: edubase-to-pdf

Die ursprüngliche Idee und die vorhandenen Reader-Selektoren wurden anhand
des MIT-lizenzierten Go-Projekts `github.com/michaelbeutler/edubase-to-pdf`
geprüft. Diese Anwendung ist eine neue Python-Implementierung mit eigener
Bedienoberfläche, seitenweiser Wiederaufnahme und OCR.

Geprüfte archivierte Version:
`v0.0.0-20260528193334-4ff05200e57b`.

- Ursprüngliches Projekt: https://github.com/michaelbeutler/edubase-to-pdf
- Paketarchiv: https://pkg.go.dev/github.com/michaelbeutler/edubase-to-pdf@v0.0.0-20260528193334-4ff05200e57b
- Quellcode-Archiv: https://proxy.golang.org/github.com/michaelbeutler/edubase-to-pdf/@v/v0.0.0-20260528193334-4ff05200e57b.zip

Die Lizenz des archivierten Originals lautet vollständig:

```text
MIT License

Copyright (c) 2024 Michael Beutler

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

## Enthaltene Komponenten

Das fertige Windows-Paket enthält Komponenten dieser Projekte. Ihre jeweiligen
Lizenzdateien bleiben Bestandteil des Downloads.

| Projekt | Aufgabe | Projektseite |
| --- | --- | --- |
| Playwright | Lokaler Browser und Screenshots | https://github.com/microsoft/playwright-python |
| Pillow | Bildprüfung und Vorschau | https://github.com/python-pillow/Pillow |
| pypdf | PDF-Prüfung und Zusammenführen | https://github.com/py-pdf/pypdf |
| pylatexenc (MIT) | LaTeX als durchsuchbaren Unicode-Text aufbereiten | https://github.com/phfaist/pylatexenc |
| CustomTkinter | Abgerundete Desktop-Oberfläche | https://github.com/TomSchimansky/CustomTkinter |
| Tesseract | Lokale Texterkennung | https://github.com/tesseract-ocr/tesseract |

## Fertiges Windows-Startpaket

Das separat veröffentlichte Windows-ZIP enthält die Python-Laufzeit, Tkinter,
die oben genannten Python-Pakete und Tesseract 5.5.3 mit den Sprachmodellen
Deutsch und Englisch aus `tessdata_fast` sowie die von Playwright bereitgestellte
Firefox-Version. Edge und Chrome werden als vorhandene Systeminstallationen
verwendet und nicht mitgeliefert. Firefox behält seine enthaltenen Lizenzdateien;
Quellcode und Anpassungen: https://github.com/microsoft/playwright/tree/main/browser_patches/firefox.
Mozilla-Lizenzhinweise: https://www.mozilla.org/MPL/2.0/.

Die Lizenzdateien der Python-Pakete und der Laufzeit stehen im Paket unter
`licenses/`; Tesseracts Dokumentation und Apache-2.0-Lizenz unter `ocr/doc/`,
die Lizenz der Sprachmodelle unter `ocr/tessdata/LICENSE`. Originaldateien und
Hinweise aus dem Tesseract-Installer bleiben erhalten. `BUILD.json` nennt die
verwendeten Versionen, die Quellcode-Kennung und die Herkunft des OCR-Installers.

- Python 3.13 / PSF-Lizenz: https://docs.python.org/3.13/license.html
  Die genaue Laufzeitversion des jeweiligen Pakets steht in `BUILD.json`.
- PyInstaller (GPL mit Ausnahme für erzeugte Programme): https://pyinstaller.org/en/stable/license.html
- Unveränderter OCR-Installer als Quelle der Laufzeit: https://github.com/tesseract-ocr/tesseract/releases/tag/5.5.3
- Sprachmodelle (Apache-2.0), festgelegter Stand: https://github.com/tesseract-ocr/tessdata_fast/tree/87416418657359cb625c412a48b6e1d6d41c29bd

Die MIT-Lizenz dieses Projekts gilt für den eigenen Programmcode; Komponenten
anderer Projekte behalten ihre jeweiligen Lizenzen.

## Optionales Mathe-OCR-Zusatzpaket

Die lokale Formelerkennung verwendet die MIT-lizenzierten Pix2Text-Modelle
MFD 1.5 (Formelbereiche) und MFR 1.5 (LaTeX-Erkennung) von BreezeDeus.
Die Modelle werden direkt mit ONNX Runtime, Optimum und Transformers ausgeführt.
Das vollständige Pix2Text-Python-Paket mit seinen Layout-/Tabellenkomponenten
ist nicht enthalten. Es werden keine Buchseiten an einen Onlinedienst gesendet.

- Projekt und Lizenz: https://github.com/breezedeus/Pix2Text
- MFD: https://huggingface.co/breezedeus/pix2text-mfd-1.5/tree/f470a885e0fca1d3d2bfa2a54991db7ae01f1861
- MFR: https://huggingface.co/breezedeus/pix2text-mfr-1.5/tree/1cef9f0bdcd6a4c63df7de1311fb0894593340cc

Das separate Zusatzpaket enthält Python 3.11.9, die CPU-Laufzeit und Modellgewichte.
Versions-, Herkunfts- und Prüfsummenangaben stehen dort in `RUNTIME.json`,
Lizenztexte in der Python-Lizenz, den Paket-Metadaten und `THIRD_PARTY_NOTICES.md`.
Die verwendeten Pakete und Versionen sind in den mitgelieferten Paket-Metadaten
dokumentiert.

Die Pix2Text-Projektlizenz lautet:

```text
MIT License

Copyright (c) 2022 BreezeDeus

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```


## Optionales NVIDIA-RTX-CUDA-Paket

`Edubase-CUDA-OCR-Windows.zip` enthält ONNX Runtime GPU 1.20.2 (MIT)
sowie NVIDIA CUDA Runtime 12.4.127, cuBLAS 12.4.5.8, cuFFT 11.2.1.3
cuDNN 9.1.0.70 sowie NVRTC und nvJitLink 12.4.127 aus den jeweiligen offiziellen NVIDIA-PyPI-Paketen.
Die NVIDIA-Komponenten behalten ihre eigenen Lizenzbedingungen; deren
Original-Lizenzen und Paket-Metadaten bleiben vollständig im Zusatzpaket.
Die MIT-Lizenz der App gilt nicht für die NVIDIA-Komponenten.

- ONNX Runtime: https://github.com/microsoft/onnxruntime
- CUDA: https://docs.nvidia.com/cuda/eula/
- cuDNN: https://docs.nvidia.com/deeplearning/cudnn/backend/latest/reference/eula.html

Das Zusatzpaket wird nur auf ausdrückliche Auswahl eingerichtet und verändert
weder den Grafiktreiber noch die vorhandene CPU-/DirectML-Laufzeit.
