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

### Derivata di $f(x)^{g(x)}$
E.g.
$$
\begin{aligned}
y&=(x+2)^{(x-1)}
\end{aligned}
$$

Formula
$$
\begin{aligned}
y&=f(x)^{g(x)}\\
&=e^{\ln{f(x)^{g(x)}}}\\
&=e^{g(x)\cdot\ln{f(x)}}\\
y'&=e^{g(x)\cdot\ln{f(x)}}\cdot(g'(x)\ln{f(x)}+\frac{g(x)}{f(x)}f'(x))\\
&=f(x)^{g(x)}\cdot(g'(x)\ln{f(x)}+\frac{g(x)}{f(x)}f'(x))
\end{aligned}
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

### Derivata composta !!
$$
(f(g(x)))'= f'(g(x))g'(x)
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

#### Cuspidi
$$
\begin{aligned}
f'_+(x)&=+\infty\\
f'_-(x)&=-\infty\\
&\lor\\
f'_+(x)&=-\infty\\
f'_-(x)&=+\infty\\
\end{aligned}
$$

#### Flessi a tangente verticale
![flessovert](./images/flessoverticale.png)
$$
\begin{aligned}
f'_+(x)=f'_-&(x)=-\infty\\
&\lor\\
f'_+(x)=f'_-&(x)=+\infty\\

\end{aligned}
$$

## Derivata seconda
Data una funzione $f(x)$ definita e continua in un intervallo e derivabile 2 volte nell'intervallo, se $f''(x)\gt0$ la funzione avrà concavità verso l'alto, se $f''(x)\lt0$ la funzione avrà concavità verso il basso.

## Derivata dell'inversa
$$
\begin{aligned}
f(x)&=y \\
f^{-1}(y)&=x \\
Df^{-1}(y)&=Df^{-1}(f(x))\\
&=Df^{-1}(f(x))\cdot Df(x)\\
\\
Df^{-1}(y)&=\frac{1}{Df(x)}
\end{aligned}
$$

### Derivata di $\arcsin{y}$
$$
\begin{aligned}
D\arcsin{y}&=\frac{1}{D\sin{x}}\\
&=\frac{1}{\cos{x}} \\
&=\frac{1}{\sqrt{1-\sin^2{x}}}\\
&=\frac{1}{\sqrt{1-y^2}}
\end{aligned}
$$

### Derivata di $\arccos{y}$
$$
D\arccos{y}=\frac{-1}{\sqrt{1-y^2}}
$$

### Derivata di $\arctg{y}$
$$
D\arctg{y}=\frac{1}{1+y^2}
$$

## Applicazioni delle derivate
### Determinare quando 2 curve sono tangenti tra loro
Determiniamo per quale $k$ le 2 curve
$$
\begin{aligned}
y&=2x^2 + k \\
y &=\ln{x}
\end{aligned}
$$

Sono tangenti tra loro e in quale punto. Sappiamo quindi che te 2 curve devono toccarsi in un solo punto e che in quel punto la tangente deve essere comune.

$$
\begin{cases}
2x^2 + k = \ln{x} \\ 
4x = \frac{1}{x} 
\end{cases}
$$

### Determinare la retta tangente and entrambe le curve
$$
\begin{aligned}
f : y &= x^2 \\
g : y &= \frac{1}{x}
\end{aligned}
$$
![tangente comune.PNG](images/tangente-comune.png)

La tangente toccherà le 2 rette in 2 punti $(x_p, y_p)$ e $(x_q,y_q)$. 
La tangente a $f$ in $P(x_p, y_p)$ è
$$
\begin{aligned}
y-y_p&=f'(x_p)\cdot(x-x_p)\\
y&=2x_p x - 2x_p^2+x_p^2\\
y&=2x_p x - x_p^2
\end{aligned}
$$
e quella a $g$ in $P(x_q,y_q)$ è
$$
\begin{aligned}
y-y_q&=f'(x_q)\cdot(x-x_q)\\
y&=-\frac{1}{x^2_q}x+\frac{1}{x_q}+\frac{1}{x_q}\\
y&=-\frac{1}{x^2_q}x+\frac{2}{x_q}
\end{aligned}
$$

La tangente deve essere comune, quindi sia la $m$ che la $q$ devono essere uguali

$$
\begin{cases}
2x_p&=-\frac{1}{x^2_q}\\
-x_p^2&=\frac{2}{x_q}
\end{cases}
$$

### Applicazione in fisica - legge oraria del moto
Una palla viene lanciata da terra ad una velocità di $60 \frac{m}{s}$ la legge oraria con cui si muove questa palla $s=60t-5t^2$.
Trova l'altezza massima.

$$
v = s' = 60 - 10t
$$

L'altezza massima è il punto in cui la velocità è 0

$$
\begin{aligned}
v &= 0\\
60 - 10t = 0\\
t = 6
\end{aligned}
$$

Da cui troviamo che $s = 180$

## Teorema di de l'Hospital
f,g definite su I, derivabili in $I/\{x_0\}$ con $g'(x)\ne0$
- se $\lim_{x\to x_o}f(x)=\lim_{x\to x_o}g(x)=0$
- oppure se $\lim_{x\to x_o}f(x)=\lim_{x\to x_o}g(x)=\infty$

allora  
$$
\exists \lim_{x\to x_0}\frac{f'(x)}{g'(x)}
\Rightarrow
\lim_{x\to x_0}\frac{f(x)}{g(x)}=\lim_{x\to x_0}\frac{f'(x)}{g'(x)}
$$

**Esempio**
$$
\lim_{x\to 1}\frac{\ln{x}}{3x-3}=\lim_{x\to 1}\frac{\frac{1}{x}}{3}=\frac{1}{3}
$$

### Problemi di ottimizzazione
> Tra tutti i rettangoli inscritti in una circonferenza di raggio $r$ determina quello di perimetro massimo

## Massimo assoluto
$x_0$ è un punto di massimo assoluto se $f(x)\le f(x_0) \forall x \in D$