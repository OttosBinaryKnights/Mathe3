# Übung 6
## Aufgabe 6.1
**Die Länge $X$ (in mm) von Leiterplatten sei angenähert normalverteilt mit Erwartungswert $ \mu = 15$. Ermitteln Sie die Varianz, wenn 98% der Leiterplatten zwischen $14 mm$ und $16 mm$ lang sind.**

$z= \frac{k-\mu}{\sigma}$

$\Phi(z)- \Phi(-z) = 0.98$

$\Phi(z)- (1-\Phi(z)) = 0.98$

$2*\Phi(z)- 1 = 0.98$

$\Phi(z) = 1.98/2$

$\Phi(z) = 0.99 \rightarrow \text{aus Tabelle bei }z=2.33$

Standardverteilung:
$\sigma= \frac{k-\mu}{z} = \frac1{2.33} \approx 0.429$

Varianz:
$\sigma^2= \frac1{2.33}^2 \approx 0.18 mm^2$

---
## Aufgabe 6.2

---
## Aufgabe 6.3
**In einem großen Netzwerk treten pro Tag im  Durchschnitt 16 Störungen auf. Man kann annehmen, dass die Anzahl der  Störungen *poissonverteilt* ist. Wie groß ist die Wahrscheinlichkeit, dass pro Tag mehr als 20 Störungen auftreten?**
*Poissonverteilung:*
$$P_\lambda(k) = \frac{ \lambda ^ k}{k!}e^{-\lambda}$$
$$F(n) =e^{-\lambda} \sum_{k=0}^{n} \frac{\lambda^{k}}{k!}$$

diskrete Werte:

$P_{16}(X > 20) = 1-F(20) = 1 - e^{-16} \sum_{k=0}^{20} \frac{16^{k}}{k!} \approx 0.131832$

*Formel berechnet mit [Wolfram Alpha (Eingabe mit verlinkt)](http://www.wolframalpha.com/input/?i=1-e%5E%28-16%29+sum%2816%5Ek%2F%28k%21%29%29+k%3D0+to+20)*

## Aufgabe 6.4
**Eine Lieferung von 60 USB-Sticks, die 8 fehlerhafte  Sticks enthält, wird einer Qualitätskontrolle unterzogen.  Hierzu werden 5 der  60 Sticks herausgegriffen und überpruft. Die Lieferung wird zurückgeschickt, wenn unter den 5 geprüften Sticks einer fehlerhaft ist. Ermitteln Sie mithilfe der Hypergeometrischen Verteilung, mit welcher  Wahrscheinlichkeit die Lieferung zurückgeschickt wird.**

## Aufgabe 6.5
**Ein Computernetz besteht aus 10 unabhängig voneinander arbeitenden Computern. Jeder dieser 10 Computer fällt in der Zeit T mit der Wahrscheinlichkeit $0.05$ aus. Mit  Hilfe der Ungleichung von Tschebyschewsoll die Wahrscheinlichkeit dafur abgeschätzt werden, dass der absolute Betrag der Differenz zwischen der Zahl der  ausgefallenen Computer und dem Erwartungswert dieser Zufallsvariablen groößer als 2 ist.**
