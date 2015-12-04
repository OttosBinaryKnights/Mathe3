# Übung 8
## Aufgabe 8.1
**Gegeben sei die Funktion $f:\mathbb{R} \rightarrow \mathbb{R}$ mit $f(x)=x^4-3cos (\frac{\pi}{2}x)-2x+4$ auf dem Intervall [−1,1].**

 a) **Zeigen Sie, dass $P_2(x)=1-2x+4x^2$ das quadratische Interpolationspolynom von f an den Stützstellen $x_i=i-1$ mit $i=0,1,2$ ist.**

 b) **Berechnen Sie $f(0,5)$ näherungsweise mithilfe des Interpolationspolynoms $P_2(x)$.**

 c) **Bestimmen Sie fünf Stützstellen $a_i,b_i, 0 \leq i \leq 4$, mit $a_i \in [-1,1]$,so dass $P_2(x)$ das Interpolationspolynom bzgl. diesen Stellen ist.**

---
## Aufgabe 8.2
**Gegeben dei die Funktion $f:\mathbb{R}_{\leq -4} \rightarrow \mathbb{R}$ mit $f(x)=\sqrt{x+4}$ an den Stützstellen $x_0=-3,x_1=0$ und $x_2=5$. Bestimmen Sie den Wert des Interpolationspolynoms $p(x^* )=0,41$**

 a) **nach der Methode von Lagrange**

 b) **nach der Methode von Newton**

 c) **mit dem Neville-Algorithmus.**

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

 a) **Bestimmen Sie das Interpolationspolynom $P_2(x)$ an den Stützstellen $(3,f(-3)),(5,f(5))$ und $(6,f(6))$.**

 b) **Benutzen Sie das Interpolationspolynom $P_2(x)$, um $\sqrt{2}$ näherungsweise zu berechnen.**

 c) **Geben Sie einen Näherungswert für $\int_{-2}^4 f(x)dx$ mithilfe des Interpolationspolynoms $P_2(x)$ an.**

---
## Aufgabe 8.5
**Gegeben sei die Funktion $f:D \rightarrow [-1,1]$ mit $f (x) = sin \frac{\pi}{4}x$.**

 a) **Bestimmen Sie eine Näherung für das bestimmte Integral $I=\int_0^{\frac{\pi}{2}}sin\frac{\pi}{4}x dx$, indem Sie das Interpolationspolynom $P_2(x)$ an den Stützstellen $x_0 = 0,x_1 = 1$ und $x_2 = 2$ der Funktion $f(x)$ benutzen.**

 b) **Bestimmen Sie eine weitere Näherung für das Integral I, indem Sie als Näherung für $f(x)$ das Taylorpolynom an der Stelle $x^*= 1$ benutzen.**

 c) **Vergleichen Sie die unter a) und b) erhaltenen Näherungswerte mit einem Wert aus dem Taschenrechner.**
