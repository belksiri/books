GNU Radio Step by Step - Volume 1
Fundamentals, GNU Radio Companion, and Signal Processing
Chapters 1 to 26

Belk Siri - reader resources v1.0.0 (2026-09-20)

===========================================================================
WHAT THIS ARCHIVE CONTAINS
===========================================================================

34 files, 718067 bytes.

  flowgraphs/CHnn/   the example flowgraphs of the chapters
  flowgraphs/TP-nn/  the flowgraphs of the hands-on exercises

The folders are named after the stable identifiers of the book, which are
the same in every language: CH02 is Chapter 2, and TP-03 is Exercise 3.
The folder names are never translated, so that one archive serves every
edition.

The audio file book-audio.wav is placed INSIDE the folder of each hands-on
exercise that reads it. The flowgraphs name it by itself, so in the current
folder: it must stay next to the .grc file. Copy the whole folder, not just
the .grc.

Two files are NOT provided, because you are the one who produces them:
echantillons.iq, written by the flowgraph of Exercise 8, and the .cfile of
real samples recorded in Exercise 18. Their names come from the book and
are not translated either: they are the names the flowgraphs write.

The layout is the one the book announces in the section "Getting and using
the files of this book": one folder per chapter or per hands-on exercise,
named after its identifier. The file name repeats the identifier of the
flowgraph in lowercase; it is also written in the Options block, which
lets you find it again after a rename.

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
  The measurements of Chapters 8 to 11 of Volume 2 were made with an
  RTL2832U dongle and an R820T tuner actually plugged in, antenna
  connected, real transmissions actually received.
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

The file audio/book-audio.wav is an original synthesis produced for the
book: six notes at the exact frequencies 220, 330, 440, 550, 440 and
220 Hz, 44,100 samples per second, one channel, 16 bits, 6 seconds. It
contains no third-party recording and no voice.

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

The file MANIFEST.json gives the path, the size and the SHA-256 checksum of
every file. To verify one file:

  macOS     shasum -a 256 flowgraphs/TP-03/fg_tp03_001.grc
  Windows   certutil -hashfile flowgraphs\TP-03\fg_tp03_001.grc SHA256
  Linux     sha256sum flowgraphs/TP-03/fg_tp03_001.grc

The checksum of the archive itself is published on the volume page:
https://belksiri.github.io/books/gnu-radio-pas-a-pas/en/volume-1/

===========================================================================
ONE ARCHIVE FOR EVERY EDITION
===========================================================================

This archive is shared by the French and English editions. It keeps its
original name, gnu-radio-pas-a-pas-volume-1-resources.zip, and its
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
