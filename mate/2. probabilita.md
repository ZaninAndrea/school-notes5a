# Probabilità
La probabilità tratta **eventi aleatori**, due casi particolari sono gli eventi certi e gli eventi impossibili
$$
0 \le p(E) \le 1
$$
<!-- toc -->

## Probabilità classica (o a priori)
Quando a priori conosco tutta la gamma di eventi possibili. E.g. il lancio di un dado. 
$$
p(E) = \frac{\text{n° casi favorevoli}}{\text{n° casi possibili}}
$$
La probabilità dell'evento complementare è definita così:
$$
p(\overline{E}) = 1- p(E)
$$

### Con 2 eventi
$$
p(E_1 \cup E_2)= p(E_1) + p(E_2) - p (E_1 \cap E_2)
$$
Quando $$p(E_1 \cap E_2)=0$$ i 2 eventi sono incompatibili, altrimenti sono compatibili. 
$$
p(E_1 \cap E_2)= p(E_1) \cdot p(E_2)
$$


### Evento condizionato
Quando un evento precedente condiziona le probabilità di un evento successivo.
> Da una giara con 5 palline rosse, 2 nere e 3 blu estraggo 2 palline una dopo l'altra senza reinserirle nella giara, quali sono le probabilità di pescare uuna pallina blu e poi una rossa?
> $$
\begin{align*}
p(BR) &= p(\text{B 1° estr}) \cdot p(\text{R 2° estr | è uscito blu al 1°}) \\
&= \frac{3}{10} \cdot \frac{5}{9}
\end{align*}
$$

### Bayes
$$
p(A)\cdot p(B|A)=p(B)\cdot p(A|B)
$$