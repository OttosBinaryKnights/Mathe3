# Blatt 03
## Aufgabe 3.1
**Wir  führen  das  Experiment  durch  "Zweimal  hintereinander würfeln".
Welche der folgenden Ereignisse sind unabhangig.**

|   | 1 | 2 | 3 | 4 | 5 | 6 |
|---|---|---|---|---|---|
| 1 | 2 | 3 | 4 | 5 | 6 | 7 |
| 2 | 3 | 4 | 5 | 6 | 7 | 8 |
| 3 | 4 | 5 | 6 | 7 | 8 | 9 |
| 4 | 5 | 6 | 7 | 8 | 9 | 10|
| 5 | 6 | 7 | 8 | 9 | 10| 11|
| 6 | 7 | 8 | 9 | 10| 11| 12|
---
* **(a)** $A=\{(1;1);(2;2);(3;3);(4;4)\}$
$B:\text{ Augensumme groesser oder gleich 5}$

aus Tabelle:

$P(A) = \frac{4}{36} = \frac{1}{9}$

$P(B) = \frac{36-6}{36} = \frac{5}{6}$

$P(A \cap B) = \frac{2}{36}$

$P(A) * P(B) = \frac{5}{54} \neq P(A \cap B)$
$ \rightarrow $ stochastisch abhängig

---
* **(b)** $A:\text{ Ein Wurfel zeigt eine 1}$
$B:\text{ Ein Wurfel zeigt eine 2}$

aus Tabelle:

$P(A) = \frac{11}{36}$

$P(B) = \frac{11}{36}$

$P(A \cap B) = \frac{2}{36}$

$P(A) * P(B) = \frac{121}{1296} \neq P(A \cap B)$
$ \rightarrow $ stochastisch abhängig

---
* **(c)** $A: \text{Beide Augenzahlen sind gerade.}$
$B: \text{Beide Augenzahlen sind ungerade.}$

aus Tabelle:

$P(A) = \frac{9}{36}$

$P(B) = \frac{9}{36}$

$P(A \cap B) = 0$ (nicht möglich)

$P(A) * P(B) \neq 0 = P(A \cap B)$
$ \rightarrow $ stochastisch abhängig

---
* **(d)** $A: \text{Beide Augenzahlen sind gerade.}$
$B: \text{Ein Wurfel zeigt eine gerade Zahl.}$

aus Tabelle:

$P(A) = \frac{9}{36}$

$P(B) = \frac{36-9}{36} = \frac{27}{36}$

$P(A \cap B) = \frac{9}{36}$

$P(A) * P(B) =  \frac{243}{1296} \neq \frac{9}{36} = P(A \cap B)$
$ \rightarrow $ stochastisch abhängig

---
## Aufgabe 3.2
**Wir  führen  das  Experiment  durch  "Zweimal  hintereinanderwürfeln". Der Ereignisraum ist also**
$\Omega = \{1;2;3;4;5;6\} \times \{1;2;3;4;5;6\} $
**Wir definieren drei Zufallsvariablen:**

$X: \text{Anzahl der Wuerfe, bei denen eine gerade Zahl geworfen wird.}$
$Y: \text{Anzahl der Wuerfe, bei denen eine Zahl 5 geworfen wird.}$
$ Z: \text{Ergebnis des ersten Wurfes.}$

**Welche der Zufallsvariablen sind unabhangig (Definition von Unabhängigkeit von Zufallsvariablen kommt am 29.10. in der Vorlesung). Begründen Sie Ihre Antwort!**

|             |     | $\frac{1}{4}$ | für | $t=0$|
| :---------: | --- | --- | --- | --- |
|  $P(X=t)=$  |     | $\frac{1}{2}$ | für | $t=1$ |
|             |     |  $\frac{1}{4}$  | für | $t =2$ |

|             |     |  0  | für | $t<0$ |
| :---------: | --- | --- | --- | --- |
|             |     | $\frac{1}{4}$ | für | $0 <= t < 1$|
| $F(X=t)=$ |     | $\frac{3}{4}$ | für | $1 <= t < 2$ |
|             |     |  $1$  | für | $t >= 2$ |

---
## Aufgabe 3.3
**Gegeben  ist  die  Verteilungsfunktion  einer  diskreten  Zufallsvariablen**

|       |     |  0  | für | $t<0$ |
| :---: | --- | --- | --- | --- |
|       |     | 0,1 | für | $0 <= t < 2$ |
| F(t)= |     | 0,4 | für | $2 <= t < 4$ |
|       |     | 0,8 | für | $4 <= t < 6$ |
|       |     | 1 | für | $t >= 6$ |


**Berechnen Sie: $P(1 < X <= 4); P(1 <= X <= 4); P(X>=3)$.**

 * für stetige Funktion über Dichtefunktion zu lösen
 * für diskrete Funktion hingegen über?

$P(1 < X <= 4) = \int_1^4F(t)dt = $

---
## Aufgabe 3.4
**Die zufällige Anzahl $X$ von Ausfällen eines Servers pro Monat genügt folgender Verteilung:**

Ausfälle $x_i$ |  0  |  1  |   2  |  3  |  4  |  >4
 :---          |:---:|
$P(X=x_i)$      | 0,5 | 0,2 | 0,1  | 0,1 | 0,1 | 0

**Der Ausfall des Servers verursacht verschiedene Kosten. Der einmalige Ausfall des Servers kostet 1000 EUR. Fällt der Server zweimal aus, so betragen die Kosten 1500 EUR. Bei drei- und viermaligem Ausfall mussen jeweils 2000 EUR bezahlt werden. Wie groß ist die Wahrscheinlichkeit dafur, dass mehr als 1000 EUR Kosten im Monat wegen Ausfällen des Servers entstehen?**

$P(\text{"Mehr als 1000 EUR Kosten im Monat"}) = P(X >= 2) =$
$= P(X=2)+P(X=3)+P(X=4)+P(X>4) =$
$0,1 + 0,1 + 0,1 +0 = 0,3$

---
## Aufgabe 3.5
**Die  Intaktwahrscheinlichkeit  bezogen  auf  die  Zeit $t$ betragen fur  zwei  unabhängig  voneinander  arbeitende  Computernetze 0,9 bzw. 0,8. Sei $X$ die Zufallsvariable für die Anzahl der in der Zeit $t$ intakten Computernetze. Ermitteln Sie**

**(a) die Verteilungsfunktion $F(x)$,**

$A: \text{System A intakt}$

$B: \text{System B intakt}$

Intakte Systeme $x_i$ |  2  |  1  |   0  |
 :---                 |:---:|
$P(X=x_i)$            | 0,72| 0,26 | 0,02

$P(X=2) = P(A) * P(B) =0,9 * 0,8 = 0,72$

$P(X=1) = P(\overline{A}) * P(B) + P(A) * P(\overline{B}) = 0,1 * 0,8 + 0,9 * 0,2 = 0,26$

$P(X=0) = P(\overline{A}) * P(\overline{B}) = 0,1 * 0,2 = 0,02$

|       |     |  0  | für | $t<0$ |
| :---: | --- | --- | --- | --- |
| F(X)= |     | 0,02 | für | $0 <= t < 1$ |
|       |     | 0,28 | für | $1 <= t < 2$ |
|       |     | 1 | für | $2 <= t $ |

**(b)  die Wahrscheinlichkeit, dass in der Zeit $t$ wenigstens ein Computernetz intakt ist.**

Gegenereignis zu "alle ausgefallen"

$P(X>=1) = 1 - P(X=0) = 0,98$
