# Übung 7
## Aufgabe 7.1
**Eine Maschine produziert Gehäuseteile eines Computers mit einem Ausschussanteil von 9%.**

(a) **Nach welcher Verteilung bestimmt sich die Anzahl der brauchbaren Gehäuseteile in einer Anzahl $n$ von produzierten Gehäuseteilen.**

Anzahl brauchbarer Teile bestimmt sich nach Binominialverteilung B(n,P)

* $X$ ~ $B(n, 0.09)$
* Bernoulli-Exp. (2 mögl. Ergebnisse, p= const.)

(b) **Berechnen Sie mit einer geeigneten Näherung die Wahrscheinlichkeit für 110 oder mehr brauchbare  Gehäuseteile in einer Produktion von 1000 Gehäuseteilen.**
**Begründen Sie: Warum dürfen Sie die Näherung verwenden?**

* $n= 1000$
* $p=0.09$

*$\Phi(z)$ verwendebar, weil LaPlace-Bedingung $\sigma = \sqrt{np(1-p)} > 9$ erfüllt mit $\sigma \approx 82$*

$X:$  brauchbare Gehäuseteile bei Produktion von 1000


$P(X \geq 110) = 1 - P(X<=109)$
$=1- \Phi(\frac{x+\frac12-(n*p)}{\sqrt(n*p*(1-p)))})$
$=1- \Phi(\frac{109+\frac12-(1000*0.91)}{\sqrt(1000*0.91*0.09)})$
$=1-\Phi(-88.45)$
$=1-(1-\Phi(88.45))$
$=\Phi(88.45)$
$=1$

---
## Aufgabe 7.2
**Aus  der  Produktion  von  Zylinderschrauben  wird  eine  Stichprobe vom Umfang $n=25$ entnommen und an jeder Schraube die Schaftlänge gemessen. Die Stichprobe ergibt $\bar{x} = 16 mm$ und $s^2= 484 \mu m^2$. Bestimmen Sie ein Kondenzintervall für $\sigma^2$ unter der Voraussetzung, dass das Kondenzniveau $0.99$ beträgt.**

* $n = 25$
* $\bar{x} = 16 mm$
* empirische Varianz:
  $\bar{s}^2 = 484 \mu m^2$

Gelöst nach [Henk-Skript 20.19](https://www.math.uni-magdeburg.de/owncloud/public.php?service=files&t=3fd7efaa203e7903d230efac8438d854)

1. Konfidenzniveau

  $\gamma = 0.99 \rightarrow -> z= 2.58$

2. Bestimme das $1-\alpha/2$ und $\alpha/2$-Quantil   $z_{1-\alpha/2},z_{\alpha/2}$ der $X^2$-Verteilung mit $n-1$ Freiheitsgraden

  $z_{1-\alpha/2} = 1 - \frac{0.01}{2}=0.995$

  $z_{\alpha/2} = \frac{0.01}{2}=0.005$

  *$z_u$ und $z_o$ aus [Tabelle der  Chi-Quadrat-Verteilung](https://de.wikibooks.org/wiki/Statistik:_Tabelle_der_Chi-Quadrat-Verteilung):*

  $df = n-1 = 24$ (degrees of freedom = Freiheitsgrade)

  (für $df=24, p=0.995$)

  $\rightarrow z_{0.995;24} = 45.56$

  (für $df=24, p=0.005$)

  $\rightarrow z_{0.005;24} = 9.89$
3. Intervall:

  $$\sigma^2 \in [\frac{(n-1) \bar{s}^2}{z_{1-\frac{\alpha}{2}; n-1}};
  \frac{(n-1) \bar{s}^2}{z_{\frac{\alpha}{2}; n-1}}]\text{ zu Konfidenz }\gamma$$

  $$\sigma^2 \in [\frac{(25-1) 484}{45.56};
  \frac{(25-1) 484}{9.89}]$$

  $$\approx [254.96, 1174.52]$$




---
## Aufgabe 7.3
**$X_1,...,X_n$ sei eine unabhängige, identisch verteilte Stichprobe  einer  normalverteilten  Zufallsvariablen $X$,  von der $\mu$ und $\sigma^2$ unbekannt sind. Bestimmen Sie ein Kondenzintervall für $\mu$ zum Vertrauensgrad $1-\alpha = 0.95$ aus den Stichprobenwerten 104, 115, 112, 89, 94, 106, 119, 99, 102 und 90.**

gelöst mit Hilfe des Videos: (https://www.youtube.com/watch?v=DdwTa28W4Os)

$\mu ges. \sigma ungbekannt -> blabla verteilung$

1. Stichprobe

  104, 115, 112, 89, 94, 106, 119, 99, 102, 90
2. Punktschätzung

  $\bar{x} = \frac{ 104 + 115 + 112 + 89 + ... + 90}{10} = 103$

3. Schätzung Streuung

  $s^* = \sqrt{\frac{ (104 -103)^2 + (115-103)^2  ... }{10-1} }= \sqrt{106}$

4. Konfidenzniveau(symmetrisch)

  $\gamma = 0.95$

  Korrektur nicht normal, nicht chi sondern __Verteilung:
  $\rightarrow z= 1.96$

  $z_{1-\alpha/2;n-1} = 2.26$


5. Einsetzen in Formel für Konfidenzintervalle:
  $$\mu \in [\bar{x} - z_{1-\alpha/2;n-1}* \frac{s^*}{\sqrt{n}};\bar{x} + z_{1-\alpha/2;n-1}* \frac{s^*}{\sqrt{n}}]\text{ zu Konfidenz }\gamma$$

  $103 - 2.26* \frac{\sqrt{106}}{\sqrt{10}} = 92.428 ... $

  $103 + 2.26* \frac{\sqrt{106}}{\sqrt{10}} = 169.678 ...$

    $\mu \in [95.64...;110.385..]$

---
## Aufgabe 7.4
**Unter 3000 Lebendgeburten wurden 1578 Knaben gezählt. Bestimmen Sie daraus ein Kondenzintervall fur die Wahrscheinlichkeit $p$ einer Knabengeburt zu $1 - \alpha = 0.99$.**

$n=3000; x=1578$

$\bar{x}=\frac{x}{n} = 1578 / 3000 = 0.526$

$\gamma = 0.99 \rightarrow z = 2.58$

$$ [p - z* \sqrt{\frac{p*(1-p)}{n}};p + z* \sqrt{\frac{p*(1-p)}{n}}]\text{ zu Konfidenz }\gamma$$

$$ [0.526 - 2.58* \sqrt{\frac{0.526*0.474}{3000}}; 0.526 + 2.58* \sqrt{\frac{0.526*0.474}{3000}}]\text{ zu Konfidenz }\gamma$$

$$ [0.50248; 0.54952]\text{ zu Konfidenz }\gamma$$

---
# Aufgabe 7.5
**Sei  die  Funktion $f: D\rightarrow R$ mit $f(x)= tan(x)$ an den Stützstellen $(0,f(0)),(\frac16, f(\frac16))$ und $(\frac14, f(\frac14))$ gegeben.**

(a) **Bestimmen Sie das Interpolationspolynom $P_2(x) = a_0+a_1x+a_2x^2$.**

*Ziel: Polynom durch die 3 gegebenen Punkte*

| | $x_0$|$x_2$|$x_1$|
| :---: | :---: | :---: | :---: |
|x| $0$ | $\frac16$ | $\frac14$ |
|y| $0$ | $\frac{\sqrt3}{3}$ | 1 |



$tan(0) = 0 = a_0$

$tan(\frac14) = 1 = a_0 + a_1 * (x_1-x_0) = a_1 * \frac14$

$\rightarrow a_1 = 4$

$tan(\frac16) = \frac{\sqrt3}{3} = a_0 + a_1 * (x_1-x_0) + a_2 * (x_2-x_0)* (x_2-x_1)$
$= 0 + 4 * (\frac14) + a_2 * (\frac16)* (-\frac{1}{12})$

$\rightarrow a_2 = $


*Newtonsche Interpolationsformel:*
$P(x) = a_0 + a_1 * (x-x_0) + a_2 * (x-x_0)* (x-x_1) $


(b) **Benutzen Sie zur Interpolation $Q(x) = b_0 + b_1x + b_2\frac{1}{x-\frac12}$, d. h. berechnen Sie die Konstanten $b_0, b_1$ und $b_2$ von $Q(x)$.**

$b_0 + b_1x+b_2 \frac{1}{x-0.5} $

$b_0 + b_1*0+b_2 \frac{1}{0-0.5}  = 0$

$b_0 + b_1 \frac16 +b_2 \frac{1}{\frac16-0.5} = \frac{\sqrt3}{3}$

$b_0 + b_1\frac14+b_2 \frac{1}{\frac14-0.5} = 1 $

Über Gauß:
$$b_0 = 2 * \sqrt{3} - 4$$
$$ b_1 = 8 \sqrt{3} - 12$$
$$ b_2 = \sqrt{3} - 2$$

(c)  **Welche Näherungen ergeben sich aus (a) und (b) für $tan(20\deg)$?**

$tan(20\deg) = tan(\frac19 \pi)$

$$P_2(\frac19) = 0.3452$$
$$Q(\frac19) = 0.3594$$
$$tan(20\deg) = 0.36$$
