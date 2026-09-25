GNU Radio Schritt für Schritt — Band 1
Grundlagen, GNU Radio Companion und Signalverarbeitung
Kapitel 1 bis 26

Belk Siri — Materialien v1.0.0 (2026-09-20)

Hinweis: Das Archiv ist allen Ausgaben gemeinsam und enthält deshalb eine
französische README.txt. Dies ist derselbe Text auf Deutsch. Er wird auf der
Materialienseite bereitgestellt, nicht im Archiv, damit dessen Prüfsumme —
die in der französischen Ausgabe gedruckt steht — unverändert bleibt.

===========================================================================
WAS DIESES ARCHIV ENTHÄLT
===========================================================================

34 Dateien, 718 067 Byte.

  flowgraphs/CHnn/   die Beispiel-Flowgraphs der Kapitel
  flowgraphs/TP-nn/  die Flowgraphs der Übungen

Die Audiodatei book-audio.wav liegt IN dem Ordner jeder Übung, die sie
liest. Die Flowgraphs bezeichnen sie nur mit ihrem Namen, also im aktuellen
Ordner: Sie muss neben der .grc-Datei bleiben. Kopieren Sie den ganzen
Ordner, nicht nur die .grc-Datei.

Zwei Dateien liegen NICHT bei, weil Sie sie selbst erzeugen:
echantillons.iq, geschrieben vom Flowgraph der Übung 8, und die .cfile mit
echten Abtastwerten, die in Übung 18 aufgezeichnet wird.

Der Aufbau ist der, den das Buch im Abschnitt „Die Materialien zu diesem
Buch“ ankündigt: ein Ordner je Kapitel oder je Übung, benannt nach seiner
Kennung. Der Dateiname übernimmt die Kennung des Flowgraphs in
Kleinbuchstaben; sie steht außerdem im Block Options, sodass sich die Datei
auch nach einer Umbenennung wiederfinden lässt.

Die Ordnernamen TP-01 bis TP-18 sind die unveränderlichen Kennungen der
Übungen. Im deutschen Text heißen sie Übung 1 bis Übung 18; die Ordner
behalten ihre Namen, damit ein einziges Archiv allen Sprachen dient.

===========================================================================
REFERENZVERSIONEN
===========================================================================

  GNU Radio    3.10.12.0
  Radioconda   2025.03.14 (osx-arm64)
  System       macOS 26.6.2, Apple Silicon

Die Flowgraphs wurden mit GNU Radio 3.10.12.0 gespeichert. Öffnen Sie sie
mit derselben Version oder einer neueren der Reihe 3.10. Eine ältere
Version kann sie nicht lesen: Das Dateiformat hat sich zwischen 3.7 und 3.8
geändert.

===========================================================================
LOSLEGEN
===========================================================================

1. Entpacken Sie dieses Archiv in Ihren Arbeitsordner.
2. Kopieren Sie den Ordner des Kapitels, das Sie interessiert, in Ihren
   eigenen Ordner flowgraphs/ und arbeiten Sie dann an der Kopie. Die
   Übungen lassen Sie Werte ändern; das Original erlaubt es, ohne erneutes
   Herunterladen zum Ausgangszustand zurückzukehren.
3. Öffnen Sie die .grc-Datei in GNU Radio Companion (Menü File, dann Open).
4. Erzeugen Sie mit F5, führen Sie mit F6 aus, halten Sie mit F7 an.

Das Python-Programm, das GRC neben die .grc-Datei schreibt, wird bei jeder
Erzeugung neu gebaut. Es liegt hier nicht bei, und es gibt nie einen Grund,
es zu ändern oder zu speichern.

===========================================================================
HARDWARE
===========================================================================

Kein Flowgraph dieses Archivs verlangt einen Funkempfänger.
Alles läuft in der Simulation. Für die Flowgraphs, die Ton erzeugen,
genügt eine Soundkarte.

===========================================================================
RECHTE
===========================================================================

(c) 2026 Belk Siri. Alle Rechte vorbehalten.

Diese Dateien werden als Begleitung zum Buch „GNU Radio Schritt für
Schritt“ bereitgestellt. Das Herunterladen und der persönliche Gebrauch
sind gestattet. Ein Recht zur Weiterverwendung, zur öffentlichen Änderung
oder zur Weitergabe wird zum jetzigen Zeitpunkt nicht eingeräumt.

Die Datei audio/book-audio.wav ist eine eigens für das Buch erzeugte
Synthese: sechs Töne mit den genauen Frequenzen 220, 330, 440, 550, 440 und
220 Hz, 44 100 Abtastwerte pro Sekunde, ein Kanal, 16 Bit, 6 Sekunden. Sie
enthält keine fremde Aufnahme und keine Stimme.

Die .grc-Flowgraphs sind Textdateien, die für dieses Buch erstellt wurden.
Sie enthalten weder Logo noch Code noch sonstiges Material des
GNU-Radio-Projekts.

===========================================================================
KEINE VERBINDUNG
===========================================================================

GNU Radio wird in diesem Buch als die behandelte Software genannt. Diese
unabhängige Veröffentlichung wird vom GNU-Radio-Projekt und von der Free
Software Foundation weder herausgegeben noch unterstützt noch gebilligt.

===========================================================================
DIESES ARCHIV PRÜFEN
===========================================================================

Die Datei MANIFEST.json nennt Pfad, Größe und SHA-256-Prüfsumme jeder
Datei. So prüfen Sie eine Datei:

  macOS   shasum -a 256 flowgraphs/TP-03/fg_tp03_001.grc
  Windows certutil -hashfile flowgraphs\TP-03\fg_tp03_001.grc SHA256
  Linux   sha256sum flowgraphs/TP-03/fg_tp03_001.grc

Die Prüfsumme des Archivs selbst steht auf der Seite des Bandes:
https://belksiri.github.io/books/gnu-radio-pas-a-pas/de/volume-1/

===========================================================================
SEITE ZUM BUCH
===========================================================================

https://belksiri.github.io/books/gnu-radio-pas-a-pas/

Korrekturen, Aktualisierungen und das Melden von Problemen finden Sie dort.
Die deutsche Korrekturseite:
https://belksiri.github.io/books/gnu-radio-pas-a-pas/de/korrekturen/
