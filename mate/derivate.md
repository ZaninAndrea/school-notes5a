# Derivate
Definisco come rapporto incrementale di una funzione
$$
\begin{aligned}
\frac{\Delta y}{\Delta x}&=\frac{f(x_0+h)-f(x_0)}{x_0+h-x_0}\\
&=\frac{f(x_0+h)-f(x_0)}{h}\\
\end{aligned}
$$

La definizione di derivata è
$$
f'(x_0)=\lim_{h\to0}\frac{f(x_0+h)-f(x_0)}{h}
$$

La funzione si dice derivabile in $x_0$ se esiste $f'(x_0)$ ed esso è finito.

## Teorema derivabilità e continuità
Se una funzione è derivabile in $x_0$ allora è continua in $x_0$.

## Trovare la tangente in un punto
La retta tangente ad $f$  in un punto $x_0$ è
$$
y-f(x_0)=f'(x_0) \cdot (x-x_0)
$$

## Derivate fondamentali
### Derivata di $x^n$
Esempio con $x^3$

$$
\begin{aligned}
&\lim_{h\to 0}\frac{f(x+h)-f(x)}{h}=\\
&\lim_{h\to 0}\frac{(x+h)^3-f(x)^3}{h}=\\
&\lim_{h\to 0}\frac{x^3+3x^2h+3xh^2+h^3-x^3}{h}=\\
&\lim_{h\to 0}3x^2+3xh+h^2&=3x^2\\
\end{aligned}
$$

Formula generale
$$
(x^n)'=nx^{n-1}\qquad \text{con }n\ne 0
$$

### Derivata di $\sin{(x)}$
$$
\begin{aligned}
&\lim_{h\to0}\frac{\sin{(x+h)}-\sin{(x)}}{h}\\
&\lim_{h\to0}\frac{\sin{(x)\cos{(h)}}+\sin{(h)}\cos{(x)}-\sin{(x)}}{h}\\
&\lim_{h\to0}\frac{\sin{(x)(\cos{(h)}-1})}{h} \cdot \frac{\sin{(h)}\cos{(x)}}{h}&=\cos{x}
\end{aligned}
$$

Formula generale
$$
\sin{x}=\cos{x}
$$

### Derivata di $\cos{x}$
$$
(\cos{x})'=-\sin{h}
$$

### Derivata di $a^x$
$$
\begin{aligned}
&\lim_{x\to0}\frac{a^{x+h}-a^x}{h}=\\
&\lim_{x\to0}\frac{a^{x}(a^h-1)}{h}=\\
&\lim_{x\to0}\frac{a^x(e^{\ln{a^h}}-1)}{h}\\
&\lim_{x\to0}\frac{a^x(e^{\ln{a^h}}-1)\ln{a}}{h\ln{a}}&=a^x\ln{a}
\end{aligned}
$$

Caso generale
$$
(a^x)'=a^x\ln{a}
$$

Caso particolare
$$
(e^x)'=e^x
$$

### Derivata di $log_a x$
Forma generale
$$
(\log_a x)'=\frac{1}{\ln{(a)}\cdot x}
$$

Caso specifico
$$
(\ln{x})'=\frac{1}{x}
$$

## Derivate composte
### Somma di funzioni
$$
(f(x)+g(x))'=f'(x)+g'(x)
$$

### Prodotto per uno scalare
$$
(kf(x))'=kf'(x)
$$

### Prodotto di funzioni
Dimostrazione
$$
\begin{aligned}
&\lim_{h\to0}\frac{f(x+h\cdot g(x+h)-f(x\cdot g(x)))}{h}=\\
&\lim_{h\to0}\frac{f(x+h\cdot g(x+h)-g(x+h)\cdot f(x)+g(x+h)\cdot f(x)-f(x\cdot g(x)))}{h}=\\
&\lim_{h\to0}g(x+h)\frac{f(x_h)-f(x)}{h} + f(x)\frac{g(x+h)-g(x)}{h}=\\
&= f'(x)\cdot g(x) + f(x)g'(x)
\end{aligned}
$$

Formula generale

$$
(f(x)\cdot g(x))'=f'(x)\cdot g(x) + f(x)g'(x)
$$

### Funzione elevata a potenza
$$
(f^n(x))'=nf^{n-1}(x)f'(x)
$$

### Rapporto di funzioni
$$
(\frac{f(x)}{g(x)})'=\frac{f'(x)\cdot g(x) - f(x)g'(x)}{g^2(x)}
$$

## Punti stazionari
Informazioni che otteniamo dalla derivata
- $f'(x)\gt0$ la funzione è crescente
- $f'(x)\lt0$ la funzione è decrescente
- $f'(x)=0$ punto stazionario

### Classificazione dei punti stazionari
#### Minimi e massimi locali
![minimo.PNG](images/minimo.png)

#### Flesso a tangente orizzontale
![flesso.PNG](images/flesso.png)

## Punti di non derivabilità
### Punti angolosi
$$
\begin{aligned}
f'_+(x)&=l_1\\
f'_-(x)&=l_2\\
l_1&\ne l_2
\end{aligned}
$$

![angoloso.PNG](images/angoloso.png)

### Cuspidi
$$
\begin{aligned}
f'_+(x)&=+\infty\\
f'_-(x)&=-\infty\\
&\lor\\
f'_+(x)&=-\infty\\
f'_-(x)&=+\infty\\
\end{aligned}
$$

### Flessi a tangente verticale

$$
\begin{aligned}
f'_+(x)=f'_-&(x)=-\infty\\
&\lor\\
f'_+(x)=f'_-&(x)=+\infty\\

\end{aligned}
$$