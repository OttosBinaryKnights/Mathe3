# Übung 7
## Aufgabe 7.1
**Eine Maschine produziert Gehäuseteile eines Computers mit einem Ausschussanteil von 9%.**

(a) **Nach welcher Verteilung bestimmt sich die Anzahl der brauchbaren Gehäuseteile in einer Anzahl $n$ von produzierten Gehäuseteilen.**

Normalverteilung?!

(b) **Berechnen Sie mit einer geeigneten Näherung die Wahrscheinlichkeit für 110 oder mehr brauchbare  Gehäuseteile in einer Produktion von 1000 Gehäuseteilen.**
**Begründen Sie: Warum dürfen Sie die Näherung verwenden?**

$X:$  brauchbare Gehäuseteile bei Produktion von 1000

$P(X \geq 110)$

---
## Aufgabe 7.2
**Aus  der  Produktion  von  Zylinderschrauben  wird  eine  Stichprobe vom Umfang $n=25$ entnommen und an jeder Schraube die Schaftlänge gemessen. Die Stichprobe ergibt $\bar{x} = 16 mm$ und $s^2= 484 \mu m^2$. Bestimmen Sie ein Kondenzintervall für $\sigma^2$ unter der Voraussetzung, dass das Kondenzniveau $0.99$ beträgt.**

* $n = 25$
* $\bar{x} = 16$
* empirische Varianz:
  $\bar{s}^2 = 484$

Gelöst nach [Henk-Skript 20.19](https://www.math.uni-magdeburg.de/owncloud/public.php?service=files&t=3fd7efaa203e7903d230efac8438d854)

1. Konfidenzniveau

  $\gamma = 0.99 \rightarrow -> z= 2.58$

2. Bestimme das $1-\alpha/2$ und $\alpha/2$-Quantil   $z_{1-\alpha/2},z_{\alpha/2}$ der $X^2$-Verteilung mit $n-1$ Freiheitsgraden

  $z_{1-\alpha/2} = 1 - \frac{0.01}{2}=0.995$

  $z_{\alpha/2} = \frac{0.01}{2}=0.005$

  *$z_u$ und $z_o$ aus [Tabelle der  Chi-Quadrat-Verteilung](https://de.wikibooks.org/wiki/Statistik:_Tabelle_der_Chi-Quadrat-Verteilung):*

  $df = n-1 = 24$ (degrees of freedom = Freiheitsgrade)

  (für $df=24, p=0.995$)

  $\rightarrow X^2_{0.995;24} = 45.56$

  (für $df=24, p=0.005$)

  $\rightarrow X^2_{0.005;24} = 9.89$
3. Intervall:

  $$\sigma^2 \in [\frac{(n-1) \bar{s}^2}{X^2_{1-\frac{\alpha}{2}; n-1}};
  \frac{(n-1) \bar{s}^2}{X^2_{\frac{\alpha}{2}; n-1}}]\text{ zu Konfidenz }\gamma$$

  $$\sigma^2 \in [\frac{(25-1) 484}{45.56};
  \frac{(25-1) 484}{9.89}]$$

  $$\approx [254.96, 1174.52]$$




---
## Aufgabe 7.3
**$X_1,...,X_n$ sei eine unabhängige, identisch verteilte Stichprobe  einer  normalverteilten  Zufallsvariablen $X$,  von der $\mu$ und $\sigma^2$ unbekannt sind. Bestimmen Sie ein Kondenzintervall für $\mu$ zum Vertrauensgrad $1-\alpha = 0.95$ aus den Stichprobenwerten 104, 115, 112, 89, 94, 106, 119, 99, 102 und 90.**

gelöst mit Hilfe des Videos: (https://www.youtube.com/watch?v=DdwTa28W4Os)

1. Stichprobe

  104, 115, 112, 89, 94, 106, 119, 99, 102, 90
2. Punktschätzung

  $\bar{x} = \frac{ 104 + 115 + 112 + 89 + ... + 90}{10} = 103$

3. Schätzung Streuung

  $s^* = \sqrt{\frac{ (104 -103)^2 + (115-103)^2  ... }{10-1} }= \sqrt{106}$

4. Konfidenzniveau

  $\gamma = 0.95 \rightarrow -> z= 1.96$

5. Einsetzen in Formel für Konfidenzintervalle:
  $$\mu \in [\bar{x} - z* \frac{s^*}{\sqrt{n}};\bar{x} + z* \frac{s^*}{\sqrt{n}}]\text{ zu Konfidenz }\gamma$$

  $103 - 1,96* \frac{\sqrt{106}}{\sqrt{10}} = 96.6187$

  $103 + 1,96* \frac{\sqrt{106}}{\sqrt{10}} = 109.381$

    $\mu \in [96.6187;109.381]\text{ zu Konfidenz }\gamma$
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

(b) **Benutzen Sie zur Interpolation $Q(x) = b_0 + b_1x + b_2\frac{1}{x-\frac12}$, d. h. berechnen Sie die Konstanten $b_0, b_1$ und $b_2$ von $Q(x)$.**

(c)  **Welche Näherungen ergeben sich aus (a) und (b) für $tan(20\deg)$?**
