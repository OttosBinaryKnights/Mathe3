# Blatt 02
## Aufgabe 2.1
**Sei A Ereignis eines Zufallsexperimentes mit dem Ereignisraum $\Omega$.
Betrachten Sie die Abbildung $P' : 2\Omega \rightarrow [0,1]$ deﬁniert durch $P'(B) := P(A\cup B)$.
Untersuchen Sie, ob P' eine Wahrscheinlichkeit auf $\Omega $ deﬁniert, d.h. prüfen Sie die Eigenschaften K1,K2 und K3.**

---

## Aufgabe 2.2
**Die Modulprüfungen zur Mathematik I und II können als benotete oder unbenotete Leistungen abgelegt werden. Für den unbenoteten Leistungsnachweis entscheiden sich 30% der Studierenden in der Mathematik I und 60% in der Mathematik II. In Mathematik I erreichen 68% der Studierenden den Leistungsnachweis und in Mathematik II erhalten 62% den Leistungsnachweis beim ersten Versuch.**

$$A: \text{"Mathe 1 Schein"}$$

$$a: \text{"Mathe 1 im ersten Versuch bestanden"}$$

$$B: \text{"Mathe 2 Schein"}$$

$$b: \text{"Mathe 2 im ersten Versuch bestanden"}$$

 * **a) Wieviel % der Studierenden erreichen im ersten Versuch den Leistungsnachweis in Mathematik II, nachdem sie den Leistungsnachweis in Mathematik I im ersten Versuch erhalten haben?**

*"Wahrscheinlichkeit von b unter der Vorraussetzung a"*

 $P(b | a)
 = \frac{P(b \cap a)}{P(a)}
 = \frac{ 0,62 * 0,68 }{0,62}
 = 0,68$

 * **b) Wieviel % der Studierenden erreichen im ersten Versuch den Leistungsnachweis in Mathematik II, obwohl sie den Leistungsnachweis in Mathematik I im ersten Versuch nicht erhalten haben?**

$P(b | \bar{a})
= \frac{ P(b\cap\bar{a} )}{ P(\bar{a}) }
= \frac{ 0,62 * 0,32 }{0,62}
= 0,32$

---

## Aufgabe 2.3
**Ein roter und ein blauer Würfel werden geworfen.**

$$A: \text{"Der rote Wurfel zeigt eine gerade Zahl"}$$

$$B: \text{"Der blaue Wurfel zeigt eine gerade Zahl"}$$

$$C: \text{"Die Augensumme ist eine ungerade Zahl"}.$$
**a) Untersuchen Sie, ob die Ereignisse A,B und C paarweise unabhängig sind.**

$P(A) = 3/6 = 0,5$

$P(B) = 3/6 = 0,5$

$P(C) = 16/36 = 0,5$

wenn $P(A \cap C) = P(A) * P(C)$, dann stochastik unabhängig:

* $P(A \cap C) = 0,25 = P(A) * P(C) \rightarrow$ stoch. unabh.

* $\text{gleiche gilt fuer: }  P(B) \text{ und } P(C) \rightarrow$ stoch. unabh.

* $P(A \cap B) = 0,25 = P(A) * P(B) \rightarrow$ stoch. unabh.


**b) Sind die Ereignisse A,B und C unabhängig?**

Gleichzeitiges eintreten von A,B,C nicht möglich.

* $P(A \cap B \cap C) = 0 \neq \frac{1}{8} = P(A) * P(B) * P(C)$

 $\rightarrow$ stoch. abhängig

---
## Aufgabe 2.4
### Zwei Würfel werden geworfen.
**a) Bestimmen Sie die Wahrscheinlichkeit, die Augensumme 7 zu werfen unter
der Bedingung, dass wenigstens einmal die Augenzahl 3 geworfen wird.**

Zwei Würfel: 6^2 = 36 Kombinationen

$A:$ "Augensumme 7"

$B:$ "mindestens ein Würfel Augenzahl 3"

P(B) = 2*eine Drei + Dreierpasch=

$P(B) = \frac{2*5 + 1}{36} = \frac{11}{36}$

$P(A \cap B) = \frac{2}{36}$

$$P(A | B) = \frac{P(A \cap B)}{P(B)} = \frac{\frac{2}{36}}{\frac{11}{36}} = \frac{2}{11} = 0,181$$

**b) Bestimmen Sie die Wahrscheinlichkeit, dass die Augensumme 7 ist,
falls die Augensumme ungerade ist.**

$A:$ "Augensumme 7"

$B:$ "Augensumme ungerade"

$P(B) = \frac{18}{36} = \frac{1}{2}$

$P(A \cap B) = \frac{6}{36} = \frac{1}{6}$

$$P(A | B) = \frac{P(A \cap B)}{P(B)} = \frac{\frac{18}{36}}{\frac{6}{36}} = \frac{1}{2} = 0,5$$

---
## Aufgabe 2.5
**Für eine Firma werden drei Großrechner gekauft.
Diese haben unterschiedliche Qualitätseigenschaften.
Die Wahrscheinlichkeit dafür, dass diese länger als 4000 Stunden ausfallfrei
arbeiten, betragen 0,8; 0,7; 0,6. Sei X die Anzahl der Großrechner,
die länger als 4000 Stunden ausfallfrei arbeiten. Bestimmen Sie**

* **a) die Wahrscheinlichkeitsverteilung von X,**

$X: \text{Anzahl der Grossrechner, die laenger 4000h ausfallfrei} $

![Graph der Verteilungsfunktione](2-5a_Verteilungsbaum.jpg)

| $X = x_i$    |   $0$ |  $1$  |  $2$  |  $3$  |
| ------------ | :---: | :---: | :---: | :---: |
| $P(X = x_i)$ | 0,024 | 0,188 | 0,452 | 0,336 |


* **b) die Verteilungsfunktion,**


|          |  |  |  
| -------: | --- | --- |
|          |     | 0,000 für $t < 0$
|          |     | 0,024 für $0 <=t < 1$|
|          |  {  | 0,212 für $1 <=t < 2$ |
| $F(X) =$ |     | 0,664 für $2<= t < 3$ |
|          |     | 1,000 für $3 <= t$ |

* **c) den Graph der Verteilungsfunktion,**
![Graph der Verteilungsfunktione](2-5c_Graph_der_Verteilungsfunktion.jpg)
* **d) $P(X \ge 1)$.**

$ P(X \ge 1) = 1 - P(X = 0) = 0,976 $
