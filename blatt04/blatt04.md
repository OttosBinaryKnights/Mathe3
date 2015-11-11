# Übung 4
## Aufgabe 4.1
**Gegeben sei eine Funktion $f:R \rightarrow R$ mit**

|f(x) = | $1 - | x - 1|$ | für $-1 <= x <= 1$
| --- | --- |
| | $0$ | **sonst** |
(a) **Zeigen Sie, dass $f$ Dichtefunktion einer Verteilungsfunktion ist.**

Eigenschaften einer Verteilungsfunktion:
 1. $F$ ist monoton steigend
 2. $F$ ist rechtsseitig stetig
 3. $lim_{x \rightarrow- \infty} F(x)=0$ und $lim_{x \rightarrow \infty} F(x)=1$

*Idee: *
Da Dichtefunktion Integral einer Verteilungsfunktion $F(X)$ ist müssen diese Kriterien auf das Integral von $\int f(x)=F(X)$ zutreffen.

*z.z. F(X) monoton steigend*

* $F'(x) >= 0$
da $F'(x) = f(x)$ und $f(x) >= 0$
$$ \rightarrow F(X)\text{ monoton steigend}$$

*Z.z. F(X) ist rechtsseitig stetig*

  * Da f'(x) keine Nullstellen -> ganz F(x) stetig, somit auch rechtsstetig

  TODO: (ggf. noch rechnen)

*Z.z. $lim_{x \rightarrow- \infty} F(x)=0$ und $lim_{x \rightarrow \infty} F(x)=1$ :*
* $lim_{x \rightarrow- \infty} F(x) = lim_{x \rightarrow- \infty} \int_{-\infty}^{x} 0 = 0$

* $lim_{x \rightarrow \infty} F(x) = lim_{x \rightarrow \infty} \int_{-\infty}^{x} f(x) =
\int_{-1}^{0} f(x) + \int_{0}^{1} f(x) = $

  $= \int_{-1}^{0} f(x) dx+ \int_{0}^{1} f(x) dx=
 \int_{-1}^{0} (x)dx + \int_{0}^{1} (-x+2) dx =$

 $= [0,5 x^2]_{-1}^0 + [-0,5x^2+2x]_0^1 =$

 $= -0,5 - 0,5 + 2 = 1$

(b)  **Bestimmen Sie Erwartungswert und Median**

$E(X) = \int_0^\infty (1-F(x))dx - \int_{-\infty}^0 F(x)dx = $

## Aufgabe 4.2
**Gegeben sei eine Funktionf:R!Rmitf(x) =1(1 +x2):(a)  Zeigen Sie, dassfDichtefunktion einer Verteilungsfunktion ist (Hilf-reich konnte die Aufgabe 7.4 aus Mathematik II des letzten Semesterssein.).(b)  Bestimmen Sie die Verteilungsfunktion und skizzieren Sie den Graphender Verteilungsfunktion.**

##Aufgabe 4.3
**Die LebensdauerX(in Zeiteinheiten) eines Speichermediumseines Computers kann durch die Dichtefunktionf(x) =(0furx00;06x2e0;02x3furx >0beschrieben werden.(a)  Bestimmen Sie die Verteilungsfunktion vonX.(b)  Wie  gro  ist  die  Wahrscheinlichkeit  dafur,  dass  ein  solches  Bauele-ment mindestens 2 Zeiteinheiten ausfallfrei arbeitet?(c)  Welche Zeituberleben ungefahr90%der Bauelemente?**

## Aufgabe 4.4
**Es sei $f$ eine durch $f(x) =(x2(1x)$fur0x10fur1< x <0und1< x <1gegebene Funktion mit2R.(a)  Bestimmen Sieso, dassfdie Dichtefunktion einer stetigen Zufalls-groeXist.(b)  Ermittlen Sie die Verteilungsfunktion und den ErwartungswertE(X).(c)  Skizzieren Sie die Graphen der Dichte- und der Verteilungsfunktion.(d)  Berechnen SieP(X <12)undP(X < E(X)).**

## Aufgabe 4.5
**Die  ausfallfreie  Arbeitszeit $X$ (in  Zeiteinheiten)  einer  Art von Computerbauteilen hat die folgende Verteilungsfunktion $F(t)$:**

|  $F(t)=$  | $0$ für $t <0$ |
| --- | ---: |
| | $1-e0^{0,5t}$ für $t>=0$|

(a)  **Bestimmen Sie die Wahrscheinlichkeit dafur, dass ein solches Bauteil mindestens eine Zeiteinheit ohne Ausfall arbeitet.**

(b) **Bestimmen  Sie  die  zugehörige  Dichtefunktion $f(x)$ der  Verteilungsfunktion $F$ und die mittlere ausfallfreie Arbeitszeit.**
