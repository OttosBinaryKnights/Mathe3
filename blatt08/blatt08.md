# Übung 8
## Aufgabe 8.1
**Gegeben sei die Funktion $f:\mathbb{R} \rightarrow \mathbb{R}$ mit $f(x)=x^4-3cos (\frac{\pi}{2}x)-2x+4$ auf dem Intervall [−1,1].**

 a) **Zeigen Sie, dass $P_2(x)=1-2x+4x^2$ das quadratische Interpolationspolynom von f an den Stützstellen $x_i=i-1$ mit $i=0,1,2$ ist.**

 $x_0 = -1$

 $P_2(x_0)=1+2+4 = 7$

 $f(x_0)=1-0+2+4 =7$

---

 $x_1 = 0$

 $P_2(x_1)=1$

 $f(x_1)=-3+4 =1$

 ---

 $x_2 = 1$

 $P_2(x_2) = 1-2+4 = 3$

 $f(x_2) = 1-0-2+4 =3$

(wichtig als Begründung zu schreiben, sonst keine Punkte in Klausur:)
 Einsetzen reicht, da es nur ein mögliches Interpolationspolynoms für diese drei Stützpunkte geben kann.

 b) **Berechnen Sie $f(0.5)$ näherungsweise mithilfe des Interpolationspolynoms $P_2(x)$.**

 $P_2(0.5)=1-1+1 = 1$

 c) **Bestimmen Sie fünf Stützstellen $a_i,b_i, 0 \leq i \leq 4$, mit $a_i \in [-1,1]$,so dass $P_2(x)$ das Interpolationspolynom bzgl. diesen Stellen ist.**

 Punkte sollen nur auf Polynom liegen, vier schon gegeben, eine fehlt noch:

 $P_2(-0.5) = 1+1+1=3$

 $\{(-1,7),(-0.5,1),(0,1),(0.5,1),(1,3)\}$

---
## Aufgabe 8.2
**Gegeben sei die Funktion $f:\mathbb{R}_{\geq -4} \rightarrow \mathbb{R}$ mit $f(x)=\sqrt{x+4}$ an den Stützstellen $x_0=-3,x_1=0$ und $x_2=5$. Bestimmen Sie den Wert des Interpolationspolynoms $p(x^* )=0,41$**

 a) **nach der Methode von Lagrange**

 $f(x)=\sqrt{x+4}$

 $x_0=-3 \Rightarrow f(x_0)=1$

 $x_1=0 \Rightarrow f(x_1)=2$

 $x_2=5 \Rightarrow f(x_2)=3$

 $p(x)=\sum_{i=0}^n f(x_i)*L_i(x)$

 $L_i(x)= \prod_{\begin{matrix}j=0 \\ j \neq i \end{matrix}}^n \frac{x-x_j}{x_i - x_j}$ *("Gewichtungsfunktion"?)*

 $p(x)= f(x_0)*(\frac{x-x_1}{x_0-x_1})* (\frac{x-x_2}{x_0-x_2})$
 $+ f(x_1)* (\frac{x-x_0}{x_1-x_0})* (\frac{x-x_2}{x_1-x_2})$
 $+ f(x_2)* (\frac{x-x_0}{x_2-x_0})* (\frac{x-x_1}{x_2-x_1})$

 $= f(-3)*(\frac{x-0}{-3-0})* (\frac{x-5}{-3-5})$
 $+ f(0)* (\frac{x-(-3)}{0-(-3)})* (\frac{x-5}{0-5})$
 $+ f(5)* (\frac{x-(-3)}{5-(-3)})* (\frac{x-0}{5-0})$

 $= 1*(\frac{x}{-3})* (\frac{x-5}{-8})$
 $+ 2* (\frac{x+3}{3})* (\frac{x-5}{-5})$
 $+ 3* (\frac{x+3}{8})* (\frac{x-0}{5})$

$p_L(0.41) =(0.41/-3) * ((0.41-5)/-8) + 2 * ...$

 $p_L(0.41) = 2.264$ (angeblich)

 b) **nach der Methode von Newton**

allgemein:
 $$p(x)= \sum_{i=0}^n a_i * \prod_{j=0}^{i-1} (x-x_j)$$

Interpolationspolynom in diesem Fall:
 $$p_N(x)=a_0+a_1(x-x_0)+a_2(x-x_0)(x-x_1)$$


 | $a_0$ | $f(x_0)=1$ | $f(x_1)=2$ | $f(x_2)=3$ |
 | ----- | ---------- | ---------- | ---------- |
 | $a_1$ | $f(x_0,x_1)=\frac{2-1}{0-(-3)}=\frac13$ | $f(x_1,x_2)=\frac{3-2}{0-5}=-\frac15$ |   |
 | $a_2$ | $f(x_0,x_1,x_2)=\frac{-\frac15 - \frac13}{5-1} = \frac{-\frac{8}{15}}{4}=-\frac{2}{15}$ |   |   |

 $\Rightarrow p(x)=3+(-\frac15)(x-(-3))+(-\frac{2}{15})(x-(-3))(x-0)$

 $=3-\frac35 x -\frac{2}{15}* (x+3)x$

 $=3-\frac35 x -\frac{2}{15} x^2-\frac{6}{15}$

 $=\frac{13}{5}-\frac35 x -\frac{2}{15}x^2$

 $p(o.41)=2.332$

 $a_i=a_{i,i}$

 $\alpha = \begin{matrix}
y_i & j=0 \\
\frac{\alpha_{i,j-1}-\alpha_{i-1,j-1}}{x_i-x_{i-j}} & 1\leq j \leq i
 \end{matrix}$

Lösung:
nach dem Newton Schema (im Dreieck:)

 $\begin{matrix}
 a_0=1 \\
 a_1=\frac13 \\
 a_2=-\frac{1}{60}
 \end{matrix}$

 $P_n(x) = 1+ \frac{1}{3}(x+3)+(-\frac{1}{60})(x+3)x$
 $= \frac{-x^2}{60}+\frac{3x}{60}+\frac{x}{3}+2$

 c) **mit dem Neville-Algorithmus.**

 $\begin{matrix}
 P_0(x)=f(-3)=1 \\
 P_1(x)=f(0)=2 \\
 P_2(x)=f(5)=3
 \end{matrix}$

 $P_{01}(x)=\frac{(x-x_0)P_1(x)-(x-x_1)P_0(x)}{(x_1-x_0)}$

 $=\frac{(x+3)* 2-(x-0)* 1}{0+3}=\frac{2x+6-x}{3}=\frac{x+6}{3}$

 $P_{12}(x)=\frac{(x-x_1)P_2(x)-(x-x_2)P_1(x)}{(x_2-x_1)}$

 $=\frac{(x-0)* 3-(x-5)* 2}{5-0}=\frac{3x-2x+10}{5}=\frac{x+10}{5}$

 $P_{012}(x)=\frac{(x-x_0)P_{12}(x)-(x-x_2)P_{01}(x)}{(x_2-x_0)}$

 $=\frac{(x+3)* \frac{x+10}{5}-(x-5)* \frac{x+6}{3}}{5+3}=\frac{3x-2x+10}{5}=\frac{x+10}{5}$

 $P_{012}(0.41)=2.113$

---
## Aufgabe 8.3
**Zeigen Sie, dass sich, numerisch günstig auswertbar, das Interpolationspolynom $p(x)$ in Lagranscher Form auch darstellen lässt durch**

$$p(x)=\begin{cases}
y_i &
     x=x_i;i=0,...,n \\
\frac{\sum \limits_{i=0}^n
    \frac{c_i}{x-x_i}y_i}
  {\sum \limits_{i=0}^n
    \frac{c_i}{x-x_i}} &
      x \neq x_i; i=0,...,n
\end{cases}$$

**wobei $\frac 1c_i=\prod \limits_{\begin{matrix} k=0 \\ k \neq i \end{matrix}}^n (x_i-x_k)$ gilt.**

---
## Aufgabe 8.4
**Gegeben sei die Funktion $f:\mathbb{R}_{\leq 6} \rightarrow \mathbb{R}$ mit $f(x)=\sqrt{6-x}$.**

 a) **Bestimmen Sie das Interpolationspolynom $P_2(x)$ an den Stützstellen $(-3,f(-3)),(5,f(5))$ und $(6,f(6))$.**

 Lösung über Newton:

 $\begin{matrix}
 -3 & 3 \\
 5 & 1 & \frac{1-3}{5-(-3)}=-1/4\\
 6 & 0 & \frac{0-1}{6-(-3)}=-1/9 & \frac{-1/9-1/4}{9}=-\frac{13}{81}\\
 \end{matrix}$

 $P(x)= 3 - \frac13 (x+3) - \frac{13}{81} (x+3) x$
 $=3 - \frac13 x - 1 - \frac{13}{81} x^2 -\frac{13}{27}x$

 * $a_0 = 7/ 2 $
 * $a_1 = - 1/ 12 $
 * $a_2 = - 1/ 12 $

irgendwo verrechnet, rauskommen sollte wohl:

 $P_2(x) = \frac72 - \frac{1}{12}x - \frac{1}{12}x^2$

 b) **Benutzen Sie das Interpolationspolynom $P_2(x)$, um $\sqrt{2}$ näherungsweise zu berechnen.**

 $f(4) \approx P(\sqrt{4})$
 $= \frac{7}{2} - \frac{4}{12} -\frac{16}{12}$
 $= \frac{11}{6}$

 c) **Geben Sie einen Näherungswert für $\int_{-2}^4 f(x)dx$ mithilfe des Interpolationspolynoms $P_2(x)$ an.**

 $\int_{-2}^4 f(x)dx \approx \int_{-2}^4 P_2 (x) dx$
 $= \int_{-2}^4 (\frac72 - \frac{1}{12}x - \frac{1}{12}x^2)$
  $= [\frac72 x - \frac{x^2}{24} - \frac{x^3}{36}]_{-2}^4$
  $= "\frac{37}{2}"$

---
## Aufgabe 8.5
**Gegeben sei die Funktion $f:D \rightarrow [-1,1]$ mit $f (x) = sin \frac{\pi}{4}x$.**

 a) **Bestimmen Sie eine Näherung für das bestimmte Integral $I=\int_0^{\frac{\pi}{2}}sin\frac{\pi}{4}x dx$, indem Sie das Interpolationspolynom $P_2(x)$ an den Stützstellen $x_0 = 0,x_1 = 1$ und $x_2 = 2$ der Funktion $f(x)$ benutzen.**

 $\begin{matrix}
 0 & 0 \\
 1 & \frac{\sqrt{2}}{2} & \frac{1-3}{5-(-3)}=-1/4\\
 2 & 1
 \end{matrix}$

 b) **Bestimmen Sie eine weitere Näherung für das Integral I, indem Sie als Näherung für $f(x)$ das Taylorpolynom an der Stelle $x^*= 1$ benutzen.**

 c) **Vergleichen Sie die unter a) und b) erhaltenen Näherungswerte mit einem Wert aus dem Taschenrechner.**

 Integral-Taschenrechner:
 $I=\int_0^{\frac{\pi}{2}}sin\frac{\pi}{4}x dx = 0.8521$
