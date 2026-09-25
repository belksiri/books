GNU Radio Schritt für Schritt — Band 2
Modulation, digitale Kommunikation und RTL-SDR
Kapitel 1 bis 16

Belk Siri — Materialien v1.0.1 (2026-09-21)

Hinweis: Das Archiv ist allen Ausgaben gemeinsam und enthält deshalb eine
französische README.txt. Dies ist derselbe Text auf Deutsch. Er wird auf der
Materialienseite bereitgestellt, nicht im Archiv, damit dessen Prüfsumme —
die in der französischen Ausgabe gedruckt steht — unverändert bleibt.

Band 2 ist auf Deutsch vollständig übersetzt und gesetzt. Die Materialien
sind allen Sprachen gemeinsam.

===========================================================================
KAPITELNUMMERIERUNG
===========================================================================

Band 2 liest sich für sich allein: Seine Kapitel sind 1 bis 16 gedruckt.

Die Ordner und Dateinamen dieses Archivs tragen die INTERNE TECHNISCHE
KENNUNG des Kapitels (CH27 bis CH42). Diese Kennungen bleiben erhalten,
damit die Dateien kompatibel bleiben: Sie ändern sich nie, weder von einer
Ausgabe zur nächsten noch von einer Sprache zur anderen, und sie stehen
außerdem im Block Options jedes Flowgraphs.

  gedrucktes Kapitel  1  ->  interne Kennung CH27  Grundlagen der Modulation
  gedrucktes Kapitel  2  ->  interne Kennung CH28  Amplitudenmodulation (AM)
  gedrucktes Kapitel  3  ->  interne Kennung CH29  Frequenzmodulation (FM)
  gedrucktes Kapitel  4  ->  interne Kennung CH30  Vom Bit zum Symbol: ASK und FSK
  gedrucktes Kapitel  5  ->  interne Kennung CH31  Phasenmodulation und QAM
  gedrucktes Kapitel  6  ->  interne Kennung CH32  Der unvollkommene Kanal
  gedrucktes Kapitel  7  ->  interne Kennung CH33  Der RTL-SDR
  gedrucktes Kapitel  8  ->  interne Kennung CH34  Den RTL-SDR installieren und erkennen
  gedrucktes Kapitel  9  ->  interne Kennung CH35  Den Empfänger einstellen
  gedrucktes Kapitel 10  ->  interne Kennung CH36  FM-Radio empfangen
  gedrucktes Kapitel 11  ->  interne Kennung CH37  Aufzeichnen, wiedergeben und erkunden
  gedrucktes Kapitel 12  ->  interne Kennung CH38  Bewährte Praxis, Fehlersuche und rechtlicher Rahmen
  gedrucktes Kapitel 13  ->  interne Kennung CH39  Den erzeugten Python-Code lesen und ändern
  gedrucktes Kapitel 14  ->  interne Kennung CH40  Embedded Python Blocks
  gedrucktes Kapitel 15  ->  interne Kennung CH41  OOT-Module und Ökosystem
  gedrucktes Kapitel 16  ->  interne Kennung CH42  Quellen und Lernwege

Die Zuordnung der Nummern hängt an den Kennungen, nicht an der Sprache:
Sie gilt für jede Ausgabe des Buches gleichermaßen.

Die TP-nn-Ordner sind davon nicht betroffen: Die Übungen behalten ihre
Nummer, im Buch wie im Archiv. Übung 11 des Buches ist der Ordner TP-11.

===========================================================================
WAS DIESES ARCHIV ENTHÄLT
===========================================================================

16 Dateien, 631 172 Byte.

  flowgraphs/CHnn/   die Beispiel-Flowgraphs der Kapitel
  flowgraphs/TP-nn/  die Flowgraphs der Übungen

Die Audiodatei book-audio.wav liegt IN dem Ordner der Übung, die sie liest.
Die Flowgraphs bezeichnen sie nur mit ihrem Namen, also im aktuellen
Ordner: Sie muss neben der .grc-Datei bleiben. Kopieren Sie den ganzen
Ordner, nicht nur die .grc-Datei.

===========================================================================
REFERENZVERSIONEN
===========================================================================

  GNU Radio    3.10.12.0
  Radioconda   2025.03.14 (osx-arm64)
  System       macOS 26.6.2, Apple Silicon

Die Flowgraphs wurden mit GNU Radio 3.10.12.0 gespeichert. Eine Version vor
3.8 kann sie nicht lesen: Das Dateiformat hat sich zwischen 3.7 und 3.8
geändert.

===========================================================================
LOSLEGEN
===========================================================================

1. Entpacken Sie dieses Archiv in Ihren Arbeitsordner.
2. Kopieren Sie den Ordner des Kapitels oder der Übung in Ihren eigenen
   Ordner flowgraphs/ und arbeiten Sie dann an der Kopie.
3. Öffnen Sie die .grc-Datei in GNU Radio Companion (Menü File, dann Open).
4. Erzeugen Sie mit F5, führen Sie mit F6 aus, halten Sie mit F7 an.

===========================================================================
HARDWARE
===========================================================================

Anders als in Band 1 verlangen mehrere Flowgraphs dieses Bandes einen
RTL-SDR-Empfänger. Die im Buch veröffentlichten Messungen wurden mit einem
tatsächlich angeschlossenen RTL2832U-Stick und einem R820T-Tuner
durchgeführt, mit angeschlossener Antenne und tatsächlich empfangenen
Aussendungen. Der RTL-SDR Blog V3, das Referenzmodell des Buches, wurde
nicht erprobt, und in diesen Sitzungen wurde kein Hörtest bestätigt.

===========================================================================
RECHTE
===========================================================================

(c) 2026 Belk Siri. Alle Rechte vorbehalten.

Diese Dateien werden als Begleitung zum Buch „GNU Radio Schritt für
Schritt“ bereitgestellt. Das Herunterladen und der persönliche Gebrauch
sind gestattet. Ein Recht zur Weiterverwendung, zur öffentlichen Änderung
oder zur Weitergabe wird zum jetzigen Zeitpunkt nicht eingeräumt.

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
Datei. Die Prüfsumme des Archivs selbst steht auf der Seite des Bandes:
https://belksiri.github.io/books/gnu-radio-pas-a-pas/de/volume-2/

===========================================================================
SEITE ZUM BUCH
===========================================================================

https://belksiri.github.io/books/gnu-radio-pas-a-pas/

Die deutsche Korrekturseite:
https://belksiri.github.io/books/gnu-radio-pas-a-pas/de/korrekturen/
