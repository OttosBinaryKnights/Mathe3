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

wie 7.3 gelöst.

1. Stichprobe

2. Punktschätzung

  $\bar{x} = 16$

3. Schätzung Streuung

  $s^* = \sqrt{484}$

4. Konfidenzniveau

  $\gamma = 0.99 \rightarrow -> z= 2.58$

5. Einsetzen in Formel für Konfidenzintervalle:
### FALSCH! Es wurde nach Konfidenzintervall für $\sigma^2$ gefragt
  $$\mu \in [\bar{x} - z* \frac{s^*}{\sqrt{n}};\bar{x} + z* \frac{s^*}{\sqrt{n}}]\text{ zu Konfidenz }\gamma$$


  $\mu \in [4.648;27.352] \text{ zu Konfidenz }\gamma$



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

      $$|\frac{x}{n}-P| \leq 3* \frac{\sigma}{n}$$

      $$|0.526 - P| \leq 3* \frac{\sqrt{3000*P*(1-P)}}{3000}$$
      $$(0.526 - P)^2 \leq 9* \frac{P*(1-P)}{3000}$$
      $$0.526^2 - 1.052 P + P^2 \leq 9* \frac{P*(1-P)}{3000}$$
      $$830.028 - 3156 P + 3000 P^2 \leq 9P-9P^2$$
      $$830.028 - 3165 P + 3009 P^2 \leq 0$$

      $$p_{1} = 0.498614$$
      $$p_{2} = 0.55323$$

---
# Aufgabe 7.5
**Sei  die  Funktion $f: D\rightarrow R$ mit $f(x)= tan(x)$ an den Stützstellen $(0,f(0)),(\frac16, f(\frac16))$ und $(\frac14, f(\frac14))$ gegeben.**

(a) **Bestimmen Sie das Interpolationspolynom $P_2(x) = a_0+a_1x+a_2x^2$.**

(b) **Benutzen Sie zur Interpolation $Q(x) = b_0 + b_1x + b_2\frac{1}{x-\frac12}$, d. h. berechnen Sie die Konstanten $b_0, b_1$ und $b_2$ von $Q(x)$.**

(c)  **Welche Näherungen ergeben sich aus (a) und (b) für $tan(20\deg)$?**
