# Polinomi di Taylor e resto di Lagrange

## Che cosa sto approssimando?

Voglio approssimare il valore esatto $f(x)$ con un polinomio $P_n(x)$. Scelgo un centro $a$ dove conosco la funzione e le sue derivate. Il polinomio di Taylor di ordine $n$ si scrive

$$
P_n(x)=\sum_{k=0}^{n}\frac{f^{(k)}(a)}{k!}(x-a)^k.
$$

Il primo termine, quello di ordine $0$, vale $f(a)$. Per esempio, per $f(x)=e^x$ e $a=0$ vale $e^0=1$. Anche tutte le derivate di $e^x$, calcolate in $0$, valgono $1$. È per questo che nello sviluppo dell’esponenziale compaiono i termini $1$, $x$, $x^2/2!$, $x^3/3!$ e così via.

## Come misuro l’errore?

L’errore è dato dalla differenza tra il valore esatto e l’approssimazione. Chiamo questa differenza $R_n(x)$. Se la funzione ha derivate continue fino all’ordine $n+1$ nell’intervallo tra $a$ e $x$, la formula di Taylor con resto di Lagrange dà

$$
R_n(x)=f(x)-P_n(x)=\frac{f^{(n+1)}(\xi)}{(n+1)!}(x-a)^{n+1}.
$$

Qui $n$ è l’ordine intero del polinomio. La scritta $f^{(n+1)}(\xi)$ indica la derivata di ordine $n+1$ calcolata in un punto $\xi$ compreso tra $a$ e $x$. Quando voglio misurare **quanto è grande l’errore**, confronto il suo valore assoluto $|R_n(x)|$ con la precisione richiesta.

## Esempio dei miei appunti · Approssimare $\sqrt e$ con errore inferiore a $10^{-4}$

**1. Scrivo l’errore e lascio $n$ da determinare.** Siccome $\sqrt e=e^{1/2}$, uso $f(x)=e^x$ con centro $a=0$ e calcolo il polinomio nel punto $x=1/2$. Quindi $0<\xi<1/2$ e la derivata che compare nel resto vale $e^\xi$.

$$
\sqrt e-P_n\left(\frac12\right)
=\frac{e^\xi}{(n+1)!}\left(\frac12-0\right)^{n+1}
=\frac{e^\xi}{2^n\cdot 2\cdot(n+1)!}.
$$

Questa quantità è positiva. In questo esempio coincide quindi con $|R_n(1/2)|$, l’errore da confrontare con $10^{-4}$.

**2. Scelgo un maggiorante di $e^\xi$.** L’esponenziale è crescente, quindi $e^\xi<e^{1/2}=\sqrt e$. So anche che $e<4$, dunque $\sqrt e<\sqrt4=2$. Perciò $e^\xi<2$.

Se metto $2$ al numeratore, ottengo una frazione più grande dell’errore vero. Se questa frazione è minore di $10^{-4}$, lo sarà anche l’errore vero. Il $2$ è comodo anche perché si semplifica:

$$
\left|R_n\left(\frac12\right)\right|
=\frac{e^\xi}{2^n\cdot 2\cdot(n+1)!}
<\frac{2}{2^n\cdot 2\cdot(n+1)!}
=\frac{1}{2^n(n+1)!}.
$$

**3. Ora scelgo l’ordine $n$.** Per avere la precisione richiesta mi basta verificare

$$
\frac{1}{2^n(n+1)!}<\frac{1}{10^4}
\quad\Longleftrightarrow\quad
2^n(n+1)!>10^4.
$$

Con $n=5$ ottengo $2^5\cdot6!=32\cdot720=23040>10000$. Quindi l’ordine $5$ basta.

**4. Scrivo l’approssimazione.** Nell’esponenziale sostituisco $x=1/2$ e tengo i termini dall’ordine $0$ all’ordine $5$:

$$
P_5\left(\frac12\right)
=1+\frac12+\frac{1}{4\cdot2!}+\frac{1}{8\cdot3!}
+\frac{1}{16\cdot4!}+\frac{1}{32\cdot5!}.
$$

Questa somma è la mia approssimazione. Per scrivere il valore esatto aggiungo il resto:

$$
\sqrt e=P_5\left(\frac12\right)+R_5\left(\frac12\right),
\qquad
\left|R_5\left(\frac12\right)\right|<\frac{1}{23040}<10^{-4}.
$$
