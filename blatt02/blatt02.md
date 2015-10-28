# Blatt 02
## Aufgabe 2.1
Sei A Ereignis eines Zufallsexperimentes mit dem Ereignisraum $\Omega$.
Betrachten Sie die Abbildung $P' : 2\Omega \rightarrow [0,1]$ deﬁniert durch $P'(B) := P(A\cup B)$.
Untersuchen Sie, ob P' eine Wahrscheinlichkeit auf $\Omega $ deﬁniert, d.h.
prüfen Sie die Eigenschaften K1,K2 und K3.

---

## Aufgabe 2.2
Die Modulprüfungen zur Mathematik I und II können als benotete oder unbenotete
Leistungen abgelegt werden. Für den unbenoteten Leistungsnachweis entscheiden
sich 30% der Studierenden in der Mathematik I und 60% in der Mathematik II.
In Mathematik I erreichen 68% der Studierenden den Leistungsnachweis und in
Mathematik II erhalten 62% den Leistungsnachweis beim ersten Versuch.
 * a) Wieviel % der Studierenden erreichen im ersten Versuch den
 Leistungsnachweis in Mathematik II, nachdem sie den Leistungsnachweis in
  Mathematik I im ersten Versuch erhalten haben?
 * b) Wieviel % der Studierenden erreichen im ersten Versuch den
  Leistungsnachweis in Mathematik II, obwohl sie den Leistungsnachweis
  in Mathematik I im ersten Versuch nicht erhalten haben?

---

## Aufgabe 2.3
Ein roter und ein blauer Würfel werden geworfen.
Seien A das Ereignis ”Der rote Würfel zeigt eine gerade Zahl”,
B das Ereignis ”Der blaue Würfel zeigt eine gerade Zahl” und C das
Ereignis ”Die Augensumme ist eine ungerade Zahl”.
* a) Untersuchen Sie, ob die Ereignisse A,B und C paarweise unabhängig sind.
* b) Sind die Ereignisse A,B und C unabhängig?

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

| $X = x_i$    |   $0$ |  $1$  |  $2$  |  $3$  |
| ------------ | :---: | :---: | :---: | :---: |
| $P(X = x_i)$ | 0,024 | 0,188 | 0,452 | 0,366 |


* **b) die Verteilungsfunktion,**
* **c) den Graph der Verteilungsfunktion,**
* **d) $P(X \ge 1)$.**
