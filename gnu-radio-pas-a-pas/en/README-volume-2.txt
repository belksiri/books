GNU Radio Step by Step - Volume 2
Modulation, Digital Communications, and RTL-SDR
Chapters 1 to 16

Belk Siri - reader resources v1.0.1 (2026-09-21)

===========================================================================
CHAPTER NUMBERING
===========================================================================

Volume 2 reads on its own: its chapters are printed 1 to 16.

The folders and file names in this archive carry the INTERNAL TECHNICAL
IDENTIFIER of the chapter (CH27 to CH42). Those identifiers are kept so the
files stay compatible: they never change, from one edition to the next or
from one language to the next, and they are also written into the Options
block of every flowgraph.

  printed chapter 1   ->  internal identifier CH27   Principles of modulation
  printed chapter 2   ->  internal identifier CH28   Amplitude modulation (AM)
  printed chapter 3   ->  internal identifier CH29   Frequency modulation (FM)
  printed chapter 4   ->  internal identifier CH30   From bit to symbol: ASK and FSK
  printed chapter 5   ->  internal identifier CH31   Phase modulation and QAM
  printed chapter 6   ->  internal identifier CH32   The imperfect channel
  printed chapter 7   ->  internal identifier CH33   The RTL-SDR
  printed chapter 8   ->  internal identifier CH34   Installing and detecting the RTL-SDR
  printed chapter 9   ->  internal identifier CH35   Tuning the receiver
  printed chapter 10  ->  internal identifier CH36   Receiving FM radio
  printed chapter 11  ->  internal identifier CH37   Recording, replaying, and exploring
  printed chapter 12  ->  internal identifier CH38   Good practice, troubleshooting, and the legal framework
  printed chapter 13  ->  internal identifier CH39   Reading and modifying the generated Python code
  printed chapter 14  ->  internal identifier CH40   Embedded Python Blocks
  printed chapter 15  ->  internal identifier CH41   OOT modules and the ecosystem
  printed chapter 16  ->  internal identifier CH42   Resources and learning paths

The TP-nn folders are not affected: the hands-on exercises keep their
number, the same in the book and in the archive. Exercise 11 of the book is
folder TP-11.

===========================================================================
WHAT THIS ARCHIVE CONTAINS
===========================================================================

16 files, 631172 bytes, arranged by printed chapter:

  chapter 2   flowgraphs/TP-11/fg_tp11_001.grc
  chapter 3   flowgraphs/TP-12/book-audio.wav
  chapter 3   flowgraphs/TP-12/fg_tp12_001.grc
  chapter 3   flowgraphs/TP-12/fg_tp12_002.grc
  chapter 4   flowgraphs/TP-13/fg_tp13_001.grc
  chapter 4   flowgraphs/TP-13/fg_tp13_002.grc
  chapter 5   flowgraphs/TP-14/fg_tp14_001.grc
  chapter 6   flowgraphs/TP-15/fg_tp15_001.grc
  chapter 6   flowgraphs/TP-15/fg_tp15_002.grc
  chapter 8   flowgraphs/CH34/fg_ch34_001.grc
  chapter 9   flowgraphs/TP-16/fg_tp16_001.grc
  chapter 10  flowgraphs/TP-17/fg_tp17_001.grc
  chapter 10  flowgraphs/TP-17/fg_tp17_002.grc
  chapter 11  flowgraphs/TP-18/fg_tp18_001.grc
  chapter 11  flowgraphs/TP-18/fg_tp18_002.grc
  chapter 14  flowgraphs/CH40/fg_ch40_001.grc

  flowgraphs/CHnn/   the example flowgraphs of the chapters
  flowgraphs/TP-nn/  the flowgraphs of the hands-on exercises

The audio file book-audio.wav is placed INSIDE the folder of each hands-on
exercise that reads it. The flowgraphs name it by itself, so in the current
folder: it must stay next to the .grc file. Copy the whole folder, not just
the .grc.

Two files are NOT provided, because you are the one who produces them:
echantillons.iq, written by the flowgraph of Exercise 8 in Volume 1, and the
.cfile of real samples recorded in Exercise 18. Their names come from the
book and are not translated either: they are the names the flowgraphs write.

Chapters 1, 7, 12, 13, 15 and 16 have no flowgraph: they are chapters of
explanation, of method or of reference. Chapter 9 has no folder of its own:
its flowgraph is the one of Exercise 16.

===========================================================================
REFERENCE VERSIONS
===========================================================================

  GNU Radio    3.10.12.0
  Radioconda   2025.03.14 (osx-arm64)
  System       macOS 26.6.2, Apple Silicon

The flowgraphs were saved with GNU Radio 3.10.12.0. Open them with the same
version, or with a more recent version of the 3.10 series. An older version
will not be able to read them: the file format changed between 3.7 and 3.8.

===========================================================================
GETTING STARTED
===========================================================================

1. Unzip this archive into your working folder.
2. Copy the folder of the chapter you are interested in into your own
   flowgraphs/ folder, then work on the copy. The exercises will have you
   change values; the original lets you go back to the starting state
   without downloading again.
3. Open the .grc file in GNU Radio Companion (menu File, then Open).
4. Generate with F5, run with F6, stop with F7.

The Python program that GRC writes next to the .grc file is rebuilt at
every generation. It is not provided here, and there is never any reason
to edit it or to save it.

===========================================================================
HARDWARE
===========================================================================

5 of the flowgraphs in this archive need an RTL-SDR receiver plugged in:
they belong to chapters 8, 9, 10 and 11. The others run in simulation, with
no hardware at all.

===========================================================================
WHAT WAS ACTUALLY VERIFIED
===========================================================================

macOS 26.6.2, Apple Silicon
  Reference system of the book. Complete chain verified: loading of the
  block definitions, opening of the flowgraphs, generation, execution.
  Audio output verified with a confirmed listening test (440 Hz tone,
  3 seconds).

Windows 11 Pro 25H2 (2026-09-18)
  Installation and execution verified: installer checked, Radioconda
  isolated, GRC launched, three flowgraphs run without hardware - 39 points
  out of 39.
  NOT TRIED: the graphical installation wizard, the "radioconda Prompt",
  AUDIO OUTPUT, and any radio hardware - therefore the WinUSB driver
  installed with Zadig.

RTL-SDR receiver
  The measurements of chapters 8 to 11 were made with an RTL2832U dongle
  and an R820T tuner actually plugged in, antenna connected, real
  transmissions actually received.
  THE RTL-SDR BLOG V3, THE REFERENCE MODEL OF THE BOOK, WAS NOT TRIED.
  NO LISTENING TEST was validated during those sessions: no sound was
  produced or heard.

No other configuration was tried. What is not written here was not
verified.

===========================================================================
LICENSE
===========================================================================

(c) 2026 Belk Siri. All rights reserved.

These files are made available to accompany the book "GNU Radio Step by
Step". Downloading them and using them personally are permitted. No license
to reuse, to modify publicly or to redistribute is granted at this stage.

The file book-audio.wav is an original synthesis produced for the book: six
notes at the exact frequencies 220, 330, 440, 550, 440 and 220 Hz, 44,100
samples per second, one channel, 16 bits, 6 seconds. It contains no
third-party recording and no voice.

The .grc flowgraphs are text files created for this book. They contain no
logo, no code and no resource belonging to the GNU Radio project.

===========================================================================
NO AFFILIATION
===========================================================================

GNU Radio is cited as the software studied in this book. This independent
publication is not published, sponsored or endorsed by the GNU Radio
project or by the Free Software Foundation.

===========================================================================
VERIFYING THIS ARCHIVE
===========================================================================

The file MANIFEST.json gives the path, the printed chapter, the size and
the SHA-256 checksum of every file. To verify one file:

  macOS     shasum -a 256 flowgraphs/TP-11/fg_tp11_001.grc
  Windows   certutil -hashfile flowgraphs\TP-11\fg_tp11_001.grc SHA256
  Linux     sha256sum flowgraphs/TP-11/fg_tp11_001.grc

The checksum of the archive itself is published on the volume page:
https://belksiri.github.io/books/gnu-radio-pas-a-pas/en/volume-2/

===========================================================================
ONE ARCHIVE FOR EVERY EDITION
===========================================================================

This archive is shared by the French and English editions. It keeps its
original name, gnu-radio-pas-a-pas-volume-2-resources.zip, and its
checksum: the French edition is already published and prints that checksum
on paper. Renaming the archive or rebuilding it would invalidate what is
printed in a book that is already in the hands of readers.

A .grc file holds official GNU Radio block names, numeric values and stable
identifiers. None of that depends on the language of the book, which is why
there is one archive and not two.

===========================================================================
BOOK PAGE
===========================================================================

https://belksiri.github.io/books/gnu-radio-pas-a-pas/en/

Corrections, updates and problem reports are there.
