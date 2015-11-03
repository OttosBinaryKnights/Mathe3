# Blatt 03
## Aufgabe 3.1
**Wir  fuhren  das  Experiment  durch  "Zweimal  hintereinander würfeln".
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

$X: \text{Anzahl der Wurfe, bei denen eine gerade Zahl geworfen wird.}$
$Y: \text{Anzahl der Wurfe, bei denen eine Zahl 5 geworfen wird.}$
$ Z: \text{Ergebnis des ersten Wurfes.}$

**Welche der Zufallsvariablen sind unabhangig (Definition von Unabhangigkeit von Zufallsvariablen kommt am 29.10. in der Vorlesung). Begründen Sie Ihre Antwort!**

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

$P(1 < X <= 4) = $

---
## Aufgabe 3.4
**Die zufällige Anzahl $X$ von Ausfällen eines Servers pro Monat genügt folgender Verteilung:**

Ausfälle $x_i$ |  0  |  1  |   2  |  3  |  4  |  >4
 :---          |:---:|
$P(X=x_i)$      | 0,5 | 0,2 | 0,1  | 0,1 | 0,1 | 0

**Der Ausfall des Servers verursacht verschiedene Kosten. Der einmalige Ausfall des Servers kostet 1000EUR. Fällt der Server zweimal aus, so betragen die Kosten 1500EUR. Bei drei- und viermaligem Ausfall mussen jeweils 2000EUR bezahlt werden. Wie groß ist die Wahrscheinlichkeit dafur, dass mehr als 1000EUR Kosten im Monat wegen Ausfallen des Servers entstehen?**

$P(\text{"Mehr als 1000EUR kosten im Monat"}) = P(X >= 2) =$
$= P(X=2)+P(X=3)+P(X=4)+P(X>4) =$
$0,1 + 0,1 + 0,1 +0 = 0,3$

---
## Aufgabe 3.5
**Die  Intaktwahrscheinlichkeit  bezogen  auf  die  Zeit $t$ betragen fur  zwei  unabhängig  voneinander  arbeitende  Computernetze 0,9 bzw. 0,8. Sei $X$ die Zufallsvariable für die Anzahl der in der Zeit $t$ intakten Computernetze. Ermitteln Sie**

**(a) die Verteilungsfunktion $F(x)$,**

**(b)  die Wahrscheinlichkeit, dass in der Zeit $t$ wenigstens ein Computernetzintakt ist.**
