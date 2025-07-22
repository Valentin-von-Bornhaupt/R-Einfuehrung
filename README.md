# Eine kurze Einführung in die Programmierung mit R
Autoren: Valentin von Bornhaupt und Dr. Michael Welter

[PDF-Download](https://github.com/Valentin-von-Bornhaupt/R-Einfuehrung/releases)

Dieses Skript ist eine Einführung in die Programmierung mit R. Es richtet sich an Studierende des Biologie-Bachelors der Universität Bonn, die noch keine oder nur wenig Erfahrung mit der Programmiersprache R haben. Ziel ist es, die Grundlagen der Programmierung zu vermitteln und die Studierenden in die Lage zu versetzen, einfache Programme in R zu schreiben.

## Inhalt
01. Start
02. Kommentare
03. Taschenrechner
04. Variablen
05. Vektoren
06. Grafiken
07. If-Verzweigungen
08. For-Schleifen
09. Funktionen
10. Matrizen
11. Dataframes


## Hinweise für die Weiterentwicklung
- Für das Kompilieren muss R und Knitr installiert sein. LaTeX muss zugriff auf R haben. Das einfachste ist, alle Dateien bei Overleaf zu öffnen und dort zu kompilieren -- dort ist bereits alles vorinstalliert.

Hinweise zu Knitr:
- R-Code zwischen `<<>>=` und `@` einfügen. 
```r
   <<>>=
   # Hier kommt R-Code hin
   @ 
   ```
Knitr kann Parameter in `<<>>=` entgegebennehmen:
- Für mögliche Parameter schreibe `<<PARAMETER>>=` statt `<<>>=`
- Mehrere `PARAMETER` werden durch `,` separiert.

Von mir bislang genutzte Knitr-Parameter:
- Grafikausgabegröße fixieren + Zentrieren
`fig.width = 4, fig.height = 4.4, fig.align='center'`
- Code nicht anzeigen (wird dennoch ausgeführt): `include = FALSE`
- Code nicht ausführen (wird dennoch angezeigt): `eval = FALSE`
- Schriftgröße: `size="huge"`, Ordnung:
`Huge > huge > LARGE > Large > large > normalsize > small > footnotesize > scriptsize > tiny`

Bugs:
- Leider gibt es Probleme mit Text-Overflow bei Knitr-Ausgaben in mit dem DIN A4 Papierformat. Ein Workaround wäre die Schriftgröße in den Code-Blöcken anzupassen (siehe `main.Rtex`). Aber das ist nicht schön.