# Blatt 01 (unkorrigiert)
## 1.1 12 Bauteile, davon 2 defekt. Mit welcher Wahrscheinlichkeit ist/sind unter 4 ausgewählten ...
Alle möglichen Kombinationen:
$$ \binom{12}{4} = 495$$

### a) kein defektes Bauteil:
$$ P(X) = \binom{8}{4} / \binom{12}{4} = \frac{70} {495} \approx 14,1 \% $$

### b) 1 defektes Bauteil:
$$ P(X) = \binom{8}{3} * \binom{4}{1} / \binom{12}{4} = \frac{56 * 6} {495} \approx 45,3 \% $$


### a) 2 defekte Bauteile:
$$ P(X) = \binom{8}{2} * \binom{4}{2} / \binom{12}{4} = \frac{28 * 6} {495} \approx 33,9 \% $$

## 1.2 Wie zuverlässig ist der Test?

|                   | Test ok   | Test fail |
| ----------------- |:---------:| ---------:|
| **normgerecht**   | 0,98      | 0,02      | 0,96
| **kaputt**        | 0,05      | 0,95      | 0,04

$$
P(X) = \frac{0,96 * 0,98}{0,96 * 0,98 + 0,04 * 0,05} \approx 99,79\%
$$

## 1.3 Mit welcher Wahrscheinlichkeit wird die Sendung zurückgeschickt?
100 Diskette, davon 10 defekt. Zum Test werden 5 gezogen. Wenn im Test n > 1 defekte -> Sendung wird zurückgeschickt.


Gegenereignis zu, "wenn 0 oder 1 Diskette defekt"
$$
P(X) = 1 - \frac{ \binom{90}{5} + \binom{90}{4} * \binom{10}{1}}{\binom{100}{5}} \approx 7,686 \%
$$

## 1.4
|            | Prog 1 | Prog 2 |
| ---------- |:------:| :------:|
| **Inf**    | 20     | 35     | *55*
| **CV**     | 40     | 5      | *45*
|            | *60*   | *40*   |

### a) X: Prog 1 unter den CVlern
$$ P(X) = 40 / 45 = 88,9 \%$$

### b) X: Prog 1 unter den Inf
$$ P(X) = 20 / 55 = 36,4 \%$$

### a) X: Inf unter den Prog2-Usern
$$ P(X) = 35 / 40 = 87,5 \%$$

## 1.5 Mit welcher Wahrscheinlichkeit wird die Serie nicht ausgeliefert?
100 Drucker, davon 5 defekt. Zum Test werden 5 gezogen. Wenn im Test n > 0 defekte -> Sendung wird nicht ausgeliefert.


Gegenereignis zu, "wenn 0 alle heil"
$$
P(X) = 1 - \frac{ \binom{95}{5}}{\binom{100}{5}} \approx 23,04 \%
$$
