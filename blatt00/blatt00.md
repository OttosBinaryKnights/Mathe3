# Blatt 0
## 0.1 Berechnen Sie das Integral ... auf dem Dreieck ...
$$
\int_{1}^{2}{ (\int_{x}^{2}{e^{x+y} }dy)}dx =

 \int_{1}^{2}{[e^{x+y}]^2_x}dx =$$

 $$ =\int_{1}^{2}{(e^{x+2}-e^{2x})}dx =

 [e^{x+2}-{e^{2x}\over2}]^2_1 =

\frac{e^4}{2} - e^3 +\frac{e^2}{2}
$$

oder alternativ (entlang y-Achse integrieren):

$$
\int_{1}^{2}{ (\int_{1}^{y}{e^{x+y} }dx)}dy =
\frac{e^4}{2} - e^3 +\frac{e^2}{2}
$$


## 0.2 Berechnen Sie das Volumen der Menge ...
$$
\int_{0}^{4}{ [\int_{x-1}^{x+3}{ (\int_{0}^{x+y+4}{1}dz)}dy]}dx =
\int_{0}^{4}{ [\int_{x-1}^{x+3}{ (x+y+4)} \text{ dy}]}dx = $$
$$
=\int_{0}^{4}{(8x + 20)}dx =
64+80 = 144
$$

## 0.3 Berechnen Sie das Integral ...
$$
\int_{1}^{4}{ [\int_{x}^{2x}{ (\int_{0}^{xy}{xyz} \text{ dz})}dy]}dx =
\frac{15}{64}*(4^8-1)
$$


## 0.4 Lieferung von 30 PCs, unterscheidbar, davon 4 fehlerhaft.
### a) Möglichkeiten 4 PCs aus der Lieferung zu prüfen
$$
\binom{30}{4} = {30! \over 4! * 26!} = 27405
$$


### b) Möglichkeiten 4 PCs aus der Lieferung zu prüfen, mit genau 2 defekten
$$
\binom{24}{2} * \binom{6}{2} = 4140
$$


### c) Möglichkeiten 4 PCs aus der Lieferung zu prüfen, mit genau 2 defekten
Summe aus zwei Fällen:

1. Fall: 4 funktionstüchtige PCs
$$ \binom{24}{4} $$

2. Fall: genau 1 defekter PC
$$\binom{24}{3} *  \binom{6}{1} $$

Beide Fälle addieren:
$$
 \binom{24}{4} +  \binom{24}{3} *  \binom{6}{1} = 22770
$$

## 0.5 Die Qualität von 10 Erzeugnissen wird nacheinander überpruft ("Gut-schlecht-Prüfung")

### a) Wieviele verschiedene Prüfungprotokolle möglich?
$$n = 2^{10} = 1024$$

### b) Wie viele Protokolle erhalten das Element g genau 6x?
$$n = \binom{10}{6} = {10! \over 4! * 6!} = 210$$
