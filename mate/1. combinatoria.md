# Calcolo Combinatorio### 
<!-- toc -->
## Fattoriali
Sono indicati con il simbolo ! dopo il numero
$$
n!=
\begin{cases}
	n=0 & n! = 1 \\
	n\ge1 & n!=n \cdot (n-1)!\\
\end{cases}
$$
#### Proprietà
$$
k!=k\cdot(k-1)!
$$
## Coefficiente binomiale
#### Definizione
$$
\binom{n}{k} = \frac{n!}{k!(n-k)!}
$$
#### Casi particolari
$$
\binom{n}{n} = 1 \qquad \binom{n}{0}=1 \qquad \binom{0}{0}=1\qquad
\binom{n}{k}=\binom{n}{n-k}
$$

### Formula binomiale di Newton
$$
(A+B)^n = \sum_{k=0}^{n}{\binom{n}{k}A^{n-k}B^{k}}
$$
e.g.
$$
(x-1)^3=\binom{3}{0}x^3(-1)^0 + \binom{3}{1}x^2(-1)^1 +\binom{3}{2}x^1(-1)^2+\binom{3}{3}x^0(-1)^3
$$

### Esericizi
$$
\begin{align*}
1.& &\frac{\binom{10}{7}+\binom{9}{0}+\binom{9}{1}}{\binom{0}{0}}& &[130] \\
2.& &\binom{10}{k}=\binom{10}{k-2}& &[k=6]
\end{align*}
$$

## Combinatoria
### Permutations without repetition
permutations is the rearrangement of objects or symbols in an ordered list without repetitions, perhaps missing some elements. Each unique ordering is called a permutation.
$$
P_{n,r}=\frac{n!}{(n-r)!}
$$
**n** is the size of the sequence **from** which the objects are permuted
**r** is the size of the size of the sequence **in** which the objects are permuted.
> **Italiano**  
> quando n e k sono uguali vengono chiamati permutazioni, altrimenti le chiamiamo disposizioni

Sulla calcolatrice si calcola con la funzione nPr
#### With undistinguishable objects
If some of the objects are undistinguishable the number of permutations of all of them is
$$
P_{n,r_1,r_2,r_3}=\frac{n!}{r_1!\;r_2!\;r_3!}
$$
### Permutation with repetition
The formula to compure the number of permutation with repetition is
$$
n^r
$$
### Combinations without repetitions
Selections where the order doesn't matter and the objects can only be chosen once
$$
C_{n,r}=\frac{n!}{(n-r)!r!}=\binom{n}{r}
$$

### Combinations with repetition
$$
C^R_{n,r}=C_{n+r-1,r}=\binom{n+r-1}{r}=\binom{n+r-1}{n-1}
$$
