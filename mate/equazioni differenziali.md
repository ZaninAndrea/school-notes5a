# Equazioni differenziali
## Equazioni di primo ordine
Solo con $x,y,y'$
### Senza y
$$
y'=f(x)
$$

E.g.

$$
\begin{aligned}
y'&=2x^3-\ln{x}\\
y&=\int (2x^3-\ln{x}) dx
\end{aligned}
$$

### Equazioni a variabili separabili
$$
y'=f(x)\cdot g(x)
$$

E.g.

$$
\begin{aligned}
2y'&=xy+2y\\
2\frac{dy}{dx}&=(x+2)y\\
\int\frac{2}{y}dy&=\int(x+2)dx\\
2\ln{| y |}&=\frac{x^2}{2}+2x+c\\
|y|&=e^{\frac{x^2}{4}+x+c}
\end{aligned}
$$

### Equazioni lineari
$$
y'=a(x)y+b(x)
$$

Procedimento:

$$
\begin{aligned}
A(x)&=\int a(x) dx\\
y&=e^{A(x)}\cdot \bigg[\int b(x)e^{-A(x)} dx + c\bigg]
\end{aligned}
$$

Dimostrazione

$$
\begin{aligned}
y'-a(x)y&=b(x)\\
y'e^{-A(x)}-a(x)e^{-A(x)}y&=b(x)e^{-A(x)}\\
D\Big[ye^{-A(x)}\Big]&=b(x)e^{-A(x)}\\
ye^{-A(x)}&=\int b(x)e^{-A(x)} dx \\
y&=e^{A(x)}\cdot \bigg[\int b(x)e^{-A(x)} dx + c\bigg]
\end{aligned}
$$

E.g.
$$
\begin{aligned}
x&\gt0\\
y'+\frac{y}{x}&=x\\
y'&=-\frac{1}{x}y+x\\
A(x)&=-\ln{x}\\
y&=e^{-\ln{x}}\bigg[\int x e^{\ln{x}}dx+c \bigg]\\
&=\frac{1}{x}\bigg[\int x^2 dx + c \bigg]\\
&=\frac{1}{x}\bigg[\frac{x^3}{3}+c \bigg]
\end{aligned}
$$

