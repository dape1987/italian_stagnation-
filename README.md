# Capire la stagnazione italiana

Slide Beamer (16:9, circa 25 minuti) per un seminario interno sulla stagnazione italiana di lungo periodo, a partire da Krahé M. (2023), *Understanding Italy’s Stagnation*, Dezernat Zukunft, Background Paper.

## File

- `main.tex`: le slide. Ogni frame è `\begin{frame}{Titolo}{Etichetta}`; l’etichetta compare sopra il titolo.
- `references.bib`: i riferimenti citati, dalla bibliografia del paper.
- `plainnat-it.bst`: `plainnat` con “e” al posto di “and” nelle citazioni.

## Overleaf

New Project → Import from GitHub → `italian_stagnation`. Compilatore: pdfLaTeX (predefinito).

## Da completare

- `[Relatore]` e `[data]` nel preambolo (`\author`, `\date`).
- Note del relatore: sono già nei `\note{}`; per vederle, togliere il commento a `\setbeameroption{show notes on second screen=right}`.

## Macro per modificare il contenuto

| Macro | Uso |
|---|---|
| `\card{titolo}{testo}` | colonna con filetto in alto |
| `\statcard{numero}{testo}` | numero grande con didascalia |
| `\riga{etichetta}{testo}` | riga di una tabella “etichetta–testo” |
| `\nota{testo}` | riquadro grigio con il messaggio chiave |
| `\fonte{testo}` | fonte in basso a sinistra |
| `\darkslide`, `\altslide` | sfondo blu o grigio (dentro `{...}` attorno alla frame) |

I grafici a barre sono in `pgfplots`: per cambiare un valore basta modificare le coordinate in `\addplot`.
