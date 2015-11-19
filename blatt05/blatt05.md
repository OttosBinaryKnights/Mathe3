# Übung 5
## Aufgabe 5.1
 (a) **Ermitteln  Sie  Erwartungswert  und  Varianz  zu  den  Aufgaben  2.5 sowie 3.4 und 3.5.**


 | aus  [Aufg 2.5](https://github.com/OttosBinaryKnights/Mathe3/blob/master/blatt02.pdf)    |   $0$ |  $1$  |  $2$  |  $3$  |
 | ------------ | :---: | :---: | :---: | :---: |
 | $P(X = x_i)$ | 0,024 | 0,188 | 0,452 | 0,336 |

 $E(X) = 0.188 + 0.904 + 1.008 = 2.19$

 $Var(X) = (0-2.19)^2 +(1-2.19)^2 +(2-2.19)^2 +(3-2.19)^2 = 6.9044$

 ---

 aus  [Aufg. 3.4](https://github.com/OttosBinaryKnights/Mathe3/blob/master/blatt03.pdf)|  0  |  1  |   2  |  3  |  4  |  >4
  :---          |:---:|
 $P(X=x_i)$      | 0,5 | 0,2 | 0,1  | 0,1 | 0,1 | 0

 $E(X) = 0.2 + 0.2 + 0.3 + 0.4 = 1.1$

 $Var(X) = 14.05$

---
 aus  [Aufg. 3.5](https://github.com/OttosBinaryKnights/Mathe3/blob/master/blatt03.pdf)|  2  |  1  |   0  |
  :---                 |:---:|
 $P(X=x_i)$            | 0,72| 0,26 | 0,02

 $E(X) = 1.42 + 0.26 = 1.68$

 $Var(X) = 3.3872$

---
 (b) **Bestimmen Sie die Varianz zu den Aufgaben 4.1 und 4.4**

*aus [Lösung 4.1](https://github.com/OttosBinaryKnights/Mathe3/blob/master/blatt04.pdf)*:
Keine Dichtefunktion, daher kein Erwartungswert, also auch keine Varianz

---
*aus [Lösung 4.4](https://github.com/OttosBinaryKnights/Mathe3/blob/master/blatt04.pdf)*:

$E(X) = \mu = \frac35$

$Var(x) = \int (x - \mu)^2 f(x) dx$
$= \int_0^1 (x - \frac35)^2 (4x^3 -3x^4) dx$
$= \int_0^1 (x - \frac35)^2 (4x^3 -3x^4) dx$
$= [-\frac{3x^7}{7} + \frac{3x^6}{5} + \frac{73x^5}{125}  - \frac{6x^4}{5} + + \frac{12x^3}{25}]_0^1$
$= 0.035..$

---
## Aufgabe 5.2
**Wir  führen  das  Experiment  durch  "Dreimal  hintereinander eine Münze werfen". Wir definieren zwei Zufallsvariablen $X$ und $Y$ zu diesem Zufallsexperiment wie folgt:**

| $X=$ | $0$ wenn im ersten Wurf "Kopf " geworfen wird|
| --- | --- |
|  | $1$ **sonst** |

**und $Y=$"Anzahl Würfe, die "Kopf" zeigen".**

**Bestimmen Sie Erwartungswert und Varianz von $X;Y;X+Y$ sowie $XY$.**

| $X=$ | $0$ | $1$ |
| --- | --- |
|  | $\frac12$ | $\frac12$ |

$E(X)=0.5 * 0 + 0.5 * 1 = 0.5$

| $Y=$ | $0$ | $1$ | $2$ | $3$ |
| --- | --- |
|  | $\frac18$ | $\frac38$ | $\frac38$ | $\frac18$ |

$E(Y)=\frac38 + 2 * \frac38 + 3*\frac18 $
$= 4 * \frac38 $
$=1.5$

## Aufgabe 5.3
**Ein  Computerhersteller  erhält  regelmäßig  Lieferungen,  die aus  jeweils $N= 100$ Erzeugnissen  bestehen.  Aus  statistischen  Unterlagen geht hervor, dass die Zahl der in einer Lieferung enthaltenen Ausschussstücke eine  Zufallsvariable  ist,  die  binomialverteilt  ist  mit  den  Parametern $n= 2$ und $p= 0.1$.  Einer  Lieferung  mit  unbekanntem  Ausschussanteil  werden $m= 10$ Qualitatskontrollproben  entnommen.  Die  gesamte  Lieferung  wird nur dann angenommen, wenn alle $m= 10$ Erzeugnisse qualitätsgerecht sind.**

(a)  **Wie  groß  ist  die  Wahrscheinlichkeit  dafür,  dass  eine  Lieferung $k=0,1,2$ Ausschussstücke enthält?**


$$P(E)= \begin{pmatrix} n \\ k  \end{pmatrix} * p^k q^{n-k}$$

$P(2) = \begin{pmatrix} 2 \\ 2  \end{pmatrix} * 0.1^2 0.9^0 = 0.01$

$P(1) = \begin{pmatrix} 2 \\ 1  \end{pmatrix} * 0.1^1 0.9^1 = 0.18$

$P(0) = \begin{pmatrix} 2 \\ 0  \end{pmatrix} * 0.1^0 0.9^2 = 0.81$

sinnvoll??

(b)  **Bestimmen Sie die Wahrscheinlichkeit dafür, dass eine Lieferung angenommen wird.**

(c)  **Wie viel Sendungen muss der Computerhersteller durchschnittlich erhalten, damit insgesamt ein Ausschussstück erwartet werden muss?**

## Aufgabe 5.4
**In einer Werkstatt einer Computerfirma unterliege die zufällige Reparaturzeit  eines  Computers  einer  Exponentialverteilung  mit  dem  Parameter $\lambda= 0.5$.**

Das bedeutet laut [Wikipedia](https://de.wikipedia.org/wiki/Exponentialverteilung#Definition):
$$ f(x) = \begin{cases}
\lambda e^{-\lambda x} \text{ fur } x \geq 0 \\
0 \text{ fur }x < 0
\end{cases}$$

$$ F(x) = \begin{cases}
1- e^{-\lambda x} \text{ fur } x \geq 0 \\
0 \text{ fur }x < 0
\end{cases}$$

$$ E(x) = \int_0^{\infty} \lambda x e^{-\lambda x} =
 \frac1 \lambda$$

(a)  **Bestimmen  Sie  die  Wahrscheinlichkeit  dafür,  dass  zur  Reparatur  eines  beliebigen  Computers  mindestens  3  Stunden  aufgewendet  werden müssen.**

$F(X>=3) = 1- F(3) = 1- F(3)
=1 - (1- e^{-\lambda x}) = e^{-0.5*3} = 0.2231...$

(b) **Wie viele Stunden werden im Durchschnitt zur Reparatur eines Computers benötigt?**

$ E(x) = \int_0^{\infty} \lambda x e^{-\lambda x} =
 \frac1 \lambda = 2$
## Aufgabe 5.5
**Die  Breite  des  Controllers  auf  einem  USB-Stick *X* in  mm lässt  sich  als  Zufallsvariable  auffassen. $X$ sei  normalverteilt  und  habe  den Mittelwert= 10mm und die Standardabweichung $\sigma = 0.02mm$.**

Diese Aufgabestellung ist offensichtlich sehr ähnlich zu  [Aufgabe 10c und d der Uni Stuttgart](http://www.uni-stuttgart.de/bio/adamek/numerik/uestat,loe,b2.pdf)

(a) **Wieviel Prozent Ausschuss sind zu erwarten, wenn die Breite um maximal $+/-0.03mm$ vom Sollwert $10mm$ abweichen soll?**

Über Ungleichung von Tschebyschow zu lösen?

Lösung aus Stuttgart:

$P(9.97 \leq X \leq 10.03)$
$= \Phi(\frac{10.03-10.0}{0.02})-\Phi(\frac{9.97-10.0}{0.02})$
$= \Phi(1.5) - \Phi(-1.5)$
$= 0.8664$

$$\rightarrow Ausschuss = 1- P(...) = 0.1336$$

(b) **Wie  mussen  die  Toleranzgrenzen $10-c$ und $10 +c$ gewählt  werden, damit nicht mehr als 5% Ausschuss entstehen?**

Lösung aus Stuttgart:

Das Quantil der Standardnormalverteilung für 97.5% (beidseitig) ist 1.96. Daraus berechnen wir für das Quantil der Normalverteilung mit $\mu = 10$ und $\sigma = 0.02$ den Wert $10 + 1.96 * 0.02$.
Die Grenzen sind also $10 - 0.039 \leq X \leq 10 + 0.039$.
