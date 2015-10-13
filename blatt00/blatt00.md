# Blatt 0
## 0.1 Berechnen Sie das Integral ... auf dem Dreieck ...
\[
\int_{1}^{2}{ (\int_{x}^{2}{e^{x+y} }dy)}dx = 

 \int_{1}^{2}{[e^{x+y}]^2_x}dx =
 
 \int_{1}^{2}{(e^{x+2}-e^{2x})}dx =

 [e^{x+2}-{e^{2x}\over2}]^2_1 =
 
\frac{e^4}{2} - e^3 +\frac{e^2}{2}

\]
## 0.2
## 0.3 Berechnen Sie das Integral ...
\[
\int_{0}^{4}{ (\int_{x-1}^{x+3}{ [\int_{0}^{x+y+4}{1}dz ]}dy)}dx =
\frac{28671}{36}
\]
## 0.4 Lieferung von 30 PCs, unterscheidbar, davon 4 fehlerhaft.
### a) Möglichkeiten 4 PCs aus der Lieferung zu prüfen
\[
4 aus 30 = {30! \over 4! * 26!} = 27405
\]
### b) Möglichkeiten 4 PCs aus der Lieferung zu prüfen, mit genau 2 defekten
\[
2 aus 24* 2 aus 6 = 4140
\]
### c) Möglichkeiten 4 PCs aus der Lieferung zu prüfen, mit genau 2 defekten
Summe aus zwei Fällen:
1. Fall: 4 funktionstüchtige PCs
2. Fall: genau 1 defekter PC
\[
4 aus 24 + 3 aus 24 * 1 aus 6 = 22770
\]

## 0.5 Die Qualität von 10 Erzeugnissen wird nacheinander überpruft ("Gut-schlecht-Prüfung")
### a) Wieviele verschiedene Prüfungprotokolle möglich?
\[n = 2^{10} = 1024\]

### b) Wie viele Protokolle erhalten das Element g genau 6x?
\[n = 6 aus 10 = {10! \over 4! 6!} = 210\]
