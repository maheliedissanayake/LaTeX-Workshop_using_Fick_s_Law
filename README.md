# LaTeX-Workshop anhand der Fickschen Gesetze

### Mahelie Dissanayake, 04.11.2026

Materialien für einen 90-minütigen LaTeX-Workshop für Physikstudierende. Die Teilnehmenden setzen dabei selbst ein kleines Dokument: eine Zusammenfassung über die Fickschen Diffusionsgesetze. 
Darin stehen Abschnitte in eigenen Dateien, nummerierte Gleichungen, Abbildungen, eine Tabelle und ein Literaturverzeichnis. Der Text ist schon vorhanden, es geht nur ums Setzen. 
So passt der Workshop für Einsteiger und für alle, die schon ein bisschen LaTeX können.

## Inhalt

| Ordner / Datei | Was ist das? |
|---|---|
| [`folien/LaTeX-Workshop.pptx`](folien/LaTeX-Workshop.pptx) | Folien: kurze Geschichte von TeX und LaTeX, Vorteile, Grundlagen, die fünf Aufgaben und Quellen |
| [`aufgaben/`](aufgaben/) | Aufgabenblatt als PDF, als Word-Datei und als LaTeX-Quelltext |
| [`starter/`](starter/) | Starter-Projekt für die Teilnehmenden: Text fertig, Formatierung fehlt (siehe `TODO`-Kommentare) |
| [`loesung/`](loesung/) | Musterlösung, fertig gesetzt als [`musterloesung.pdf`](loesung/musterloesung.pdf) |
| [`download/`](download/) | Starter-Projekt und Musterlösung als ZIP zum Hochladen in Overleaf |

## Ablauf

| Zeit | Thema |
|---|---|
| 0:00 | Geschichte & warum LaTeX? |
| 0:13 | Overleaf & die Aufgabe |
| 0:18 | Schritt 1 · Grundgerüst |
| 0:30 | Schritt 2 · Struktur & Text |
| 0:42 | Schritt 3 · Formeln |
| 1:02 | Schritt 4 · Tabelle & Abbildung |
| 1:14 | Schritt 5 · Literatur & Verweise |
| 1:24 | Fehler, Ausblick, Fragen |

Vor jeder Aufgabe zeigen ein paar Folien das Nötige. Danach arbeiten alle selbst, insgesamt etwa 40 Minuten.

## Die Aufgabe

| Schritt | Darum geht's | Zeit |
|---|---|---|
| 1 · Grundgerüst | Dokumentklasse `scrartcl`, Pakete, Titel mit `\maketitle` | 7 min |
| 2 · Struktur & Text | Präambel und Abschnitte in eigene Dateien (`\input`), `\section`, Inhaltsverzeichnis, Listen | 7 min |
| 3 · Formeln | `equation` und `align`, eigene Befehle mit `\newcommand`, Verweise mit `\eqref` | 12 min |
| 4 · Abbildungen & Tabelle | `figure` mit `\includegraphics`, Tabellen mit `booktabs`, `\caption`, `\label`, `\ref` | 8 min |
| 5 · Literatur & Querverweise | `biblatex` mit `\cite`, `\printbibliography`, klickbare Links mit `hyperref` | 6 min |

Jeder Schritt spielt sich hauptsächlich in einer Datei ab. Wer hängen bleibt, kann trotzdem mit dem nächsten Schritt weitermachen.

## Loslegen

**In Overleaf** (empfohlen, keine Installation nötig):

1. [`download/starter-projekt.zip`](download/starter-projekt.zip) herunterladen.
2. In [Overleaf](https://www.overleaf.com) auf **New Project → Upload Project** gehen und die ZIP-Datei hochladen.
3. Das Aufgabenblatt (`aufgaben.pdf`) liegt mit im Projekt. Einfach bei Schritt 1 anfangen.

**Lokal** (mit TeX Live oder MiKTeX):

```bash
cd loesung
latexmk -pdf main.tex
```

`latexmk` startet auch `biber` für das Literaturverzeichnis. Gebraucht werden unter anderem KOMA-Script, `amsmath`, `siunitx`, `booktabs` und `biblatex`. Das alles ist in einer vollständigen TeX-Live-Installation enthalten.

## Quellen

Die inhaltlichen Aussagen auf den Folien (Geschichte, Vorteile von LaTeX, Physik der Diffusion) sind mit Büchern und Fachartikeln belegt. Die Nummern unten rechts auf den Folien verweisen auf das Literaturverzeichnis auf den letzten beiden Folien.

## Lizenz

[![CC BY 4.0](https://img.shields.io/badge/Lizenz-CC%20BY%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/deed.de)

© 2026 Mahelie Dissanayake. 
Das Material steht unter der Lizenz [Creative Commons Namensnennung 4.0 International (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/deed.de). 
Ihr dürft es frei nutzen, verändern und weitergeben, auch für eigene Workshops. Bedingung ist, dass ihr mich als Urheberin nennt, auf die Lizenz verweist und angebt, ob ihr etwas geändert habt. Den vollständigen Lizenztext findet ihr in [`LICENSE`](LICENSE).
