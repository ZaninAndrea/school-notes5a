# Elettrostatica
<!-- toc -->

## Metodi di carica
Materiali:
* isolanti, gli elettroni non si spostano all'interno
* conduttori, hanno degli elettroni liberi di muoversi

Metodi di carica: 
- strofinamento, va bene sia per isolanti che per conduttori, la carica dipende dal materiale
- contatto, solo per i conduttori, gli elettroni si trasferiscono per ridistribuirsi
- induzione, solo per i conduttori, una carica esterna divide le cariche interne positive e negative, successivamente una delle 2 cariche esterne viene sottratta e l'oggetto rimane quindi con un eccesso dell'altra carica

## Forza elettrica
La forza elettrica può essere sia attrattiva che repulsiva.
La forza elettrica è una forza conservativa.
La **legge di Coulomb** che descrive la forza elettrica è analoga alla legge dell'attrazione gravitazionale.
$$
\begin{align*}
\overrightarrow{F_{el}}&=k\frac{q_1 q_2}{r^2}\\
k&=8.99\cdot 10^9 \frac{Nm^2}{C^2} \\
\overrightarrow{F_{el}}&=\frac{1}{4\pi \epsilon_0}\cdot \frac{q_1 q_2}{r^2} \\
\epsilon_0&=8.85\cdot 10^{-12}\frac{C^2}{Nm^2}
\end{align*}
$$
Quanità di carica di un elettrone o protone
$$
e=1.602 \cdot 10^{-19} C
$$

A livello microscopico le forze elettriche sono molto più grandi delle forze gravitazionali (all'interno di un atomo la differenza ha un ordine di grandezza di $$10^{39}$$)

## Campo elettrico
Se una carica di prova $$q_0$$ è sottoposta ad una forza $$\overrightarrow{F}$$ in un certo punto allora il **campo elettrico** in quel punto è
$$
\overrightarrow{E}=\frac{\overrightarrow{F}}{q_0}
$$

La presenza di una carica genera un campo elettrico ed esso influenza tutte le cariche nello spazio, un cambiamento in una carica si ripercuote sul campo elettromagnetico alla velocità della luce. Il campo elettrico generato in un punto $$A$$ da una carica $$q_1$$ è
$$
\overrightarrow{E}(A,q_1)=\frac{1}{4\pi \epsilon_0} \cdot \frac{q_1}{d^2}
$$

Il campo elettrico è anche una **funzione vettoriale della posizione**.
Posso rappresentare un campo elettrico con le **linee di forza**, che
* sono uscenti dalle cariche positive ed entranti nelle cariche negative
* il numero di linee è proporzionale all'intensità della carica
* sono simmetriche in tutte 3 le dimensioni
* la densità di linee è proporzionale all'intensità del campo
* due linee di uno stesso campo non possono incrociarsi

![linee di forza](/assets/Linee-Forza-Cariche-Puntiforme-300x150.png)

## Teorema di Gauss
### Flusso di campo elettrico
Il flusso di campo elettrico $$\theta_E$$ è definito come
$$
\theta_E \overset{\text{def}}{=} \sum_i \overrightarrow{E_i} \cdot \Delta \overrightarrow{S}
$$

$$\overrightarrow{S_i}$$ è il vettore superficie, ossia il vettore normale alla superficie, con modulo uguale all'area della superficie e uscente dalla stessa. 
Posso pensarlo anche come 
$$
\theta_E = \text{linee di campo }\overrightarrow{E}\text{ uscenti }-\text{linee di campo }\overrightarrow{E}\text{ entranti} $$

### Teorema
Il teorema di Gauss dice che 
$$
\theta_E = \frac{Q_{\text{interno}}}{\epsilon_0}
$$

### Applicazioni
#### Calcolare il campo elettrico di un filo
La **densità lineare di carica** è definita come 
$$
\lambda = \frac{q}{l}
$$
Scelgo una superficie simmetrica rispetto al filo: un cilindro. Le faccie superiore e inferiore del cilindro non sono bucate da linee di campo in quanto sono perpendicolari alle stesse
$$
\begin{align*}
\theta_E &= \overrightarrow{E} \cdot S_1 \cdot \cos{90°} + \overrightarrow{E} \cdot S_2 \cdot \cos{90°} + \overrightarrow{E} \cdot S_3 \cdot cos{0°} \\
 &= 0 + 0 + E \cdot 2\pi r h \\
\theta_E &= \frac{q_{\text{interna}}}{\epsilon_0} \\
&= \frac{\lambda \cdot h}{\epsilon_0} \\
\overrightarrow{E} \cdot 2\pi r h &= \frac{\lambda \cdot h}{\epsilon_0} \\ 
&\Downarrow \\
E &= \frac{\lambda}{2\pi \epsilon_0 r}
\end{align*}
$$

#### Calcolare il campo elettrico di una lamina 
Scelgo come superficie quella ci un cilindro che attraversa la lamina, la cui superficie circolare non è quindi bucata da linee di campo. 
$$\sigma$$ indica la **densità superficiale di carica**.
$$
\begin{align*}
\theta_E &= \overrightarrow{E} \cdot \overrightarrow{S_1} \cdot cos{0°} + \overrightarrow{E} \cdot \overrightarrow{S_2} \cdot cos{0°} + \overrightarrow{E} \cdot \overrightarrow{S_3} \cdot cos{90°} \\
&= \overrightarrow{E} \cdot \overrightarrow{S_1} + \overrightarrow{E} \cdot \overrightarrow{S_2}  \\
\theta_E &= \frac{q_{\text{interna}}}{\epsilon_0} \\
&= \frac{\sigma \cdot S_1}{\epsilon_0} \\
2\overrightarrow{E}S_1 &= \frac{\sigma \cdot S_1}{\epsilon_0} \\
&\Downarrow \\
\overrightarrow{E} &= \frac{\sigma}{2\epsilon_0}
\end{align*}
$$
Quindi il campo elettrico generato da una lamina non dipende dalla distanza, supponendo che la lamina sia infinitamente larga.

#### Campo elettrico di una sfera uniformemente carica
Una sfera nella quale la carica è uniformemente distribuita.
Densità volumica/volumetrica di carica $$\rho = \frac{q}{V}$$
##### All'interno della sfera
$$
\begin{align*}
\theta_E(s) &= \overrightarrow{E} \cdot \overrightarrow{S} \\
&= \overrightarrow{E} \cdot 4\pi r^2 \\
\theta_E (s) &= \frac{\rho \cdot \frac{4}{3}\pi r^3 }{\epsilon_0} \\
\overrightarrow{E} \cdot 4\pi r^2 &= \frac{\rho \cdot \frac{4}{3}\pi r^3 } {\epsilon_0} \\
&\Downarrow \\
\overrightarrow{E} &= \frac{\rho r}{3 \epsilon_0} 
\end{align*}
$$

##### All'esterno della sfera
$$
\begin{align*}
\theta_E(s) &= \overrightarrow{E} \cdot \overrightarrow{S} \\
&= \overrightarrow{E} \cdot 4\pi r^2 \\
\theta_E (s) &= \frac{\rho \cdot \frac{4}{3}\pi R^3 }{\epsilon_0} \\
\overrightarrow{E} \cdot 4\pi r^2 &= \frac{\rho \cdot \frac{4}{3}\pi R^3 } {\epsilon_0} \\
&\Downarrow \\
\overrightarrow{E} &= \frac{\rho R^3}{3 \epsilon_0 r^2} 
\end{align*}
$$

Si comporta esattamenta come una carica puntiforme, quindi posso usare anche la formula della carica puntiforme
$$
\begin{align*}
\overrightarrow{E} &= \frac{\rho R^3}{3 \epsilon_0 r^2} \\
&= \frac{\rho \frac{4}{3}\pi R^3}{4\pi \epsilon_0 r^2} \\
&= \frac{1}{4\pi \epsilon_0} \cdot \frac{q}{r^2}
\end{align*}
$$

## Potenziale
$$
\Delta V \overset{\text{def}}{=} \frac{\Delta U}{q_0} = - \frac{W}{q_0}
$$

$$\Delta U$$ è la differenza di potenziale elettrico
$$\Delta V$$ è la differenza di potenziale

Il potenziale diminuisce se ci si muove nella direzione del campo elettrico, quindi le cariche posistive si muovono verso zone di potenziale basso e quelle negative verso zone di potenziale alto.

Il potenziale è una grandezza scalare

L'unità di misura della differenza di potenziale è il **Volt,** indicato con $$V=1\frac{J}{C}$$
L'energia si può misurare utilizzando l'unità **elettronvolt**: $$eV=e\cdot 1V = 1.6 \cdot 10^{-19} J$$

### Differenza di potenziale in un campo elettrico uniforme
![](/assets/campo.PNG)
$$
\begin{align*}
W&=F_{el}\cdot \Delta s \\
&=q_0 E \Delta s \\
&\downarrow \\
\Delta V &= - \frac{W}{q_0} \\
&= - \frac{q_0 E \Delta s}{q_0} \\
&= - E \Delta s \\
&\downarrow \\
E&=-\frac{\Delta V}{\Delta s}
\end{align*}
$$

### Differenza di potenziale in un campo generato da una carica puntiforme
![](/assets/campo2.png)
Con il calcolo integrale la formula risulta:
$$
\begin{align*}
V_A - V_B &= \frac{1}{4\pi \epsilon_0}\frac{q}{r_A} - \frac{1}{4\pi \epsilon_0}\frac{q}{r_B} \\
V(r) &= \frac{1}{4\pi \epsilon_0}\frac{q}{r}
\end{align*}
$$

Se $$r \to + \infty$$ allora $$V \to 0$$

### Superfici equipotenziali
Le linee equipotenziali sono perpendicolari alle linee di campo. Nel caso di una carica puntiforme le superfici equipotenziali sono sfere.

### Conduttori
![](/assets/punte.png)
Prendo 2 sferette conduttrici una più piccola _r_ e una più grande _R_. Le carico con la stessa quantità di carica positiva e quindi la sfera più piccola avrà potenziale maggiore.
Successivamente collego le 2 sfere con un filo conduttore, quindi gli elettroni si muovono verso le zone di potenziale alto (la sferetta piccola); gli elettroni continueranno a fluire finchè le 2 sferette avranno lo stesso potenziale

$$
\begin{align*}
V_1&=V_2 \\
\frac{1}{4\pi\epsilon_0}\frac{Q_r}{r} &= \frac{1}{4\pi\epsilon_0}\frac{Q_R}{R} \\
\frac{Q_r}{Q_R}&=\frac{r}{R} \\
E_r &= \frac{1}{4\pi\epsilon_0}\frac{Q_r}{r^2} \\
E_R &= \frac{1}{4\pi\epsilon_0}\frac{Q_R}{R^2} \\
\frac{E_r}{E_R} &= \frac{Q_r}{r^2}\frac{R^2}{Q_R} \\
&= \frac{r}{R}\frac{R^2}{r} \\
&= \frac{R}{r} \\
\sigma_r &= \frac{Q_r}{4\pi r^2} \\
\sigma_R &= \frac{Q_R}{4\pi R^2} \\
\frac{\sigma_r}{\sigma_R} &= \frac{Q_r}{r^2}\frac{R^2}{Q_R} \\
&= \frac{R}{r}
\end{align*}
$$

Troviamo quindi 3 relazioni importanti:
- tra i raggi e la cariche $$\frac{Q_r}{Q_R}=\frac{r}{R}$$ 
- tra i raggi e i campi elettrici $$\frac{E_r}{E_R}=\frac{R}{r}$$
- tra i raggi e le distribuzioni di carica $$\frac{\sigma_r}{\sigma_R}=\frac{R}{r}$$

Dall'ultima relazione possiamo capire che **sulle punte le cariche sono più concentrate**.

Con una punta è facile avere un campo elettrico che superi la rigidità dielettrica dell'aria e riuscire quindi a far passare degli ioni attraverso l'aria. Infatti se mettiamo una punta carica vicino ad una candela "vediamo" il vento elettrico

### Condensatore
Un condensatore è un dispositivo per immagazzinare energia elettrica.
Un semplice comndensatore è il **condensatore a facce piane parallele**, ossia 2 lamine cariche con la stessa densità di carica ma segno opposto poste vicine e parallele.

La **capacità** di un condensatore è il rapporto tra la quantità di carica e la differenza di potenziale elettrico che riesco a creare $$C=\frac{Q}{V}$$, l'unità di misura è il farad **F**. 
$$
\begin{align*}
Q&=\sigma A \\
E&=\frac{\sigma}{\epsilon_0} \\
\Delta V&=E\cdot d \\
&=\frac{\sigma}{\epsilon_0}\cdot d \\
C&=\frac{\sigma A}{\frac{\sigma d}{\epsilon_0}} \\
&=\frac{\epsilon_0 A}{d}
\end{align*}
$$

Dall'ultima formula $$C=\frac{\epsilon_0 A}{d}$$ capiamo che la capacità dipende solo dalla geometria del condensatore. 

Per aumentare la capacità del condensatore separo le 2 piastre con un sottile strato di un isolante, detto **dielettrico**, che separa fisicamente le 2 piastre. I dipoli indotti nell'isolante formano un campo elettrico che contrasta quello delle 2 lamine, dato che il campo elettrico complessivo si riduce, la **capacità aumenta**. La nuova capacità del condensatore è determinata dalla formula

$$
C=\frac{\epsilon_r \epsilon_0 A}{d}
$$

Dove $$\epsilon_r$$ è la costante dielettrca di quel materiale.

Tensioni molto alte possono portare alla **rottura del dielettrico**, ossia il campo elettrico è abbastanza elevato da rompere i legami tra tomi e rendere il materiale un conduttore. 
La massima intensità di campo elettrico che il dielettrico può sopportare è detta **rigidità dielettrica**.
Il dielettrico inoltre dovrebbe avere una rigidità elettrica maggiore dell'aria, in modo da permettere di avere differenze di potenziale molto alte.

L'energia immagazzinata in un condensatore è:

$$
\begin{align*}
U&=\frac{1}{2}CV^2 \\
&=\frac{1}{2}QV \\
&=\frac{1}{2}\frac{Q^2}{C}
\end{align*}
$$

La densità di energia, ossia l'energia per unità di volume è:

$$
\begin{align*}
\mu_E&=\frac{\frac{1}{2}QV}{Ad}  \\
&=\frac{1}{2}\epsilon_0 E^2
\end{align*}
$$