# Anleitung · Version 1.8.0 – Finale Version

[← Downloads und Schnellstart / English quick start](../README.md)

## PDFs zusammenfügen

1. **PDFs zusammenfügen…** anklicken und mindestens zwei PDFs vom PC auswählen.
2. Im neuen Fenster die Reihenfolge prüfen. Mit den Pfeilen nach oben/unten
   verschieben, weitere PDFs hinzufügen oder Einträge entfernen.
3. **Zusammenfügen & speichern…** wählen und einen neuen Dateinamen für die Ausgabe festlegen.

Die PDFs werden in der angezeigten Reihenfolge verbunden. Vorhandene Seiten,
Text- und Formel-Suchschichten werden übernommen; es startet keine neue OCR
und kein Browser. Die Quelldateien bleiben unverändert. Eine bereits vorhandene
Ausgabedatei wird nicht überschrieben. Passwortgeschützte PDFs müssen zuerst
als ungeschützte Kopie vorliegen.

Während des Zusammenfügens sind **Pause** und **Stoppen** verfügbar. Ein Abbruch
veröffentlicht keine unvollständige Ergebnis-PDF; zum erneuten Versuch die
Dateien wieder auswählen. Ein zuvor geladener OCR-Auftrag bleibt erhalten.

## Eigene PDF vom PC verarbeiten

1. **Eigene PDF auswählen…** anklicken und die Datei vom PC wählen. Die App
   erkennt die PDF, zeigt ihren Namen und die Seitenzahl und wählt zunächst
   **alle Seiten** aus. Bei Bedarf den Seitenbereich einschränken; **Ganze PDF**
   stellt wieder den vollständigen Bereich ein.
2. **Textsprache** einstellen. Text-OCR wird ausgeführt. Nur wenn zusätzlich
   **Mathe & Formeln erkennen** angehakt ist, werden auch Formeln erkannt.
   Dafür wie bisher einmal das Mathe-Modul einrichten. Die optionalen
   GPU-/CUDA-Einstellungen und Formelanhänge können weiter verwendet werden.
3. Ausgabetitel und Zielordner prüfen und **PDF mit OCR verarbeiten** anklicken.
   Nach Abschluss die Lesbarkeit und die Textsuche in der neuen PDF prüfen.

Die Auswahl schaltet automatisch auf den PDF-Modus um. Dafür wird kein Browser
geöffnet, keine Edubase-Anmeldung verlangt und keine Bildschirmaufnahme gemacht.
Browser- und Aufnahmeeinstellungen sind in diesem Modus deaktiviert. Die Datei
wird lokal verarbeitet. Die Original-PDF bleibt unverändert; die Ausgabe bekommt
einen freien Dateinamen und überschreibt auch keine ältere OCR-PDF.

Die ursprünglichen PDF-Seiten werden für die Ausgabe übernommen; Text und
Vektorgrafiken werden nicht durch die OCR-Arbeitsbilder ersetzt. Die OCR ergänzt
unsichtbaren Suchtext. Hat eine PDF bereits eine Textschicht, bleibt diese
erhalten: Beim Kopieren oder Extrahieren können dadurch doppelte Textstellen
auftreten. Auch in diesem Fall führt die App die gewählte OCR aus. Vorhandene
PDF-Seitenbeschriftungen bleiben erhalten; **Buchzählung** ist im PDF-Modus deaktiviert.

**Pause** und **Stoppen** gelten auch für den PDF-Auftrag. Bei Stopp oder Fehler
bleiben die internen Arbeitsdaten erhalten. **Aufnahme fortsetzen…** erkennt
auch einen gespeicherten PDF-Auftrag und setzt ihn ohne Browser fort. Dafür
verwendet die App ihre unveränderte Arbeitskopie der ursprünglichen PDF.
**Bisherige Seiten als PDF** exportiert vollständig vorbereitete Seiten ab
Beginn des gewählten Bereichs. Für eine weitere Verarbeitung nach einem
solchen Export zuvor **Arbeitsbilder behalten** einschalten.

Wie bei Edubase werden die internen Arbeitsdaten nach erfolgreichem Export
standardmässig gelöscht. Soll später **Nur OCR erneut…** verwendet werden,
vorher unter **Erweiterte Einstellungen / Performance-Einstellungen** **Arbeitsbilder behalten** aktivieren.
Die ausgewählte Originaldatei wird bei dieser Bereinigung nie gelöscht.
Mit **Neuer Auftrag** wird der PDF-Modus verlassen; danach ist die bisherige
Edubase-Aufnahme wieder verfügbar.

## Fortschritt bei Aufnahme und OCR

Unten stehen zwei Fortschrittsbalken: **Aufnahme** zählt gespeicherte Buchseiten,
**OCR** zählt fertig erkannte Seiten. Bei eingeschalteter Mathe-OCR zeigt die
Beschriftung **Text** und **Mathe** einzeln. Die Verarbeitung kann schon während
der Aufnahme laufen. Wenn alle OCR-Seiten fertig sind, kann das Speichern und
Prüfen der endgültigen PDF noch dauern; der Status darüber zeigt diesen Schritt.

Die Edubase-Aufnahme und die bisherigen Verbesserungen aus Version 1.7.0 bleiben erhalten. Die App spart wiederholte Bildzugriffe und unnötige Zwischenexporte. Die
PNG-Komprimierung, Aufnahmeauflösung, Farben und Erkennungsmodelle bleiben
unverändert. Bestehende Mathe-, GPU- und CUDA-Zusatzmodule werden weiterhin erkannt.

## Adaptive Wartezeit bei der Aufnahme

Die **Wartezeit pro Seite** beträgt standardmässig **2 Sekunden**. Sie ist die
maximale zusätzliche Beruhigungszeit nach den Ladeprüfungen. Bei vollständig
geladenen, stabilen Bild- oder SVG-Seiten kann die Aufnahme früher weitergehen.
Bei Canvas-Seiten oder unbekannter Darstellung bleibt die volle eingestellte
Wartezeit erhalten. Das gilt für Edge, Chrome und das mitgelieferte Firefox.

Die App prüft weiterhin geladene Bilder und Schriften, die richtige Seite und
eine stabile Darstellung. Diese notwendigen Prüfungen können länger dauern:
**2 Sekunden sind keine Obergrenze für die gesamte Aufnahme einer Seite.**
Die Bildqualität wird für die Beschleunigung nicht reduziert.

## OCR-Leistung

**Erweiterte Einstellungen / Performance-Einstellungen → OCR-Leistung**:

- **Automatisch:** Textseiten werden mit Reserve für Browser und Mathe-OCR parallel verarbeitet.
  Bei ausreichenden Ressourcen beginnt die OCR schon während der Aufnahme.
  Mathe-OCR nutzt das eingerichtete GPU-Modul, wenn es funktioniert.
- **CPU – maximale Leistung:** mehrere Textseiten gleichzeitig; die App begrenzt
  die Anzahl anhand der CPU-Threads, des freien RAMs und der Bildgrösse.
  Mathe-OCR darf in diesem Modus alle Rechenthreads nutzen.
- **GPU verwenden:** nur für Mathe-OCR, mit eingerichtetem GPU-Modul und geeigneter
  Grafik. Text-OCR läuft parallel auf der CPU, mit Ressourcenreserve. Bei GPU-Problemen übernimmt
  die CPU.

Die App zeigt erkannte Grafikkarten in den erweiterten Einstellungen an. Eine
manuelle Eingabe des Modells ist nicht nötig. Bei mehreren Karten bevorzugt sie
die von Windows für hohe Leistung vorgesehene GPU. Das Protokoll nennt die
tatsächlich für Mathe-OCR verwendete Karte oder meldet den CPU-Betrieb.

Während der Aufnahme verarbeitet die Text-OCR üblicherweise bis zu **zwei Seiten
gleichzeitig**. Bei wachsendem Rückstand und genügend CPU- und RAM-Reserve erhöht
die App auf bis zu **vier**. Auch wartende Seiten werden schon während der
Aufnahme abgearbeitet. Bei knappen Ressourcen verarbeitet der Export die noch
fehlenden OCR-Seiten. Hält die Text-OCR bereits mit der Aufnahme mit, bringt
zusätzliche Parallelität allein keinen Tempogewinn.

Für die GPU stehen **Standard (10 Formeln)**, **Hoch (20 Formeln)** und
**Maximum (30 Formeln)** zur Wahl. Die Zahl begrenzt die gemeinsam verarbeiteten
Formeln. Die App füllt Gruppen aus bis zu vier bereits gespeicherten Seiten und
verarbeitet ähnlich lange Ausschnitte gemeinsam. Sie wartet dafür nicht auf
noch aufzunehmende Seiten. Die ursprüngliche Formelreihenfolge bleibt erhalten.
Grössere Gruppen benötigen mehr Grafikspeicher und garantieren keine höhere
Geschwindigkeit. Bei Problemen verkleinert die App die Gruppe automatisch.
Auflösung, Farben und Erkennungsmodelle bleiben unverändert. Die Einstellung
wirkt auf GPU-Mathe-OCR, nicht auf die normale Text-OCR oder die Seitenaufnahme.

Die PDF bleibt in der richtigen Seitenreihenfolge, mit gleicher Bildauflösung und
Buchzählung. Pause lässt bereits laufende Seiten fertig werden und startet keine
weiteren; Stoppen beendet die laufende Erkennung. Fertige OCR-Seiten bleiben bei
Abbruch im Zwischenspeicher. Mehr CPU-Leistung kann den Laptop wärmer und lauter
machen und ist nicht auf jedem Gerät schneller.


## NVIDIA RTX und AMD

**CUDA verwenden (NVIDIA RTX)** ist unter **Erweiterte Einstellungen / Performance-Einstellungen** nur bei
einer erkannten NVIDIA-RTX-Karte auswählbar und standardmässig ausgeschaltet.
Zuerst **CUDA-Modul einrichten** wählen. Die App lädt ein separates Zusatzpaket;
eine manuelle Eingabe des Grafikkartenmodells oder eine CUDA-Toolkit-Installation
ist nicht erforderlich. Ein funktionierender NVIDIA-Treiber wird benötigt.

CUDA hält Formelmerkmale zwischen Erkennungsschritten im Grafikspeicher.
Modellgewichte, Auflösung und volle FP32-Genauigkeit bleiben erhalten. Hat CUDA
bereits Formelseiten erfolgreich erkannt und tritt später ein Erkennungsfehler
auf, versucht die App pro Lauf höchstens einen Neustart der CUDA-Erkennung. Bereits
fertige Ergebnisse bleiben erhalten und werden nicht erneut erkannt. Bei
Startproblemen oder erneutem Erkennungsfehler werden verfügbare Alternativen
bis hin zu DirectML und CPU versucht. Stoppen und Zeitlimits lösen keinen
Neustart aus; es gibt keine endlose Wiederholung. Das Protokoll nennt Fehler, Wechsel und die
tatsächlich aktive Technik und Grafikkarte. Eine erkannte RTX-Karte allein
garantiert nicht, dass Treiber und Zusatzmodul CUDA erfolgreich starten.

**AMD und Intel:** Das vorhandene **GPU-Modul einrichten** installiert DirectML.
Die neuen seitenübergreifenden und nach geschätzter Länge sortierten Formelgruppen
funktionieren auch damit. CUDA ist ausschliesslich für NVIDIA vorgesehen.

## Starten und drei Seiten testen

1. [Windows-App herunterladen](https://github.com/Sebii1998/edubase-to-pdf-ocr/releases/download/v1.8.0/Edubase-PDF-Windows.zip),
   ZIP vollständig entpacken und **`Edubase-PDF.exe`** starten. Die Ordner neben
   der EXE gehören zum Programm und müssen mitentpackt werden.
2. **Browser öffnen**, bei Edubase anmelden und das Buch in der
   **Einzelseitenansicht** öffnen. Der Buchtitel wird automatisch übernommen;
   **Buch erkennen** aktualisiert die Angaben bei Bedarf manuell.
3. **Reader-Seiten 1–3** einstellen, **Vorschau** prüfen und
   **Aufnehmen + OCR-PDF** starten. Währenddessen nicht selbst blättern.
4. In der fertigen PDF Reihenfolge, Lesbarkeit und Textsuche prüfen.
   Anschliessend über **Neuer Auftrag** einen grösseren Bereich aufnehmen.

Standardziel ist **`Dokumente/Edubase-PDF`**. Jeder Auftrag erhält einen eigenen
Unterordner. Mit **Ausgabe öffnen** gelangst du direkt dorthin.

## Sprache, Browser und Hilfe

- **Deutsch / English** oben rechts schaltet die Oberfläche und Hilfetexte um.
  Jeder Programmstart beginnt auf Deutsch. **Textsprache** legt unabhängig davon
  die OCR-Sprache des Buchs fest; `deu+eng` erkennt deutschen und englischen Text.
- **Edge** und **Chrome** müssen auf dem PC installiert sein. Die benötigte
  **Firefox**-Version ist im ZIP enthalten. Jede Auswahl öffnet eine eigene
  temporäre Sitzung, in der du dich anmeldest.
- Die kleinen **ⓘ** erklären Einstellungen und Aktionen: darüberfahren oder
  anklicken. Mit **Tab** und **Enter** geht es auch per Tastatur.
- Weitere Optionen findest du unter **Erweiterte Einstellungen / Performance-Einstellungen**;
  Fehlermeldungen unter **Protokoll**.
- **Protokoll kopieren** kopiert alle bisher gesammelten Meldungen mit Uhrzeit
  in die Zwischenablage – auch bei eingeklapptem Protokoll und während einer
  Verarbeitung. Die Meldungen folgen der aktuell gewählten Oberflächensprache.
  Mit **Strg+V** in einen Texteditor oder eine Support-Nachricht einfügen.

## Ganzes Buch automatisch aufnehmen

Vor **Browser öffnen** den Haken **Ganzes Buch automatisch aufnehmen** setzen,
anmelden und das gewünschte Buch öffnen. Sobald eine einzelne Buchseite und die
Seitenzahl erkannt sind, beginnt die Aufnahme von der ersten bis zur letzten
Reader-Seite mit anschliessender PDF-Erstellung. Die Automatik ist beim Start
ausgeschaltet und verarbeitet pro Start genau ein Buch.

Bei Doppelseiten oder fehlender Seitenzahl wartet die App. Zur
Einzelseitenansicht wechseln oder **Stoppen** wählen und manuell starten.

## Pause, Stopp und später fortsetzen

**Pause / Fortsetzen** unterbricht die laufende Arbeit vor der nächsten Seite.
**Stoppen** beendet den Auftrag; vollständig gespeicherte Seiten bleiben erhalten.

Zum Fortsetzen einer Edubase-Aufnahme den Browser öffnen, erneut anmelden und dasselbe Buch öffnen.
Die Automatik dabei ausgeschaltet lassen. **Aufnahme fortsetzen…** wählen,
den Auftrag laden und **Auftrag fortsetzen + OCR** anklicken. Die App prüft
bereits gespeicherte Seiten und fährt mit der fehlenden Seite fort.

Ein gespeicherter Auftrag einer eigenen PDF wird automatisch erkannt und ohne
Browser fortgesetzt. Nach dem Laden **PDF mit OCR verarbeiten** wählen.

Sind alle Bilder vorhanden und nur die Texterkennung fehlgeschlagen,
**Nur OCR erneut…** verwenden. Dafür ist kein Browser nötig.

## Nach einem Stopp die bisherigen Seiten als PDF

Nach **Stoppen** warten, bis der laufende Schritt beendet ist. Dann
**Bisherige Seiten als PDF** anklicken. Exportiert werden alle vollständig
gespeicherten Seiten ab dem Anfang des gewählten Bereichs. Wurde Seite 62 noch
nicht vollständig gespeichert, endet die Teil-PDF bei Seite 61. Der Dateiname
kennzeichnet den aufgenommenen Reader-Seitenbereich.

**Nach erfolgreichem Export werden die Arbeitsbilder automatisch gelöscht –
auch bei einer Teil-PDF.** Für weitere Seiten anschliessend **Neuer Auftrag**
verwenden. Soll derselbe Auftrag später fortsetzbar bleiben, **vor dem Export**
unter **Erweiterte Einstellungen / Performance-Einstellungen → Arbeitsbilder behalten** den Haken setzen.

## Buchseiten und Reader-Seiten

Bei einer Edubase-Aufnahme verwendet der **Seitenbereich** die Seitenzahlen des
Edubase-Readers. Bei einer eigenen PDF verwendet er die tatsächlichen
PDF-Seitenpositionen ab 1; vorhandene PDF-Seitenbeschriftungen bleiben erhalten.
Bei **Buchzählung** trägst du ein, auf welcher Reader-Seite die gedruckte
Buchseite **1** steht. Beispiel: Buchseite 1 ist Reader-Seite 37 → **37** eintragen.

Ein Export der Reader-Seiten 37–80 umfasst **44 PDF-Seiten**. Bei durchgehend
fortlaufender Buchzählung erhalten sie die PDF-Beschriftungen 1–44.
Vorspannseiten erhalten eigene Beschriftungen. Das ändert weder die Seitenbilder
noch die tatsächliche Seitenanzahl. Manche PDF-Programme zeigen diese
Beschriftungen nicht an. Werbung, unnummerierte Einschübe oder andere
Sonderzählungen werden durch diesen einfachen Versatz nicht automatisch erkannt.

## Optional: Mathe und Formeln

1. **Mathe-OCR einrichten** lädt einmalig das Zusatzmodul samt Modellen herunter
   (ca. **575 MB**, zusätzlicher Platz zum Entpacken nötig).
2. **Mathe & Formeln erkennen** aktivieren und zunächst wenige typische Seiten testen.
3. **LaTeX-Dateien zusätzlich als PDF-Anhang** nur bei Bedarf aktivieren (standardmässig aus).

Die lokale Erkennung nutzt [Pix2Text-Modelle](https://github.com/breezedeus/Pix2Text)
für Brüche, Wurzeln, Potenzen, Indizes und Formelzeichen. Sie ergänzt unsichtbaren
**Suchtext**, während die sichtbaren PDF-Seiten unverändert bleiben. Mit **Strg+F**
z. B. nach `σ` oder `F/A` suchen. Komplexe Ausdrücke werden linear dargestellt,
etwa `(a+b)/(c-d)` oder `x^2`. Treffer hängen von Erkennung und PDF-Programm ab;
mathematisch gleichwertige Schreibweisen werden nicht automatisch gefunden.

Die separate Anhangsoption speichert LaTeX und Seitenzuordnung in
`.formeln.md` und `.formeln.json` innerhalb der PDF zum Weiterverwenden.
**Für Strg+F ist kein Anhang nötig.** Zum Öffnen der optionalen Dateien
ein PDF-Programm mit Anhangsbereich verwenden.

Das Modul löst keine Aufgaben. Vorzeichen, Indizes und ähnliche Buchstaben
prüfen. Die zusätzliche Erkennung benötigt Zeit und Arbeitsspeicher;
die normale PDF-Erstellung funktioniert ohne sie.

[Zusatzmodul separat herunterladen](https://github.com/Sebii1998/edubase-to-pdf-ocr/releases/download/v1.7.0/Edubase-Mathe-OCR-Windows.zip)
– am einfachsten erfolgt die Einrichtung direkt über den Knopf in der App.
Die Mathe-, GPU- und CUDA-Pakete bleiben unverändert auf Version 1.7.0;
bereits eingerichtete Module können weiterverwendet werden.

## Ausgabe, Bildqualität und grosse Bücher

Im Ausgabeordner bleibt nach erfolgreichem Export standardmässig **nur die PDF**.
Während der Verarbeitung liegen Bilder und Zwischendateien im lokalen
Arbeitsbereich der App. Bei Stopp oder Fehler bleiben sie für einen erneuten
Versuch erhalten. Scheitert nur die Mathe-Erkennung, bleibt die normale PDF
ebenfalls erhalten; mit **Nur OCR erneut…** lässt sich die Erkennung wiederholen.

**Arbeitsbilder behalten** verhindert die automatische Bereinigung und ermöglicht
Fortsetzen oder erneutes OCR auch nach einem erfolgreichen Export. Späteres
Aktivieren stellt bereits gelöschte Bilder nicht wieder her. Vorhandene fertige
PDFs werden nicht überschrieben; ein neuer Export erhält einen freien Dateinamen.

Neue Edubase-Aufnahmen verwenden einen Browser-Auflösungsfaktor von **4**. Die PDF wird
mit **300 DPI** erstellt. Ein höherer DPI-Wert allein erzeugt keine zusätzlichen
Bilddetails. Bei kleiner Anzeige im PDF-Betrachter **Seitenbreite** oder eine
höhere Zoomstufe wählen. Die Qualität hängt auch vom Ausgangsmaterial ab.

Für sehr grosse Bücher den Export bei Bedarf aufteilen, etwa Seiten 1–250 und
251–500. Das **Seiten-Zeitlimit** gilt pro Ladeversuch, das **OCR-Zeitlimit** pro
OCR-Seite, jeweils nicht für das gesamte Buch.

## Wenn etwas nicht funktioniert

| Problem | Lösung |
| --- | --- |
| EXE, OCR oder Sprachdaten fehlen | Das vollständige Windows-ZIP erneut entpacken; alle mitgelieferten Ordner neben der EXE belassen. |
| PDFs lassen sich nicht zusammenfügen | Mindestens zwei gültige, nicht verschlüsselte PDFs auswählen, Reihenfolge prüfen und einen neuen Dateinamen wählen. Bestehende Dateien werden nicht überschrieben. |
| Eigene PDF lässt sich nicht öffnen | Eine gültige, nicht verschlüsselte PDF auswählen. Fehlermeldung und Protokoll prüfen; die Originaldatei bleibt unverändert. |
| Browser nicht gefunden | Enthaltenes Firefox oder installiertes Edge/Chrome wählen. |
| Buch wird nicht erkannt | Buch im von der App geöffneten Browser öffnen, Anmeldung abschliessen und Einzelseitenansicht wählen. |
| Seite noch nicht vollständig geladen | Einzelseitenansicht, Vorschau und Protokoll prüfen. Bei einem Lade-Zeitlimit das Seiten-Zeitlimit erhöhen und zuerst wenige Seiten testen. Eine höhere maximale Wartezeit deaktiviert die adaptive frühere Aufnahme nicht. |
| Identische Seiten gemeldet | Prüfen, ob umgeblättert wird. Identische Nachbarseiten nur erlauben, wenn diese im Buch wirklich vorkommen. |
| Sitzung abgelaufen | Browser erneut öffnen, anmelden, dasselbe Buch öffnen und Auftrag fortsetzen. |
| Formeln fehlen | Mit Strg+F nach einem erkannten Zeichen suchen; Anhänge gibt es nur bei gewählter Anhangsoption. Bei einem Erkennungsfehler das Protokoll prüfen und **Nur OCR erneut…** mit aktivierter Mathe-Option verwenden. |
| Arbeitsbilder nach dem Export fehlen | Gewollte Voreinstellung. Für weitere Seiten **Neuer Auftrag**; vor künftigen Exporten bei Bedarf **Arbeitsbilder behalten** wählen. |

[Fehler melden](https://github.com/Sebii1998/edubase-to-pdf-ocr/issues):
App-Version, Windows-Version, fehlerhaften Schritt und genaue Meldung nennen.
Keine Anmeldedaten, Bücher oder privaten PDFs hochladen.

Die Verarbeitung läuft lokal; Buchseiten und PDFs werden nicht auf GitHub oder
einen OCR-Dienst hochgeladen. Unabhängiges Projekt: Verwende nur Inhalte,
auf die du zugreifen und die du speichern darfst.

[Lizenz](../LICENSE) · [Drittanbieterhinweise](../THIRD_PARTY_NOTICES.md)
