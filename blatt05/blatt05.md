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

## Aufgabe 5.2
**Wir  führen  das  Experiment  durch  "Dreimal  hintereinander eine Münze werfen". Wir definieren zwei Zufallsvariablen $X$ und $Y$ zu diesem Zufallsexperiment wie folgt:**

| $X=$ | $0$ wenn im ersten Wurf "Kopf " geworfen wird|
| --- | --- |
|  | $1$ **sonst** |

**und $Y=$"Anzahl Würfe, die "Kopf" zeigen".**

**Bestimmen Sie Erwartungswert und Varianz von $X;Y;X+Y$ sowie $XY$.**

## Aufgabe 5.3
**Ein  Computerhersteller  erhalt  regelmaig  Lieferungen,  dieaus  jeweilsN= 100Erzeugnissen  bestehen.  Aus  statistischen  Unterlagengeht hervor, dass die Zahl der in einer Lieferung enthaltenen Ausschussstuckeeine  Zufallsvariable  ist,  die  binomialverteilt  ist  mit  den  Parameternn= 2undp= 0;1.  Einer  Lieferung  mit  unbekanntem  Ausschussanteil  werdenm= 10Qualitatskontrollproben  entnommen.  Die  gesamte  Lieferung  wirdnur dann angenommen, wenn allem= 10Erzeugnisse qualitatsgerecht sind.**
(a)  **Wie  gro  ist  die  Wahrscheinlichkeit  dafur,  dass  eine  Lieferungk=0;1;2Ausschussstucke enthalt?**
(b)  **Bestimmen Sie die Wahrscheinlichkeit dafur, dass eine Lieferung an-genommen wird.**
(c)  **Wie viel Sendungen muss der Computerhersteller durchschnittlich erhalten, damit insgesamt ein Ausschussstuck erwartet werden muss?**

## Aufgabe 5.4
**In einer Werkstatt einer Computerrma unterliege die zufalligeReparaturzeit  eines  Computers  einer  Exponentialverteilung  mit  dem  Para-meter= 0;5.
(a)  Bestimmen  Sie  die  Wahrscheinlichkeit  dafur,  dass  zur  Reparatur  ei-nes  beliebigen  Computers  mindestens  3  Stunden  aufgewendet  werdenmussen.
(b)  Wie viele Stunden werden im Durchschnitt zur Reparatur eines Com-puters benotigt?

## Aufgabe 5.5
**Die  Breite  des  Controllers  auf  einem  USB-StickXin  mmlasst  sich  als  Zufallsvariable  auassen.Xsei  normalverteilt  und  habe  denMittelwert= 10mm und die Standardabweichung= 0;02mm.(a)  Wieviel Prozent Ausschuss sind zu erwarten, wenn die Breite um ma-ximal0;03mm vom Sollwert10mm abweichen soll?(b)  Wie  mussen  die  Toleranzgrenzen10cund10 +cgewahlt  werden,damit nicht mehr als5%Ausschuss entstehen?**
