# Übung 9
## Aufgabe 9.1
**Gegeben sei die Funktion $f : R>10 \rightarrow R$ mit $f(x) = ln(x+10)$.**

a) **Ermitteln Sie einen Näherungswert für ln 11, 1 mithilfe der Polynominterpolation an den Stützstellen $x_0 = 0, x_1 = 1$ und $x_2 = 2$.**

$ P(x) = -0.01 x^2 + 0.1x + 2.3$

für $ln(11.1) \Rightarrow x=1.1$
$P(1.1) = 2.4089$

b) **Schätzen Sie den Interpolationsfehler für ln 11, 1 ab.**

Fehler: $ln(11.1)-P(1.1) = 2.4069.. - 2.4089 \approx -0,002$

Fehlerabschätzung ist was anderes:

c) **Wie hängt das Vorzeichen des Interpolationsfehlers von x ab?**


---
## Aufgabe 9.2
**Gegeben sei die Funktion $f : [0, 4] \rightarrow [0, 2]$ mit $f (x) = \sqrt{x}$ an den Stützstellen $x_0 = 0, x_1 = 1, x_2 = 4$.**

a) **Bestimmen Sie das Interpolationspolynom.**
mit Newton:

$P(x) = 0 + x - \frac{3}{16} x (x-1)$
$= -\frac{3}{16}x^2+\frac{19}{16}x$


b) **Berechnen Sie die kubischen Splines auf dem Intervall $[x_0,x_1]$ und $[x_1, x_2]$ unter der Bedingung $S_0^{′′}(x_0) = S_1^{′′}(x_2) = 0$.**

c) **Berechnen Sie mithilfe der Ergebnisse (a) und (b) jeweils Näherungswerte für $\sqrt{\frac13}$ und $\sqrt{3}$ und vergleichen Sie diese mit den Werten eines Rechners.**

---
## Aufgabe 9.3
**Gegeben sei die Funktion $f : R_{\leq 6} \rightarrow R$ mit $f(x) =\sqrt{6-x}$**

a) **Bestimmen Sie das Interpolationspolynom $P_3(x)$ an den Stützstellen $x_0 =-3,x_1 =2,x_2 =5$ und $x_3 =6$.**

b) **Benutzen Sie das Interpolationspolynom $P_3(x)$, um $\sqrt{2}$ näherungsweise zu berechnen.**

c) **Geben Sie einen Näherungswert für $\int_{-3}^{6}f(x) dx$ mithilfe des Interpolationspolynoms $P_3(x)$ an.**

---
## Aufgabe 9.4
**Gegeben sei die Funktion $f : R \rightarrow R$ mit $f(x) = 2x2^{-x}$.**

a) **Bestimmen Sie das Interpolationspolynom unter Verwendung der Stützstellen $x_0 = -1, x_1 = 0, x_2 = 1 ,x_3 = 2$ mithilfe der Methode von Lagrange.**

b) **Berechnen Sie näherungsweise mithilfe des Interpolationspolynoms das bestimmte Integral $\int_{-1}^{2}f(x) dx$.**

---
## Aufgabe 9.5
**Gegeben sei die Funktion $f : D \rightarrow[-1, 1]$ mit $f(x) = sin \frac{\pi}{4}x$.**

a) **Bestimmen Sie eine Näherung für das bestimmte Integral $I=\int_{0}^{2}sin \frac{\pi}{4}x dx$ indem Sie das Interpolationspolynom $P_2(x)$ an den Stützstellen $x_0 = 0,x_1 = 1 ,x_2 = 2$ der Funktion $f(x)$ benutzen.**

b) **Bestimmen Sie eine weitere Näherung für das Integral I, indem Sie als Näherung für $f(x)$ das Taylorpolynom an der Stelle $x^* = 1$ benutzen.**

c) **Vergleichen Sie die unter (a) und (b) erhaltenen Näherungswerte mit einem Wert aus dem Taschenrechner.**
