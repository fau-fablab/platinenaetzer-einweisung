Platinenätzer Einweisung
========================

Einweisung des [FAU FabLab](https://fablab.fau.de) in die [Platinenfertigung](https://fablab.fau.de/tool/elektronikmessen-loeten-etc/platinenfertigung/) mit Belichter und Sprühätzer.

Inhalt
------

- Regeln und Hinweise, verwendete Materialien und Chemikalien, Kosten
- Einseitige Platinen: Layout drucken, belichten, entwickeln, ätzen, entschichten, verzinnen, bohren
- Doppelseitige Platinen: Layout ausrichten, Durchkontaktieren mit der DuKo-Presse
- Wartung für Betreuer: Ätzlösung wechseln, Einstellungen des Sprühätzers

Download
--------

Die neueste Version aus [GitHub](https://github.com/fau-fablab/platinenaetzer-einweisung) ist als PDF abrufbar:

- [Einweisung](https://brain.fablab.fau.de/build/platinenaetzer-einweisung/Einweisung_Platinenaetzer.pdf)
- [Einweisungsliste](https://brain.fablab.fau.de/build/platinenaetzer-einweisung/Einweisungsliste_Platinenaetzer.pdf)
- [Betriebsanweisung Sprühätzer](https://brain.fablab.fau.de/build/platinenaetzer-einweisung/Betriebsanweisung_Spruehaetzer.pdf) (Entwurf, noch nicht freigegeben)

Außerdem baut eine GitHub Action die PDFs bei jedem Push. Auf dem Hauptbranch entsteht dabei ein
[Release](https://github.com/fau-fablab/platinenaetzer-einweisung/releases) mit Datums-Version (`vJJJJ.MM.TT`) und den PDFs.

Auschecken und bauen
--------------------

```bash
git clone --recursive git@github.com:fau-fablab/platinenaetzer-einweisung.git
cd platinenaetzer-einweisung
make
```

Die PDFs landen in `output/`. Layout, Kopf- und Fußzeile und das Logo des FAU FabLab (mit
FAU-Schriftzug) kommen aus dem Untermodul [fablab-document](https://github.com/fau-fablab/fablab-document),
das Logo wiederum aus dessen Untermodul [logo](https://github.com/fau-fablab/logo). Bei einem bestehenden
Klon die Untermodule mit `git submodule update --init --recursive` laden.

Technische Details zum Buildserver: [fau-fablab/buildserver](https://github.com/fau-fablab/buildserver)

[![Build Status](https://brain.fablab.fau.de/build/platinenaetzer-einweisung/status.svg)](https://brain.fablab.fau.de/build/platinenaetzer-einweisung/)
[![TODOs](https://brain.fablab.fau.de/build/platinenaetzer-einweisung/status-todos.svg)](https://brain.fablab.fau.de/build/platinenaetzer-einweisung/)
[![PDF bauen](https://github.com/fau-fablab/platinenaetzer-einweisung/actions/workflows/pdf.yml/badge.svg)](https://github.com/fau-fablab/platinenaetzer-einweisung/actions/workflows/pdf.yml)

Lizenz
------

[![Lizenz: CC BY-SA 3.0](https://licensebuttons.net/l/by-sa/3.0/de/88x31.png)</br>CC BY-SA 3.0](https://creativecommons.org/licenses/by-sa/3.0/)
