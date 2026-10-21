# LaTeX-Workshop anhand der Fickschen Gesetze

Materialien für einen 90-minütigen LaTeX-Workshop für Physikstudierende. Die Teilnehmenden setzen dabei selbst ein kleines Dokument: eine Zusammenfassung über die Fickschen Diffusionsgesetze. Darin stehen Abschnitte in eigenen Dateien, nummerierte Gleichungen, Abbildungen, eine Tabelle und ein Literaturverzeichnis. Der Text ist schon vorhanden, es geht nur ums Setzen. So passt der Workshop für Einsteiger*innen und für alle, die schon ein bisschen LaTeX können.

### Mahelie Dissanayake, 04.11.2026

## Inhalt

| Datei | Was ist das? |
|---|---|
| [`LaTeX-Workshop.pptx`] | Präsentationsfolien: kurze Geschichte von TeX und LaTeX, Vorteile, Grundlagen, die fünf Aufgaben und Quellen |
| [`Aufgabenblatt`]| Aufgabenblatt als PDF, als Word-Datei und als LaTeX-Quelltext |
| [`Spickzettel.pdf`] | Zusammenfassung der wichtigsten Befehle  |
| [`Starter.zip`]| Starter-Projekt für die Teilnehmenden: Text und Kopfzeile fertig, Formatierung fehlt (siehe `TODO`-Kommentare) |
| [`Loesung/`] | Musterlösung als PDF und als ZIP zum Hochladen auf Overleaf

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
| 1 · Grundgerüst | Dokumentklasse `scrartcl`, Pakete, Titel mit `\maketitle` auf eigener Titelseite | 7 min |
| 2 · Struktur & Text | Präambel und Abschnitte in eigene Dateien (`\input`), `\section`, Inhaltsverzeichnis auf eigener Seite, Listen | 7 min |
| 3 · Formeln | `equation` und `align`, eigene Befehle mit `\newcommand`, Verweise mit `\eqref` | 12 min |
| 4 · Abbildungen & Tabelle | `figure` mit `\includegraphics`, Tabellen mit `booktabs`, `\caption`, `\label`, `\ref` | 8 min |
| 5 · Literatur & Querverweise | `biblatex` mit `\cite`, Literaturverzeichnis auf eigener Seite, klickbare Links mit `hyperref` | 6 min |

Jeder Schritt spielt sich hauptsächlich in einer Datei ab. Wer hängen bleibt, kann trotzdem mit dem nächsten Schritt weitermachen.

## Loslegen

**In Overleaf** (empfohlen, keine Installation nötig):

1. [`Starter.zip`] herunterladen.
2. In [Overleaf](https://www.overleaf.com) auf **New Project → Upload Project** gehen und die ZIP-Datei hochladen.
3. Das Aufgabenblatt (`Aufgabenblatt.pdf`) liegt mit im Projekt. Einfach bei Schritt 1 anfangen.

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
Das Material steht unter der Lizenz [Creative Commons Namensnennung 4.0 International (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/deed.de). Ihr dürft es frei nutzen, verändern und weitergeben, auch für eigene Workshops. Bedingung ist, dass ihr mich als Urheberin nennt, auf die Lizenz verweist und angebt, ob ihr etwas geändert habt. Den vollständigen Lizenztext findet ihr in [`LICENSE`](LICENSE).
