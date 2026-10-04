# Anleitung

[← Downloads und Schnellstart / English quick start](../README.md)

## Starten und drei Seiten testen

1. [Windows-App herunterladen](https://github.com/Sebii1998/edubase-to-pdf-ocr/releases/download/v1.6.0/Edubase-PDF-Windows.zip),
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
- Weitere Optionen findest du unter **Erweiterte Einstellungen**;
  Fehlermeldungen unter **Protokoll**.

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

Zum Fortsetzen den Browser öffnen, erneut anmelden und dasselbe Buch öffnen.
Die Automatik dabei ausgeschaltet lassen. **Aufnahme fortsetzen…** wählen,
den Auftrag laden und **Auftrag fortsetzen + OCR** anklicken. Die App prüft
bereits gespeicherte Seiten und fährt mit der fehlenden Seite fort.

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
unter **Erweiterte Einstellungen → Arbeitsbilder behalten** den Haken setzen.

## Buchseiten und Reader-Seiten

Der **Seitenbereich** verwendet immer die Seitenzahlen des Edubase-Readers.
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
3. Die fertige PDF in einem PDF-Programm mit **Anhangsbereich** öffnen.

Die lokale Erkennung nutzt [Pix2Text-Modelle](https://github.com/breezedeus/Pix2Text)
für Brüche, Wurzeln, Potenzen, Indizes und Formelzeichen. Erkannte Formeln werden
als LaTeX mit Seitenzuordnung in zwei **PDF-Anhängen** (`.formeln.md` und
`.formeln.json`) gespeichert. Die sichtbaren PDF-Seiten bleiben unverändert;
die Anhänge ermöglichen das Weiterverwenden der erkannten Schreibweise.
Nicht jeder PDF-Betrachter zeigt Anhänge an.

Das Modul löst keine Aufgaben. Vorzeichen, Indizes und ähnliche Buchstaben
prüfen. Die zusätzliche Erkennung benötigt Zeit und Arbeitsspeicher;
die normale PDF-Erstellung funktioniert ohne sie.

[Zusatzmodul separat herunterladen](https://github.com/Sebii1998/edubase-to-pdf-ocr/releases/download/v1.6.0/Edubase-Mathe-OCR-Windows.zip)
– am einfachsten erfolgt die Einrichtung direkt über den Knopf in der App.

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

Neue Aufnahmen verwenden einen Browser-Auflösungsfaktor von **4**. Die PDF wird
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
| Browser nicht gefunden | Enthaltenes Firefox oder installiertes Edge/Chrome wählen. |
| Buch wird nicht erkannt | Buch im von der App geöffneten Browser öffnen, Anmeldung abschliessen und Einzelseitenansicht wählen. |
| Seite noch nicht vollständig geladen | Wartezeit pro Seite erhöhen und zuerst wenige Seiten testen. |
| Identische Seiten gemeldet | Prüfen, ob umgeblättert wird. Identische Nachbarseiten nur erlauben, wenn diese im Buch wirklich vorkommen. |
| Sitzung abgelaufen | Browser erneut öffnen, anmelden, dasselbe Buch öffnen und Auftrag fortsetzen. |
| Formeln fehlen | PDF-Anhänge und Protokoll prüfen. Bei einem Erkennungsfehler **Nur OCR erneut…** mit aktivierter Mathe-Option verwenden. |
| Arbeitsbilder nach dem Export fehlen | Gewollte Voreinstellung. Für weitere Seiten **Neuer Auftrag**; vor künftigen Exporten bei Bedarf **Arbeitsbilder behalten** wählen. |

[Fehler melden](https://github.com/Sebii1998/edubase-to-pdf-ocr/issues):
App-Version, Windows-Version, fehlerhaften Schritt und genaue Meldung nennen.
Keine Anmeldedaten, Bücher oder privaten PDFs hochladen.

Die Verarbeitung läuft lokal; Buchseiten und PDFs werden nicht auf GitHub oder
einen OCR-Dienst hochgeladen. Unabhängiges Projekt: Verwende nur Inhalte,
auf die du zugreifen und die du speichern darfst.

[Lizenz](../LICENSE) · [Drittanbieterhinweise](../THIRD_PARTY_NOTICES.md)
