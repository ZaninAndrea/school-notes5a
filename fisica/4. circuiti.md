## Circuiti RC
I circuiti RC sono circuiti composti da una resistenza e un condensatore collegati in serie ad una batteria.

### Carica del condensatore
$$
q(t)=C\epsilon(1-e^{-\frac{t}{RC}})
$$

$$
i(t)=\frac{\epsilon}{R}e^{-\frac{t}{RC}}
$$

$RC=\tau$ costante di tempo, l'unità di misura è il secondo.

$$
\frac{V}{A} \cdot \frac{C}{V}=\frac{1}{\frac{C}{s}} \cdot C=s
$$

Dopo un tempo $\tau$ la carica sul condensatore è già $\approx 63\%$ della carica massima

### Scarica del condensatore
$$
q(t)=C\epsilon e^{-\frac{t}{RC}}
$$

$$
i(t)=\frac{\epsilon}{R}e^{-\frac{t}{RC}}
$$

Notare che l'intensità decresce alla stessa maniera sia in un circuito di carica che di scarica