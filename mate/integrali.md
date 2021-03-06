---
category: "Matematica"
title: "Integrali"
index: 6
draft: false
---

# $\int$ntegrali
## Integrali indefiniti
$F(x)$ è primitiva di $f(x)$ in un intervallo $I$ se $F(x)$ è derivabile e $F'(x)=f(x)$

L'integrale indefinito di una funzione $f(x)$ è l'insieme di tutte le sue primitive e si indica in questo modo

$$
\int f(x)\; dx = F(x)+c
$$

$dx$ indica in quale variabile fare l'integrale

### Proprietà dell'integrale
#### Somma
$$
\int[f(x)+g(x)] \; dx = \int f(x)\; dx + \int g(x) \; dx
$$

#### Prodotto per uno scalare
$$
\int k f(x) \; dx = k \int f(x) \; dx
$$

### Calcolo di integrali
#### Polinomio
Se $n\ne-1$
$$
\int x^n \; dx = \frac{x^{n+1}}{n+1} + c
$$

Se $n=1$

$$
\int \frac{1}{x} \;dx = \ln{\mid x \mid} + c
$$

#### Esponenziale
$$
\int e^x \; dx = e^x + c
$$

#### Funzioni goniometriche
$$
\begin{aligned}
\int \sin{x} \; dx &= - \cos{x} + c \\
\int \cos{x} \; dx &= \sin{x} +c \\
\int \frac{1}{\cos^2{x}} \; dx &= \tg{x} +c \\
\int \frac{1}{1+x^2}\; dx &= \arctg{x} + c \\
\end{aligned}
$$

#### Integrali di funzioni razionali fratte
$$
\int \frac{N(x)}{D(x)} dx
$$

**Se $N(x)$ ha grado maggiore di D(x) si fa la divisione**

Esempio
$$
\int \frac{x^3+2x^2+x+1}{x^2+1} dx
$$

$$
\begin{aligned}
&+x^3 &+2x^2 &+x &+1\div x^2+1=x+2-\frac{1}{x^2+1}\\
&-x^3 & &-x \\

\end{aligned}
$$

**Se il grado di N(x) è minore di D(x)**
**Denominatore di grado 1**

$$
\int \frac{1}{ax+b} dx
$$

Uso il logaritmo

Esempio
$$
\begin{aligned}
&\int \frac{1}{2x+3}dx \\
&\frac{1}{2} \int \frac{2}{2x+3} dx \\
&\frac{1}{2} \ln{\mid 2x+3 \mid} + c
\end{aligned}
$$

**Grado 2 con $\Delta \gt 0$**
Cerco di scomporlo in 2 frazioni con denominatore di grado 1

$$
\int \frac{px+q}{(x-x_1)(x-x_2)}dx=\int\frac{A}{x-x_1}dx+\int \frac{B}{x-x_2}dx
$$

**Grado 2 con $\Delta=0$**

$$
\int \frac{px+q}{ax^2+bx+c}dx=\int\frac{A}{a(x-x_1)}+\frac{B}{(x-x_2)^2}dx
$$

Alternativamente posso "aggiustare" il numeratore in modo che sia la derivata del denominatore

**Grado 2 con $\Delta \lt 0$**
Esempio 1

$$
\begin{aligned}
&\int \frac{1}{x^2+x+1}dx=\\
&\int \frac{1}{(x^2+x+\frac{1}{4})+\frac{3}{4}} dx=\\
&\int\frac{1}{\frac{3}{4}\big[\frac{4}{3}(x+\frac{1}{2})^2+1\big]}dx=\\
\frac{4}{3}&\int\frac{1}{\big[\frac{2}{\sqrt{3}}(x+\frac{1}{2}) \big]^2+1}dx=\\
\frac{4}{3}\frac{\sqrt{3}}{2}&\int\frac{\frac{2}{\sqrt{3}}}{\big[\frac{2}{\sqrt{3}}(x+\frac{1}{2}) \big]^2+1}dx=\\
&\frac{4}{3}\frac{\sqrt{3}}{2}\arctg{(\frac{2}{\sqrt{3}}(x+\frac{1}{2}))}+c
\end{aligned}
$$

**Grado 2 con $\Delta \lt 0$ e numeratore di grado 1**
$$
\begin{aligned}
&\int\frac{2x+1}{x^2+4x+5}dx\\
&\int\frac{2x+4}{x^2+4x+5}dx-\int\frac{3}{x^2+4x+5}dx\\
&\ln{(x^2+4x+5)}-\int\frac{3}{x^2+4x+5}dx
\end{aligned}
$$

#### Sostituzioni particolari
**Caso 1**

$$
\int\frac{1}{\sqrt{x^2 \pm a^2}}\:dx
$$

oppure

$$
\int \sqrt{x^2 \pm a^2}\: dx
$$

Si usa la sostituzione
$$
t=x+\sqrt{x^2\pm a^2}
$$

**Caso 2**
$$
\int\sqrt{9-x^2}dx
$$

Uso la sostituzione
$$
\begin{aligned}
x&=3\sin{t}\\
dx&=3\cos{t}
\end{aligned}
$$

**Parametriche**
In alcuni casi è utile sostituire utilizzando le parametriche
$$
\begin{aligned}
\sin{x}&=\frac{2\tg{\frac{x}{2}}}{1+\tg^2{\frac{x}{2}}}\\
\cos{x}&=\frac{1-\tg^2{\frac{x}{2}}}{1+\tg^2{\frac{x}{2}}}
\end{aligned}
$$

Usando poi la sostituzione
$$
t=\tg{\frac{x}{2}}
$$


**Caso strano**
$$
\int \Big(\frac{1}{1+x^2}\Big)^2\: dx
$$

Uso la sostituzione 
$$
\begin{aligned}
x&=\tg{t}\\
x^2&=\tg^2{t}\\
dx&=\frac{1}{\cos^2{t}}\:dt
\end{aligned}
$$

E ottengo

$$
\begin{aligned}
\int \frac{1}{(1+\frac{\sin^2{t}}{\cos^2{t}})^2} \cdot \frac{1}{\cos^2{t}} \: dt &=\\
\int \cos^2{t} \: dt &=\\
\frac{1}{2}t+\frac{\sin{2t}}{4}&=\\
\frac{1}{2}\arctg{x}+\frac{\sin{2\arctg{x}}}{4}&=
\end{aligned}
$$

Per semplificare l'espressione ricordiamo le formule parametriche:
$$
\begin{aligned}
\sin{2t}&=\frac{2\tg{t}}{1+\tg^2{t}}
\end{aligned}
$$

Quindi sostituendo $t$ con $\arctg{x}$ ottengo

$$
\frac{1}{2}\arctg{x}+\frac{x}{2(1+x^2)}
$$

#### Integrazione per parti
L'integrazione per parti sfrutta la **derivata del prodotto**

$$
\int f(x)g'(x)dx=f(x)g(x)-\int f'(x)g(x)dx
$$

Esempio 1
$$
\begin{aligned}
\int x \cdot \sin{(x)} \: dx &= x(-\cos{x})-\int 1\cdot (-cos(x))dx\\
&= x\cos{(x)}+\sin{(x)}+c
\end{aligned}
$$

Caso particolare $\int \cos^2{x}$

$$
\begin{aligned}
\int \cos^2{x}\:dx&=\int\cos{x}\cos{x}\:dx\\
&=\cos{x}\sin{x}-\int -\sin{x}\sin{x}\: dx\\
&=\cos{x}\sin{x}+\int \sin^2{x} \: dx \\
&=\cos{x}\sin{x}+\int 1 \: dx -\int \cos^{2}{x}\:dx\\
2\int \cos^2{x}\:dx&=\cos{x}\sin{x}+x +c\\
\int \cos^2{x}\:dx&=\frac{\cos{x}\sin{x}}{2}+\frac{x}{2} +c
\end{aligned}
$$

## Integrali definiti
Prendo una funzione $f$ continua e positiva in $[a,b]$

$$
\begin{aligned}
\Delta x &= \frac{b-a}{n}\\
s_n&=\Delta x \cdot m_1+\Delta x \cdot m_2 +...+\Delta x m_n\\
S_n&=\Delta x \cdot M_1+\Delta x \cdot M_2 +...+\Delta x M_n\\
s_n&\le\text{Area sottesa}\le S_n\\
\lim_{n\to+\infty}s_n&=\lim_{n\to+\infty}S_n=\text{Area sottesa}=\int_a^b f \: dx
\end{aligned}
$$

Per calcolare l'integrale definito
$$
\begin{aligned}
F&=\int f \: dx \\
\int_a^b f\: dx &= F(b)-F(a)
\end{aligned}
$$

Per usare il cambio di variabile negli integrali definiti devo sostituire anche gli estremi dell'integrale.


## Calcolo dei volumi
### Volumi di solidi di rotazione
Possiamo calcolare il volume ottenuto dalla rotazione di un'area.

#### Rotazione attorno all'asse x
Analogamente agli integrali di area divido il volume in tanti "dischi" appena maggiori o appena minori del volume cercato.

Ogni disco piccolo ha come volume $\pi m^2 \Delta x$ e ogni disco grande $\pi M^2 \Delta x$.
Il volume del solido sarà quindi

$$
V=\pi \int_a^b [f(x)]^2 \:dx
$$

#### Rotazione attorno all'asse y
Invece di $f$ uso la sua inversa e come estremi dell'integrale uso gli estremi su y, non su x.

Altrimenti c'è un metodo alternativo. Invece di formare il nostro solido con monete impilate lo posso formare con tanti tubi verticali l'uno dentro l'altro

Ognuno dei tubi ha come area laterale $2\pi r h = 2\pi x f(x)$, quindi il volume del solido di rotazione diventa

$$
V=2\pi \int_a^b x f(x)\: dx
$$

## Lunghezza di una curva
Calcolare la lunghezza di un tratto di curva.

Divido la curva in tanti segmentini che la approssimano. La lunghezza del segmento generico $\overline{P_i P_{i+1}}$ è

$$
\overline{P_i P_{i+1}} = \sqrt{(x_{i+1}-x_i)^2+(f(x_{i+1})-f(x_i))^2}
$$

sfruttando il teorema del valore medio di Lagrange

$$
m=\frac{f(x_{i+1})-f(x_i)}{x_{i+1}-x_i}=f'(c)
$$

quindi

$$
\begin{aligned}
\overline{P_i P_{i+1}} &= \sqrt{(x_{i+1}-x_i)^2+f'(c_i)^2(x_{i+1}-x_i)^2}\\
&=(x_{i+1}-x_i)\sqrt{1+f'(c_i)^2}
\end{aligned}
$$

La lunghezza della curva è

$$
\begin{aligned}
L&=\lim_{n\to +\infty} \sum_{i=0}^n \overline{P_i P_{i+1}} \\
&=\int_a^b \sqrt{1+f'(x)^2} \: dx
\end{aligned}
$$

## Aree laterali di solidi
Divido il solido in tanti cilindri. L'area laterale di un cilindro è 

$$
2\pi \int_a^b f(x)\sqrt{1+f'(x)^2} \: dx
$$

## Integrali impropri
### Integrali con un numero finito di punti di discontinuità
#### f continua in $[a,b)$
$$
\begin{aligned}
A&=\int_a^b f(x)\: dx \\
&=\lim_{z\to b^-}\int_a^z f(x) \: dx
\end{aligned}
$$

Se il limite è finito l'integrale si dice convergente, se è infinito si dice divergente.
Se il limite non esiste si dice indeterminato.

#### f continua in $(a,b]$
$$
\begin{aligned}
A&=\int_a^b f(x)\: dx \\
&=\lim_{z\to a^+}\int_z^b f(x) \: dx
\end{aligned}
$$

#### f non continua in $c \in [a,b]$
$$
A=\lim_{z\to c^-}\int_a^z f(x) \: dx + \lim_{t\to c^+}\int_t^b f(x) \: dx
$$

### Integrali in un intervallo illimitato
$$
\int_a^{+\infty}f(x)\: dx = \lim_{z\to +\infty}\int_a^z f(x) \: dx
$$

## Integrali particolari
### Funzione gaussiana
$$
\int_{-\infty}^{+\infty}e^{-x^2}dx=\sqrt{\pi}
$$

x di grado dispari

$$
\int x \cdot e^{-x^2}dx=-\frac{1}{2}e^{-x^2}+c
$$

x di grado pari si usa per parti e si sfrutta l'integrale noto

