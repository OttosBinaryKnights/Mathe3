# Blatt 01
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
