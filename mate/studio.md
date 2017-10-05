[[toc]]
# Studio di funzione
## Continuità di una funzione
Una funzione $f(x)$ definita in $I(x_0)$ si dice continua in $x_0$ se 
$$
\lim_{x\to x_0}f(x)=f(x_0)
$$
altrimenti è discontinua.

### 1° specie di punti di discontinuità
$$
\begin{aligned}
\lim_{x\to x_0^+}f(x)&=l_1 \\
\lim_{x\to x_0^-}f(x)&=l_2 \\
l_1 &\ne l_2
\end{aligned}
$$

Il salto in $x_0$ è definito come $|l_2-l_1|$

### 2° specie di punti di discontinuità
Almeno uno dei 2 limiti è infinito o non esiste.

### 3° specie di punti di discontinuità (o discontinuità eliminabile)
$$
\exists \lim_{x\to x_0}f(x)=l \quad \land \quad (\; f(x_0)\ne l \; \lor \; \nexists f(x_0)\;)
$$

### Teorema della funzione inversa
Se una funzione $f$ è biettiva e continua nel suo dominio, allora anche la sua inversa sarà continua.

### Teorema di Veierstrass
Data una funzione continua in un intervallo chiuso $[a,b]$ allora essa assume in quell'intervallo un massimo assoluto e un minimo assoluto in tale intervallo.

### Teorema dei valori medi
Data una funzione continua in un intervallo chiuso $[a,b]$ essa assume almeno una volta tutti i valori compresi tra il massimo e il minimo assoluto.

### Teorema di esistenza degli zeri
Data una funzione continua in un intervallo chiuso [a,b] e $f(a)$ e $f(b)$ hanno segno opposto $\Rightarrow \exists c \in (a,b) \mid f(c)=0$

**E.g.**
Stabilisci se $y=x^5+2x+4$ ha zeri nell'intervallo $[0,2]$.
$f(0)=4$ e $f(2)=40$, quindi non possiamo affermarlo con certezza.

Provo con l'intervallo $[-2,-1]$
$f(-1)=1$ e $f(-2)=-32$, quindi in questo interallo è presente uno zero.