# Studio di funzione
Una funzione è una relazione tra 2 insieme che associa un elemento di $$A$$ ad un solo elemento di $$B$$.
$$
\forall \: x \in A \; \exists! \; y \in B \mid y=f(x) 
$$

## Ripasso
**DOMINIO:** l'insieme di tutti gli elementi dell'insieme $$A$$ che sono legati ad un elemento di $$B$$
**CODOMINIO:** l'insieme di tutti gli elementi dell'insieme $$B$$ che sono legati a uno o più elementi di $$A$$
Funzioni algebriche:
- razionali intere $$y=x$$
- razionali fratte $$y=\frac{1-x}{x+3}$$
- irrazionali $$y=\sqrt{x^2 - 1}$$

Funzioni trascendenti:
- logaritmiche
- esponenziali
- goniometriche

### Esercizi
#### Esercizio 1
Studio la funzione $$y=\frac{2-x}{x+5}$$
**DOMINIO:** $$x \ne -5 $$
**INTERSEZIONE CON GLI ASSI**
$$
\begin{cases}
x=0 \\
y = \frac{2-x}{x+5}
\end{cases}
\qquad
\begin{cases}
y=0 \\
y = \frac{2-x}{x+5}
\end{cases}
\\
\begin{cases}
x=0 \\
y = \frac{2}{5}
\end{cases}
\qquad
\begin{cases}
y=0 \\
x = 2
\end{cases}
$$
**STUDIO DEL SEGNO**
$$
\frac{2-x}{x+5}\gt 0 \\
-5 \lt x \lt 2
$$
**ASINTOTI**
$$
\begin{align*}
y&=\frac{2-x}{x+5} \\
&= -1 + \frac{7}{x+5} \\
y + 1 &= \frac{7}{x+5} \\
\text{asintoti: } x&=-5 \\ y&=-1
\end{align*}
$$

{% graph %}
{
    "grid": false,
    "xAxis": {
        "label": "x",
        "domain": [0, 30]
    },
    "yAxis": {
        "label": "y",
        "domain": [-1.5, 1.5]
    },
    "data": [{
        "fn": "( 2 - x )/( x + 5 )"
    }],
    "annotations": [{
        "x": -5,
        "text": "x = -5"
    }, {
        "y": -1,
        "text": "y = -1"
    }]
}
{% endgraph %}

#### Esercizio 2
$$
y=2^\sqrt{x} - \sqrt{2^x}
$$
**DOMINIO: ** $$x\ge0$$

$$
\begin{cases}
x\ge0 \\
2^x \ge 0
\end{cases}
\\
\Downarrow \\
x\ge0
$$

**INTERSEZIONI: ** (0,0) (4,0)
Con asse y
$$
\begin{cases}
x=0 \\
2^0 - \sqrt{2^0}
\end{cases}
\\
\Downarrow \\
y=0
$$

Con asse x
$$
\begin{cases}
y=0 \\
0 = 2^\sqrt{x} - \sqrt{2^x}
\end{cases} 
\\
\Downarrow \\
x_1 = 0 \quad x_2=4
$$

**SEGNO: ** $$0 \lt x \lt 4$$
$$
2^{\sqrt{x}}-\sqrt{2^x}\gt 0 \\
\Downarrow \\
0 \lt x \lt 4
$$
![](/assets/studio.png)

#### Esercizio 3
**DOMINIO: ** $$x\ne \frac{\pi}{6},\frac{11\pi}{6}$$

$$
2\cos{x}-\sqrt{3}\ne0 \\
x\ne \frac{\pi}{6},\frac{11\pi}{6}
$$

**INTERSEZIONI: ** (0,0) ($$\pi$$,0) ($$2\pi$$,0)
con x
$$
\begin{cases}
y=0\\
\sin{x}=0
\end{cases}
\\
\Downarrow
\\
x=0,\pi,2\pi
$$

### Caratteristiche delle funzioni
- **iniettive:** $$\forall \: x,y \in A \Rightarrow f(x)\ne f(y)$$
    - una funzione è reversibile se è iniettiva
- **suriettiva:** $$\forall \: y \in B \; \exists \: x \mid f(x)=y$$
- **biettiva:** sia iniettiva che suriettiva
- **crescente:** $$\forall \: x_1, x_2 \in A \mid x_1 < x_2 \Rightarrow f(x_1) \lt f(x_2)$$
- **monotòna:** una funzione si dice monotona se è sempre crescente o sempre decrescente nel suo dominio
- **periodica:** $$\exists \: T \mid f(x)=f(x+kT) \quad k \in \mathbb{Z}$$
- **pari:** $$\forall \: x \in A \; f(-x)=f(x)$$
- **dispari:** $$\forall \: x \in A \; f(-x)=-f(x)$$

## Sottoinsiemi di R
### Intervalli
Intervalli in $$\mathbb{R}$$
- **intervallo chiuso:** estermi inclusi $$[a,b]=\{x \mid x \in \mathbb{R} \quad a \ge x \ge b \}$$
- **intervallo aperto:**  estremi non inclusi $$(a,b) = ]a,b[$$
    - l'infinito non può mai essere incluso $$(- \infty, 5)$$
- **intervallo misto:** $$(a,b]$$

### Superiormente limitato
Un insieme $$A \subseteq \mathbb{R}$$ si dice **superiormente limitato** se $$\exists \; k \in \mathbb{R} \mid \forall \; x \in A \quad x \le k $$
$$k$$ non necessariamente deve appartenere ad $$\mathbb{R}$$, e.g.

$$
\begin{align*}
A &= \{ x \mid x = \frac{n}{n+1} \quad n \in \mathbb{N} \} \\
&= \{0,\frac{1}{2},\frac{2}{3},\frac{3}{4},...\}
\end{align*}
$$

$$A$$ è superiormente limitato da 1, anche se 1 non è incluso nell'insieme.
Analogamente un insieme può essere **inferiormente limitato**

### Estremo superiore
Dato $$A$$ superiormente limitato, si dice **estremo superiore** di $$A$$ quel numero $$M$$ tale che
- $$\forall x \in A \quad x \le M $$
- $$M \not\in A \to \forall \epsilon \gt 0 \; \exists x \in A  (x \ne M) \mid M - \epsilon \le x \le M $$

$$\epsilon$$ e $$\delta$$ in matematica indicano un numero positivo arbitrariamente piccolo

L'insieme $$A$$ (vedi sopra) ha come estremo superiore 1 e come estremo inferiore 0.

### Intorno
Si dice **intorno** di un punto $$ x_0 $$ un qualsiasi intervallo aperto contenente $$x_0$$, e.g. $$(x_0 - \delta \; , \; x_0 + \delta ) $$. Posso definire anche un intorno di infinito:
- intorno di $$+ \infty$$: $$(M \; , \; + \infty)$$
- intorno di $$- \infty$$: $$(- \infty \; , \; -M)$$


### Punto isolato
$$x_0$$ è detto **punto isolato** se esiste un intorno di $$x_0$$ che non contiene elementi di $$A$$ diversi da $$x_0$$

### Punto di accumulazione
$$x_0$$ si dice **punto di accumulazione** dell'insieme $$\mathbb{A}$$ se ogni intorno di $$x_0$$ contiene un elemento dell'insieme $$\mathbb{A}$$

$$
\forall \epsilon \gt 0\quad \exists x \in \mathbb{A} \mid x \in (x_0 - \epsilon, x_0 + \epsilon)
$$

E.g.
$$
\begin{align*}
A&=\{x \mid x = \frac{1}{n} \text{ con } n \in \mathbb{N} -\{0\}\} \\
&=\{0,\frac{1}{2},\frac{1}{3},\frac{1}{4}, \dots\}
\end{align*}
$$
A ha come punto di accumulazione 0.

## Limiti
### Comprensione intuitiva dei limiti
$$
\lim_{x \to 2} \frac{x^2-4}{x-2} \qquad \text{generica} \\
\lim_{x \to 2^-} \frac{x^2-4}{x-2} \qquad \text{da sinistra} \\
\lim_{x \to 2^+} \frac{x^2-4}{x-2} \qquad \text{da destra} \\
$$

**Valori della funzione avvicinandomi da sinistra**

| x | 1.9 | 1.99 | 1.999 |
| --- | --- | --- | --- |
| y | 3.9 | 3.99 | 3.999 |

Intuitivamente per $$x=2$$ attribuiremmo il valore 4, ma la funzione non vale 4, anzi la funzione non è nemmeno definita per $$x=2$$

$$
\lim_{x \to 2^-} \frac{x^2-4}{x-2} = 4
$$

**Valori della funzione avvicinandomi da destra** 

| x | 2.1 | 2.01 | 2.001 |
| --- | --- | --- | --- |
| y | 4.1 | 4.01 | 4.001 |

Anche in questo caso intuitivamente attribuiremmo valore 4 per $$x=2$$

$$
\lim_{x \to 2^+} \frac{x^2-4}{x-2} = 4
$$

### Definizione di limite
L'operazione di limite ha senso solamente quando $$x$$ tende ad un punto di accumulazione.

#### CASO l FINITO
$$
\lim_{x \to x_0} f(x) = l
$$
$$x_0$$ può essere sia un numero che infinito
$$I(x_0)$$ è un intorno di $$x_0$$
$$\forall$$ intorno di $$l$$ ($$\forall \epsilon \gt 0$$ arbitrariamente piccolo) $$\exists I(x_0) \text{ t.c. } \forall x \ne x_0 \in I(x_0) \Rightarrow \mid F(x) - l \mid  \lt \epsilon $$

**Verifica con la definizione il seguente limite**
$$
\lim_{x \to 2} \frac{x^2 -4}{x-2} = 4
$$

DEFINIZIONE
$$
\forall \epsilon \gt 0 \; \exists I(2) \text{ t.c. } \forall x \ne 2 \in I(2) \Rightarrow \mid \frac{x^2 -4}{x-2} - l \mid  \lt \epsilon 
$$

SVILUPPO LA CONDIZIONE
$$
\begin{align*}
\mid \frac{x^2 -4}{x-2} - l \mid &\lt \epsilon \\
\mid \frac{x^2 -4 -4x + 8}{x-2} \mid &\lt \epsilon \\
\mid \frac{x^2 -4x +4}{x-2} \mid &\lt \epsilon \\
\mid \frac{(x-2)^2}{x-2} \mid &\lt \epsilon \\
\mid x-2 \mid &\lt \epsilon
\end{align*}
$$

Sviluppando, ho verificato che x è molto vicino a 2, infatti la differenza tra 2 ed x è di minima (inferiore ad $$\epsilon$$)


#### Caso con limite infinito positivo
$$
\lim_{x \to x_0} f(x)=+\infty
$$

DEFINIZIONE
$$\forall M >0 \text{ arb. grande } \exists I(x_0) \mid \forall x \ne x_0 \in I(x_0) \Rightarrow f(x) \gt M$$

**Esempio**
$$
\lim_{x \to 1} \frac{1}{(x-1)^2} = + \infty
$$
VERIFICO LA CONDIZIONE
$$
\begin{align*}
\forall M>0 \; \exists I(x_0) \mid \forall x \ne x_0 \in I(x_0) \Rightarrow \frac{1}{(x-1)^2} &\gt M \\
\frac{1}{(x-1)^2} &\gt M \\
(x-1)^2 &\lt \frac{1}{M} \\
-\sqrt{\frac{1}{M}}  \lt x-1 &\lt +\sqrt{\frac{1}{M}} \\
1 -\sqrt{\frac{1}{M}} \lt x &\lt 1 +\sqrt{\frac{1}{M}}
\end{align*}
$$

Posso scegliere un M arbitrariamente grande, che porterà la condizione finale ad essere un intorno arbitrariamente piccolo.

#### Caso con limite infinito negativo
$$
\lim_{x \to x_0} f(x)=-\infty
$$

DEFINIZIONE
$$\forall M >0 \text{ arb. grande } \exists I(x_0) \mid \forall x \ne x_0 \in I(x_0) \Rightarrow f(x) \lt -M$$

**Esempio**
$$
\lim_{x \to 2} \frac{-3}{\mid x-2 \mid} = - \infty
$$

VERIFICO LA CONDIZIONE

$$
\begin{align*}
\frac{-3}{\mid x-2 \mid} &\lt -M \\
\frac{3}{\mid x-2\mid} &\gt M \\
\frac{-3}{M} \lt x-2 &\lt \frac{3}{M} \\
2 - \frac{3}{M} \lt x &\lt 2 + \frac{3}{M}
\end{align*}
$$

Analogamente a prima, posso scegliere un M arbitrariamente grande, che porterà l'ultima condizione ad essere un intorno arbitrariamente piccolo.

### Teoremi
#### Teorema di unicità
Se esiste il limite $$\lim_{x\to x_0} f(x)=l$$ allora tale limite è unico.

#### Teorema di permanenza del segno
Se $$\lim_{x\to x_0} f(x)=l$$ e $$l>0$$ allora esiste un intorno di $$X_0$$ tale che la funzione in quell'intorno è maggiore di 0

Ragionamento analogo si può svolgere anche con $$l<0$$

### Operazioni con i limiti
#### Proprietà lineari
**Limite della somma di 2 funzioni**
$$
\lim_{x \to x_0} [f(x)+g(x)]=\lim_{x\to x_0}f(x)+ \lim_{x\to x_0}g(x)
$$

E.g.
$$
\begin{align*}
\lim_{x\to x_0}(x+\frac{5}{x})&=\lim_{x\to - \infty}x + \lim_{x\to - \infty} \frac{5}{x} \\
&=-\infty + 0\\
&=- \infty \\

\lim_{x\to 0^+ } (\ln{x} + x^2) &= -\infty + 0 \\
&= -\infty \\

\lim_{x\to + \infty} x - 2^x &= + \infty -(+ \infty) \\
&= \text{forma indeterminata }+ \infty - \infty
\end{align*}
$$

**Limite del prodotto di 2 funzioni**
$$
\lim_{x \to x_0} [f(x)\cdot g(x)]=\lim_{x\to x_0}f(x) \cdot \lim_{x\to x_0}g(x)
$$

E.g.
$$
\lim_{x\to -\infty}x \cdot 2^x = \text{f.i. }0 \cdot \infty
$$

**Limite del rapporto di 2 funzioni**
$$
\lim_{x \to x_0} \frac{f(x)}{g(x)}=\frac{\lim_{x\to x_0}f(x)}{\lim_{x\to x_0}g(x)}
$$

E.g.
$$
\begin{align*}
\lim_{x\to x_0}\frac{\ln{x}}{e^{-x}} &=\frac{+\infty}{0} \\
&=+\infty
\end{align*}
$$

### Forme indeterminate
**Caso $$+\infty -\infty$$ in un polinomio**
$$
\lim_{x\to +\infty} x^4 -3x^2 +1 = fi +\infty -\infty
$$
Raccolgo il termine di grado più alto
$$
\lim_{x\to +\infty} x^4(1-\frac{3}{x^2} + \frac{1}{x^4})=+\infty
$$

**Caso $$+\infty -\infty$$ con una radice**
$$
\lim_{x\to +\infty} x-\sqrt{x^2 +1}=fi +\infty - \infty
$$

"Razionalizzo"

$$
\begin{align*}
&\lim_{x\to +\infty}x-\sqrt{x^2 + 1}\cdot \frac{x+\sqrt{x^2 +1}}{x+\sqrt{x^2+1}}= \\
&\lim_{x\to +\infty} \frac{x^2 -x^2 -1}{x+\sqrt{x^2 +1}}=0^-
\end{align*}
$$

**Caso $$\frac{\infty}{\infty}$$**
$$
\lim_{x\to + \infty} \frac{x^3+2x+3}{x^2+5}=fi \frac{\infty}{\infty}
$$

Raccolgo il termine di grado massimo sia al numeratore che al denominatore

$$
\begin{align*}
&\lim_{x\to +\infty} \frac{x^3(1+\frac{2}{x^2}+\frac{3}{x^3})}{x^2(1+\frac{5}{x^2})}= \\

&\lim_{x\to +\infty} \frac{x(1+\frac{2}{x^2}+\frac{3}{x^3})}{1+\frac{5}{x^2}}= +\infty
\end{align*}
$$

E.g.
$$
\begin{align*}
&\lim_{x\to + \infty} \frac{x^5-3x}{5x^2+4x^5} = \\
&\lim_{x\to +\infty} \frac{x^5(1-\frac{3}{x^4})}{x^5(\frac{5}{x^3}+4)}= \frac{1}{4}
\end{align*}
$$


Se i termini di grado massimo di numeratore e denominatore hanno lo stesso grado allora il limite è uguale al rapporto tra i coefficienti dei 2 termini.

**Forma indeterminata $$\frac{0}{0}$$**
$$
\begin{align*}
&\lim_{x\to 3}\frac{x^2-2x-3}{2x^2-9x+9}=fi\frac{0}{0} \\
&\lim_{x\to 3}\frac{(x-3)(x+1)}{(x-3)(2x-3)}=\\
&\lim_{x\to 3}\frac{x+1}{2x-3}=\frac{4}{3}
\end{align*}
$$

**Forma indeterminata $$0\cdot\infty$$**
$$
\begin{align*}
&\lim_{x\to\frac{\pi}{2}^+}(1-\sin{x})\tan{x} = fi \;0\cdot \infty \\
&\lim_{x\to\frac{\pi}{2}^+}(1-\sin{x})\frac{\sin{x}}{\cos{x}} \\
&\lim_{x\to\frac{\pi}{2}^+}(1-\sin{x})\frac{\sin{x}}{\cos{x}}\cdot\frac{1+\sin{x}}{1+\sin{x}} \\
&\lim_{x\to\frac{\pi}{2}^+}\cos{x}\cdot\sin{x}\cdot\frac{1}{1+\sin{x}}=0^-
\end{align*}
$$

**Forma indeterminata $$0^0$$, $$\infty^0$$, $$1^\infty$$**
$$
\begin{align*}
&\lim_{x\to x_0} {f(x) }^{g(x)} \\
&\lim_{x \to x_0} e^{(\ln{f(x)^{g(x)})}} \\
&\lim_{x \to x_0} e^{g(x)\cdot \ln{f(x)}}
\end{align*}
$$

E.g.
$$
\begin{align*}
&\lim_{x \to +\infty} x^{\frac{1}{\ln{x}}} \\
&\lim_{x \to + \infty} e^{\ln{(x^{\frac{1}{\ln{x}}})}} \\
&\lim_{x \to +\infty} e^{\frac{1}{\ln{x}}\cdot \ln{x}} \\
&\lim_{x \to + \infty} e^1 = e
\end{align*}
$$

### Asintoti
Una funzione ha come asintoto verticale la retta $$x=x_0$$ se
$$
\lim_{x \to x_0} f(x)= \infty
$$

Una funzione ha come asintoto orizzontale la retta $$y=y_0$$ se 
$$
\lim_{x\to +\infty} f(x) = y_0 \lor \lim_{x\to -\infty} f(x)=y_0
$$

Una funzione che non ha asintoti orizzontali potrebbe aver asintoti obliqui.
Cerco l'asintoto obliquo $$y=mx+q$$
Per trovare m: $$m=\lim_{x\to +\infty}\frac{f(x)}{x}$$ se m è finito continuo, se m non è finito allora l'asintoto obliquo non esiste.
Per trovare q: $$a=\lim_{x\to+\infty}[f(x)-mx]$$ se q è finito ho trovato l'asintoto obliquo, altrimenti l'asintoto obliquo non esiste.

### Teorema del confronto (o dei carabinieri)
Siano $$h,f,g$$ tre funzioni definite sullo stesso dominio.
$$
se \; \forall x \in D (x\ne x_0) \quad h(x) \le f(x) \le (g(x) \\
\land \\
\lim_{x \to x_0} h(x) = \lim_{x \to x_0}g(x) = l \\
\Downarrow \\
\lim{x \to x_0} f(x) = l
$$

E.g.
$$
\lim_{x \to + \infty} \frac{\sin{x}}{x} \\
-1 \le \sin{x} \le 1 \\
\frac{-1}{x} \le \frac{\sin{x}}{x} \le \frac{1}{x} \\
\lim_{x \to +\infty} \frac{-1}{x} = \lim_{x \to +\infty} = 0 \\
\Downarrow \\
\lim_{x \to +\infty}\frac{\sin{x}}{x}=0
$$

### Limiti notevoli
$$
\lim_{x\to 0} \frac{\sin{x}}{x} = 1
$$

**Dimostrazione**: $$y=\frac{\sin{x}}{x}$$ è una funzione pari (perchè $$f(x)=f(-x)$$) quindi 
$$
\lim_{x\to 0^-}\frac{\sin{x}}{x} = \lim_{x\to 0^+}\frac{\sin{x}}{x}
$$

Faccio il limite destro infatti se vedo x come l'angolo in radianti ossia la lunghezza dell'arco  sulla circonferenza goniometrica.

$$
\sin{x} \lt x \lt \tan{x} \\
1 \lt \frac{x}{\sin{x}} \lt \frac{1}{\cos{x}} \\
\cos{x} \lt \frac{\sin{x}} \lt 1 \\
1 \lt \frac{\sin{x}}{x} \lt 1
$$