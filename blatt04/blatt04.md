# Übung 4
## Aufgabe 4.1
**Gegeben sei eine Funktion $f:R \rightarrow R$ mit**

|f(x) = | $1 - | x - 1|$ | für $-1 <= x <= 1$
| --- | --- |
| | $0$ | **sonst** |



(a) **Zeigen Sie, dass $f$ Dichtefunktion einer Verteilungsfunktion ist.**

f(x) ist für $-1<=x<0$ negativ, somit keine gültige Dichtefunktion!

![Plotfx](Plot4.1.jpg)

(b)  **Bestimmen Sie Erwartungswert und Median**

*nicht möglich, da keine gültige Dichtefunktion*

## Aufgabe 4.2
**Gegeben sei eine Funktion $f: R \rightarrow R$ mit
$$f(x) =\frac{1}{\pi(1 +x^2)}$$**
**(a) Zeigen Sie, dass $f$ Dichtefunktion einer Verteilungsfunktion ist (Hilfreich konnte die Aufgabe 7.4 aus Mathematik II des letzten Semesters sein.).**
$$F(x) =\frac{1}{\pi} arctan(x)$$

$\int_{-\infty}^{\infty} f(x)dx =
[\frac{1}{\pi} arctan(x)]_{-\infty}^{\infty} $
$= \frac1\pi (lim_{a \rightarrow \infty}(arctan(x))-lim_{a \rightarrow -\infty}(arctan(x)))$
$= \frac1\pi (\frac\pi2-(-\frac\pi2)) $
$= 1$

-> ja Dichtefunktion

**(b)  Bestimmen Sie die Verteilungsfunktion und skizzieren Sie den Graphen der Verteilungsfunktion.**

$F(t) =
[\frac{1}{\pi} arctan(x)]_{-\infty}^{t} =
\frac{1}{\pi} lim_{a \rightarrow -\infty} [arctan(x)]_a^t=$
$=\frac{1}{\pi} lim_{a \rightarrow -\infty} (arctan(t)-arctan(a))$
$=\frac1\pi (arctan(t)+\frac{\pi}{2})$
$=\frac1\pi arctan(t)+\frac12$

![](Plot4.2.jpg)

-> Hierfür gäbe es gibt keinen Erwartungswert

## Aufgabe 4.3
**Die Lebensdauer $X$ (in Zeiteinheiten) eines Speichermedium seines Computers kann durch die Dichtefunktion **

| $f(x) =$ | $0$ | für $x <=0$|
| --- | --- |
|   | $0,06x^2e^{-0,02x^3}$ |für $x >0$ |

**beschrieben werden.**

**(a)  Bestimmen Sie die Verteilungsfunktion von X.**

$F(t) = \int_{-\infty}^t f(x) dx $

$= \int_{0}^t f(x) dx$

* *SUBSTITUIEREN:*
* $z=-0,02x^3$
* $\frac{dz}{dx}=-0.06 x^2$
* $\frac{dz}{-0.06 x^2}=dx$

$= \int_{0}^t 0.06x^2 e^z \frac{dz}{-0.06x^2}$
$= \int_{0}^t -e^z dz$
$=[-e^z]_{0}^t$

*rücksubstituieren:*

$=[-e^{-0.02 x^3}]_{0}^t$
$= -e^{-0.02 x^3} + e^0 = 1 -e^{-0.02 x^3}$



| $F(x) =$ | $0$ | für $t <=0$|
| --- | --- |
|   | $1-e^{-0.02 t^3}$ |für $t >0$ |

**(b)  Wie  groß  ist  die  Wahrscheinlichkeit  dafür,  dass  ein  solches  Bauelement mindestens 2 Zeiteinheiten ausfallfrei arbeitet?**

$P (X >= 2) =$
$=1 - F(2) $
$= 1-(1-e^{ -0.02 *2^3} )$
$= 1-(1-e^{-0,16} ) $
$= e^{-0,16} \approx 0,852 $

**(c)  Welche Zeit überleben ungefähr 90% der Bauelemente?**

$P(X>=x) = 0.9$

$1- F(x) = 1- (1-e^{-0.02 x^3}) = e^{-0.02 x^3} =0.9$
$$ e^{-0.02 x^3} = 0.9$$
$$ -0.02 x^3 = ln(0.9)$$
$$ x^3 = -ln(0.9) / 0.02$$
$$ x = \sqrt[3]{-ln(0.9) / 0.02}$$
$$ x_1 = 1.74; x_{2,3}\text{ n.def. in R }$$


## Aufgabe 4.4
**Es sei $f$ eine durch **

| $f(x) =$ | $\alpha x^2(1-x)$ |für | $0<=x<=1$
| --- |
| | 0 |für |$-\infty < x <0$ und $1< x <\infty$|

** gegebene Funktion mit $\alpha \in R$. **

(a) **Bestimmen Sie $\alpha$ so, dass $f$ die Dichtefunktion einer stetigen Zufallsgröße ist.**

Gesucht $\alpha$ für: $\int_{-\infty}^{\infty} f(x) dx <=> \int_0^1 f(x) dx = 1$

$\int_0^1 (\alpha x^2(1-x)) dx $
$= \alpha \int_0^1  x^2(1-x) dx $
$= \alpha \int_0^1  (x^2-x^3) dx $
$= \alpha( \int_0^1  x^2dx-\int_0^1 x^3 dx )$
$= \alpha([\frac{x^3}{3}]_0^1 -[\frac{x^4}{4}]_0^1)$
$= \alpha (\frac13 - \frac14)$
$= \alpha \frac{1}{12}$
$$\rightarrow \alpha = 12$$

mit $\alpha =12$ $f(x)>=0 \rightarrow$ passt

(b) **Ermittlen Sie die Verteilungsfunktion und den Erwartungswert E(X).**

Verteilungsfunktion aus Zeile bei a: $ \alpha([\frac{x^3}{3}]_0^1 -[\frac{x^4}{4}]_0^1) $


| $F(t) =$ | $0$ |für | $0<t$
| --- |
| | $4t^3 -3t^4 $ |für | $0<=t<=1$
| | 1 |für |$t>1$|

$E(X) = \int_{-\infty}^{\infty} x f(x) dx $
$= 12\int_{0}^{1}(x^3-x^4)dx$
$= 12[\frac14 x^4- \frac15x^5]_{0}^{1}$
$= \frac35$


*Median wäre
$$ \rightarrow\text{ Median bei }x=0.613272$$

(c) **Skizzieren Sie die Graphen der Dichte- und der Verteilungsfunktion.**
![Plot](Plot4.4c.jpg)
Funktionen in 2 getrennten Graphen wegen der Achsenbeschriftung

(d) **Berechnen Sie $P(X <\frac{1}{2})$ und $P(X < E(X))$.**

$P(X <\frac{1}{2}) = \int_{0}^{0.5}12x^2(1-x)dx =\frac5{16} = F(0,5)$


$P(X < E(X)) = \int_0^{\frac35} 12x^2(1-x)dx = 0.4752 = F(\frac35)$

## Aufgabe 4.5
**Die  ausfallfreie  Arbeitszeit $X$ (in  Zeiteinheiten)  einer  Art von Computerbauteilen hat die folgende Verteilungsfunktion $F(t)$:**

|  $F(t)=$  | $0$ für $t <0$ |
| --- | ---: |
| | $1-e^{-0,5t}$ für $t>=0$|

(a)  **Bestimmen Sie die Wahrscheinlichkeit dafür, dass ein solches Bauteil mindestens eine Zeiteinheit ohne Ausfall arbeitet.**

$P(X>=1) = 1- P(X<1) $
$= 1 - (P(X<=1)-P(X=1))$
$= 1- F(1) =  e^{-0.5} (\approx 0.303)$

(b) **Bestimmen  Sie  die  zugehörige  Dichtefunktion $f(x)$ der  Verteilungsfunktion $F$ und die mittlere ausfallfreie Arbeitszeit.**

$f(t) = F'(t) = - e^{-0.5t} (-0.5)=0,5 e^{-0.5t}$


|  $f(t)=$  | $0$ für $t <0$ |
| --- | ---: |
| | $0.5 e^{-0,5t}$ für $t>=0$|

*mittlere ausfallfreie Arbeitszeit E(x)*
$E(X) = \int_{-\infty}^{\infty}x*f(x) dx$
$= \int_{0}^{\infty}x*f(x) dx $
$= $

---

$\int x*0,5 e^{-0,5x} dx =
0,5 \int x*e^{-0,5x}dx =$

*partielle Integration*
$$ v = x; u' = -e^{-0,5x}$$
$$ v' = 1; u = 0,5*e^{-0,5x}$$

$$\int u v' = uv - \int u'v$$

---
das hier stimmt nicht:

TODO: Partiell Ableituen

$
[0,5*x * (-0,5)*e^{-0,5x}] - \int(0,5*(-0,5)*e^{-0,5x})=$
$[-0.25x*e^{-0,5x}]-[-0.5 e^{-0.5x}]$



$E(X) = [-0.25x*e^{-0.5x}]_{0}^{\infty}-[-0.5 e^{-0.5x}]_{0}^{\infty} =$

$=lim_{x \rightarrow \infty} (-0.25x*e^{-0,5x}+0.5 e^{-0.5x}) = ?$

---
es sollte rauskommen: (Bestätigt durch Wolfram Alpha)
$=2$
