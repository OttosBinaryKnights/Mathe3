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
**Für den Gesamtwiderstand $R$ von elektronischen Computerbauteilen einer Lieferung gleicher Bauart wird der Erwartungswert mit $\mu = 200 \Omega$
und die Varianz mit $\sigma^2 = 5 \Omega^2$
angegeben.**

* $\mu = 200 \Omega$ (Erwartungswert)
* $\sigma^2 = 5 \Omega^2$ (Varianz)
* $\rightarrow \sigma = \sqrt{5} \Omega$ (Standardabweichung)

a) **Wie groß ist die  Wahrscheinlichkeit, dass ein  Bauteil fehlerhaft ist, wenn der Gesamtwiderstand $R$ der Computerbauteile maximal um $5 \Omega$ vom Sollwert abweichen darf?**

  $a=\mu -c = 200\Omega - 5\Omega = 195\Omega$

   $b= \mu + c = 200 \Omega + 5\Omega = 205\Omega$

   $a'=\frac{a-\mu}{\delta}=\frac{195 \Omega - 200\Omega}{\sqrt{5}}=-\frac{5\Omega}{\sqrt{5}}$

   $b'=\frac{b-\mu}{\delta}=\frac{205 \Omega - 200\Omega}{\sqrt{5}}=\frac{5\Omega}{\sqrt{5}}$

   $\Rightarrow P(a'\leq z \leq b')=P(\frac{\mu-c-\mu}{\delta} \leq z \leq \frac{\mu + c- \mu }{\delta})$
   $=P(-\frac{c}{\delta} \leq z \leq \frac{c}{\delta })=P(-\frac{5}{\sqrt{5}} \leq z \leq \frac{5}{\sqrt{5}})$

   $P(-\frac{5}{\sqrt{5}} \leq z \leq \frac{5}{\sqrt{5}})=\Phi (\frac{5}{\sqrt(5)})-\Phi (-\frac{5}{\sqrt(5)})$

   $=\Phi (\frac{5}{\sqrt(5)})-(1- \Phi (\frac{5}{\sqrt(5)}))$

   $=\Phi (\sqrt{5}) - (1- \Phi (\sqrt{5}))$

   $=\Phi (\sqrt{5}) -1+ \Phi (\sqrt{5})) $

   $=(2*\Phi(\sqrt{5}))-1$

   $=0.975$

   $$P(\text{"Bauteil fehlerhaft"}) = 1 - 0.975 = 0.025$$

b) **Wie  müssen  die  Toleranzgrenzen $(200+/- \alpha) \Omega$ gewählt werden, damit die Wahrscheinlichkeit für  das Auftreten eines fehlerhaften Bauteils, d.h. $P(|R-200| > \alpha)$, kleiner als $0.01$ ist?**

$z$ ist zwischen $\frac{k-\mu}{\sigma}$
,da $k= \mu \pm \alpha $ fällt $\mu$ raus und es bleibt nur $\frac{\pm\alpha}{\sigma}$:

$P(\frac{-\alpha}{\sigma} \leq z \leq \frac{\alpha}{\sigma}) = 0.99$

$\Phi(\frac{\alpha}{\sigma}) - \Phi(\frac{-\alpha}{\sigma}) = 0.99$

... wieder umstellen ...

$\Phi(\frac{\alpha}{\sigma}) = \frac{1.99}{2}$

$\Phi(\frac{\alpha}{\sigma}) = 0.995$

aus Normalverteilungstabelle
$\rightarrow \frac{\alpha}{\sigma} = 2.58$
$\rightarrow \alpha = 5.77$

---
## Aufgabe 6.3
**In einem großen Netzwerk treten pro Tag im  Durchschnitt 16 Störungen auf. Man kann annehmen, dass die Anzahl der  Störungen *poissonverteilt* ist. Wie groß ist die Wahrscheinlichkeit, dass pro Tag mehr als 20 Störungen auftreten?**
*Poissonverteilung:*
$$P_\lambda(k) = \frac{ \lambda ^ k}{k!}e^{-\lambda}$$
$$F(n) =e^{-\lambda} \sum_{k=0}^{n} \frac{\lambda^{k}}{k!}$$

diskrete Werte:

$P_{16}(X > 20) = 1-F(20) = 1 - e^{-16} \sum_{k=0}^{20} \frac{16^{k}}{k!} \approx 0.131832$
hy
*Formel berechnet mit [Wolfram Alpha (Eingabe mit verlinkt)](http://www.wolframalpha.com/input/?i=1-e%5E%28-16%29+sum%2816%5Ek%2F%28k%21%29%29+k%3D0+to+20)*

---
## Aufgabe 6.4
**Eine Lieferung von 60 USB-Sticks, die 8 fehlerhafte  Sticks enthält, wird einer Qualitätskontrolle unterzogen.  Hierzu werden 5 der  60 Sticks herausgegriffen und überpruft. Die Lieferung wird zurückgeschickt, wenn unter den 5 geprüften Sticks einer fehlerhaft ist. Ermitteln Sie mithilfe der Hypergeometrischen Verteilung, mit welcher  Wahrscheinlichkeit die Lieferung zurückgeschickt wird.**
 * $N = 60 \text{ (Gesamtzahl)}$
 * $M = 5 \text{ (Auswahlmenge)}$
 * $m = 8 \text{ (fehlerhafte Anzahl unter N)}$
 * $x = 1 \text{ (gewahlte fehlerhafte Anzahl)}$

 *Hypergeometrische Verteilung:*
 $$P(X=x) = \frac
 {
   \begin{pmatrix} M\\x \end{pmatrix} *
   \begin{pmatrix} N-M\\n-x \end{pmatrix}
 }{
     \begin{pmatrix} N\\n \end{pmatrix}
 }$$


 $P(X=1) = \frac
 {
   \begin{pmatrix} 5\\1 \end{pmatrix} *
   \begin{pmatrix} 60-5\\8-1 \end{pmatrix}
 }{
     \begin{pmatrix} 60\\8 \end{pmatrix}
 }$
 $= 0.397$

---
## Aufgabe 6.5
**Ein Computernetz besteht aus 10 unabhängig voneinander arbeitenden Computern. Jeder dieser 10 Computer fällt in der Zeit T mit der Wahrscheinlichkeit $0.05$ aus. Mit  Hilfe der Ungleichung von Tschebyschew soll die Wahrscheinlichkeit dafür abgeschätzt werden, dass der absolute Betrag der Differenz zwischen der Zahl der  ausgefallenen Computer und dem Erwartungswert dieser Zufallsvariablen größer als 2 ist.**

*Ungleichung von Tschebyschew:*
$$P[|X - \mu| \geq k] \leq \frac{\sigma^2}{k^2}$$

Gesucht: Abschätzung von P für $|X - \mu| > 2$

Binomialverteilt, daher:

$\mu = n*p = 10 * 0.05 = 0.5$

Varianz:
$\sigma^2 = n*p*q = 10*0.05*0.95=0.475$

$P[|X - 0.5| \geq 2] \leq \frac{0.475}{2^2}$

$P[|X - 0.5| \geq 2] \leq \frac{0.475}{4}$

$P[|X - 0.5| \geq 2] \leq 0.11875$

DA aber größer als 2 sein soll sollte gelten:
(das ist nur eine Vermutung!)
$P[|X - 0.5| > 2] < 0.11875$
