# Limiti di funzioni

Appunti della **lezione del 12/10/2026**, confrontati con i **limiti di successioni** delle lezioni precedenti.

Le due colonne affiancano gli stessi concetti, **quando il parallelismo è corretto**. Le formule sono mantenute brevi per facilitare la lettura su GitHub.

## 1. Esempio introduttivo: teorema del confronto

| Limiti di successioni — lezione 07/10 | Limiti di funzioni — lezione 12/10, pagina 15 |
| :--- | :--- |
| Consideriamo $a_n=\frac{(-1)^n}{n}$. | Consideriamo $f(x)=x\sin(\frac{1}{x})$, con $x\neq 0$. |
| La parte oscillante soddisfa $-1\leq(-1)^n\leq 1$. | La parte oscillante soddisfa $-1\leq\sin(1/x)\leq 1$. |
| Quindi $-\frac{1}{n}\leq a_n\leq\frac{1}{n}$, per $n\geq1$. | Quindi $-\lvert x\rvert\leq f(x)\leq\lvert x\rvert$. |
| Poiché $\frac{1}{n}\to0$ e $-\frac{1}{n}\to0$, per confronto **$a_n\to0$**. | Poiché $\lvert x\rvert\to0$ e $-\lvert x\rvert\to0$ per $x\to0$, per confronto **$\lim_{x\to0}f(x)=0$**. |

**Idea comune:** il termine oscillante non ha bisogno di convergere: il fattore che tende a zero lo comprime tra due quantità che tendono a zero.

**Differenza:** nella successione l'indice $n$ cresce senza limite; nella funzione l'argomento $x$ si avvicina a $0$ da entrambi i lati. Inoltre, $f(0)$ **non è definita**, ma il limite esiste comunque.

## 2. Intorni (lezione 12/10, pagina 18)

Un **intorno** descrive matematicamente quali punti sono vicini a un punto fissato. Il collegamento con le successioni è la nozione di **soglia**.

| Limiti di successioni — lezione 30/09 | Limiti di funzioni — lezione 12/10, pagina 18 |
| :--- | :--- |
| Per $n\to+\infty$ consideriamo tutti gli indici oltre una soglia: **$n>N$**. | Per $x\to x_0$ consideriamo un **intorno di $x_0$** di raggio $r>0$: **$I_r(x_0)=(x_0-r,\ x_0+r)$**. |
| Gli indici considerati appartengono alla semiretta $(N,+\infty)$ (e sono naturali). | I punti dell'intorno verificano **$\lvert x-x_0\rvert<r$**; gli estremi sono esclusi. |
| Per un limite finito $\ell$, da un certo indice in poi vale $\lvert a_n-\ell\rvert<\varepsilon$. | Per un limite finito $\ell$, richiederemo $\lvert f(x)-\ell\rvert<\varepsilon$ quando $x$ è sufficientemente vicino a $x_0$ (definizione formale a pagina 24). |

**Esempio di intorno di un punto reale:** per $x_0=3$ e $r=0{,}5$,

$$
I_{0{,}5}(3)=(3-0{,}5,\ 3+0{,}5)=(2{,}5,\ 3{,}5).
$$

### Intorni di infinito

| Successioni | Funzioni |
| :--- | :--- |
| La condizione $n>N$ significa che l'indice è in un intorno di $+\infty$, limitandosi agli interi naturali. | Un intorno di $+\infty$ è $(a,+\infty)$, con $a\in\mathbb{R}$. |
| Le successioni studiate qui hanno indice $n\to+\infty$. | Per le funzioni si considera anche $x\to-\infty$: un suo intorno è $(-\infty,a)$. |

**Attenzione:** $r$ (o $\delta$ nelle definizioni successive) controlla la vicinanza **dell'argomento** a $x_0$; $\varepsilon$ controlla la vicinanza **dei valori** della funzione al limite $\ell$. Non sono intercambiabili.

---

## 3. Punti di accumulazione (pagina 19 del PDF)

La slide introduce i **punti di accumulazione di un insieme** $D\subseteq\mathbb{R}$: non è ancora una definizione di limite di funzione.

| Limiti di successioni — lezioni precedenti | Punti di accumulazione — lezione 12/10 |
| :--- | :--- |
| Il limite $a_n\to\ell$ descrive il comportamento dei **termini** quando $n\to+\infty$. | $x_0$ è di accumulazione per $D$ se in **ogni suo intorno** c'è almeno un punto di $D$ **diverso da $x_0$**. |
| Per ogni $\varepsilon>0$ esiste $N$ tale che **per tutti** gli $n>N$ vale $\lvert a_n-\ell\rvert<\varepsilon$. | Per ogni $\delta>0$ **esiste almeno un** $x\in D$ tale che $0<\lvert x-x_0\rvert<\delta$. |
| Il limite $\ell$ può non essere un termine della successione. | Il punto $x_0$ può non appartenere all'insieme $D$. |
| **Tutti i termini sufficientemente avanti** devono avvicinarsi a $\ell$. | È sufficiente trovare **almeno un punto diverso da $x_0$ in ogni intorno**. |

**Definizione della slide:**

$$
\forall\delta>0\ \exists x\in D:\ 0<|x-x_0|<\delta.
$$

**Collegamento tramite successioni (conseguenza della definizione):** $x_0$ è di accumulazione per $D$ se e solo se esiste **una successione** $(x_n)$ di elementi di $D\setminus\{x_0\}$ tale che $x_n\to x_0$. Non è necessario che *ogni* successione di punti di $D$ converga a $x_0$.

## 4. Esempi di punti di accumulazione (pagina 21 del PDF)

### Esempio A: intervallo e punto isolato

$$
A=(1,4]\cup\{6\},
\qquad \mathrm{Acc}(A)=[1,4]
$$

| Successioni — parallelismo | Punti di accumulazione — spiegazione |
| :--- | :--- |
| $x_n=1+\frac1n\to1$, con $x_n\in A$ e $x_n\neq1$. | **$1$ è di accumulazione**, anche se $1\notin A$: i punti di $A$ si avvicinano a $1$ da destra. |
| $y_n=4-\frac1n\to4$, con $y_n\in A$ e $y_n\neq4$. | **$4$ è di accumulazione**: ci sono punti di $A$ arbitrariamente vicini a $4$ da sinistra. |
| Non può esistere una successione di punti di $A\setminus\{6\}$ che converga a $6$. | **$6$ è isolato**, perché $(5,7)\cap A=\{6\}$: togliendo il punto $6$, l'intorno non contiene altri punti di $A$. |
| Anche ogni $c\in(1,4)$ può essere avvicinato con punti distinti di $A$. | Tutti i punti tra $1$ e $4$ sono di accumulazione. |

### Esempio B: i reciproci dei naturali

$$
B=\{\,\frac1n:n=1,2,3,\ldots\,\}.
$$

| Successioni — parallelismo | Punti di accumulazione — spiegazione |
| :--- | :--- |
| $b_n=\frac1n\to0$. | **$0$ è di accumulazione**: esistono elementi di $B$ arbitrariamente vicini a $0$, anche se $0\notin B$. |
| Per ogni termine fissato $b_m=\frac1m$ ci sono un precedente e un successivo distinti, salvo il primo. | Ogni $\frac1m$ è un **punto isolato** di $B$: esiste un suo intorno abbastanza piccolo senza altri elementi di $B$. |
| Il limite della successione è $0$. | Il **solo** punto di accumulazione di $B$ è $0$: $\mathrm{Acc}(B)=\{0\}$. |

**Attenzione:** il fatto che la successione $1/n$ converga a $0$ non rende ogni suo termine un punto di accumulazione dell'insieme dei suoi valori.

## 5. Verifica con la definizione (pagina 22 del PDF)

La pagina dimostra che $0$ è di accumulazione per $B$ scegliendo un elemento $1/n$ sufficientemente vicino a $0$.

| Successioni — limite già conosciuto | Insieme $B$ — verifica del punto di accumulazione |
| :--- | :--- |
| $\frac1n\to0$: fissato $\varepsilon>0$, per **tutti** gli $n>1/\varepsilon$ vale $\lvert\frac1n-0\rvert<\varepsilon$. | Fissato $\delta>0$, basta **scegliere un** $n\in\mathbb N$, $n\ge1$, con $n>1/\delta$: allora $0<\frac1n<\delta$. |
| La condizione riguarda **tutti i termini da una certa soglia in poi**. | La definizione richiede **l'esistenza di un punto** di $B$ nell'intorno, diverso da $0$. |

Passaggi:

$$
0<\frac1n<\delta
\quad\Longleftrightarrow\quad
n>\frac1\delta.
$$

Per la proprietà di Archimede esiste sempre un naturale che supera $1/\delta$. Quindi

$$
0\in\mathrm{Acc}(B)
$$

**Perché gli altri punti sono isolati?** Per $m\ge2$ i due termini adiacenti a $1/m$ sono ordinati così:

$$
\frac{1}{m+1}<\frac1m<\frac{1}{m-1}.
$$

Possiamo scegliere un intorno sufficientemente piccolo di $1/m$ che non raggiunga i termini vicini (e quindi nessun altro punto di $B$). Anche $1$ è isolato.

---

## 6. Punto di accumulazione e limite — pagina 23

Consideriamo nuovamente la funzione della pagina 15:

$$
f(x)=x\sin(1/x),\qquad D=\mathbb{R}\setminus\{0\}.
$$

Il punto $x_0=0$ **non appartiene al dominio**, ma è un **punto di accumulazione di $D$**: possiamo avvicinarci a $0$ con punti di $D$ diversi da $0$.

| Limiti di successioni | Limiti di funzioni — pagina 23 |
| :--- | :--- |
| Per $a_n=1/n$ cerchiamo una soglia $N$ oltre la quale $\lvert a_n\rvert<\varepsilon$. | Per $f(x)=x\sin(1/x)$ cerchiamo un raggio $\delta$ tale che $\lvert f(x)\rvert<\varepsilon$ se $x$ è vicino a $0$. |
| Basta scegliere $N\geq1/\varepsilon$: per tutti gli $n>N$ vale $1/n<\varepsilon$. | Basta scegliere **$\delta=\varepsilon$**: se $0<\lvert x\rvert<\delta$, allora $\lvert f(x)\rvert\leq\lvert x\rvert<\varepsilon$. |
| Quindi $\lim_{n\to+\infty}1/n=0$. | Quindi $\lim_{x\to0}x\sin(1/x)=0$. |

**Verifica:**

$$
\lvert\sin(1/x)\rvert\leq1
\quad\Longrightarrow\quad
\lvert f(x)\rvert\leq\lvert x\rvert.
$$

Fissato $\varepsilon>0$, scegliamo $\delta=\varepsilon$. Per ogni $x\in D$ con $0<\lvert x\rvert<\delta$:

$$
\lvert f(x)-0\rvert\leq\lvert x\rvert<\delta=\varepsilon.
$$

**Nota:** $f(0)$ non è definita, ma questo non impedisce l'esistenza del limite.

## 7. Definizione di limite finito — pagina 24

Siano $D\subseteq\mathbb{R}$, $f:D\to\mathbb{R}$ e $x_0$ un **punto di accumulazione di $D$**. Il numero $\ell$ è il limite di $f(x)$ per $x\to x_0$ quando:

$$
\forall\varepsilon>0\quad\exists\delta>0
$$

tale che, **per ogni $x\in D$**,

$$
0<\lvert x-x_0\rvert<\delta
\quad\Longrightarrow\quad
\lvert f(x)-\ell\rvert<\varepsilon.
$$

Si scrive:

$$
\lim_{x\to x_0}f(x)=\ell.
$$

### Parallelismo con la definizione delle successioni

| Successioni — lezione 30/09 | Funzioni — lezione 12/10 |
| :--- | :--- |
| $\lim_{n\to+\infty}a_n=\ell$. | $\lim_{x\to x_0}f(x)=\ell$. |
| Si fissa **$\varepsilon>0$**. | Si fissa **$\varepsilon>0$**. |
| Si trova una **soglia $N$**. | Si trova un **raggio $\delta>0$**. |
| Per ogni $n>N$: $\lvert a_n-\ell\rvert<\varepsilon$. | Per ogni $x\in D$ con $0<\lvert x-x_0\rvert<\delta$: $\lvert f(x)-\ell\rvert<\varepsilon$. |

**Differenza:** nella successione consideriamo tutti gli indici oltre $N$; nella funzione tutti i punti del dominio sufficientemente vicini a $x_0$, **escluso $x_0$**.

**Osservazione della slide:** il valore $f(x_0)$ è irrilevante. Può essere non definito oppure diverso da $\ell$.

## 8. Interpretazione grafica — pagina 25

La condizione

$$
\lvert f(x)-\ell\rvert<\varepsilon
$$

è equivalente a:

$$
\ell-\varepsilon<f(x)<\ell+\varepsilon.
$$

**$\varepsilon$** determina una **striscia orizzontale** attorno al valore del limite $\ell$; **$\delta$** delimita sull'asse delle $x$ un intorno di $x_0$. In quell'intorno (escluso $x_0$), i valori della funzione devono rimanere nella striscia.

### Grafici a due colonne

| Limiti di successioni | Limiti di funzioni |
| :--- | :--- |
| <img src="grafici/limite-successione.svg" alt="Punti della successione 1/n e soglia N=4; per n>4 sono nella striscia epsilon" width="420"> | <img src="grafici/limite-funzione.svg" alt="Retta f(x)=x, striscia epsilon e intorno delta attorno a zero" width="420"> |
| **Esempio:** $a_n=1/n$, $\ell=0$, $\varepsilon=1/4$, $N=4$. | **Esempio illustrativo:** $f(x)=x$, $x_0=\ell=0$, $\delta=\varepsilon=1/4$. |
| Per **tutti** gli interi $n>4$, i punti restano nella striscia. | Per **tutti** gli $x$ con $0<\lvert x\rvert<1/4$, il grafico resta nella striscia. |
| Grafico formato da **punti discreti**; troviamo una soglia **$N$**. | Grafico di una funzione sui reali; troviamo un intorno **$(x_0-\delta,x_0+\delta)$**. |

**Concetto comune:** fissiamo la tolleranza $\varepsilon$ attorno al limite; poi troviamo la condizione necessaria perché **tutti i valori richiesti** vi restino: $n>N$ oppure $0<\lvert x-x_0\rvert<\delta$.

**Nota sul grafico:** la pagina 25 usa la funzione **f(x) = x** per illustrare la definizione. L'esempio specifico della pagina 23 è invece **f(x) = x sin(1/x)**.

---

## 9. Tre esempi di limite in un punto — pagina 26

La slide mostra tre funzioni con $x\to0$ per chiarire un punto essenziale: **il limite descrive i valori vicino a $0$, non necessariamente il valore in $0$**.

### Esempi e parallelismo con le successioni

| Limiti di successioni — analogie | Limiti di funzioni — pagina 26 |
| :--- | :--- |
| **Costante:** $a_n=4$ per ogni $n$. Quindi $\lim_{n\to+\infty}a_n=4$. | **Costante:** $f(x)=4$ per ogni $x\in\mathbb{R}$. Quindi $\lim_{x\to0}f(x)=4$. |
| **Un termine diverso:** $a_1=7$ e $a_n=4$ per $n\ge2$. Quindi $\lim_{n\to+\infty}a_n=4$. | **Valore nel punto diverso:** $f(0)=7$ e $f(x)=4$ per $x\neq0$. Quindi $\lim_{x\to0}f(x)=4$. |
| **Quadrati:** $a_n=1/n^2$ e $a_n\to0$ quando $n\to+\infty$. | **Funzione quadratica:** $f(x)=x^2$ e $\lim_{x\to0}x^2=0$. |

### 9.1. Funzione costante

Per $f(x)=4$, vogliamo dimostrare che il limite è $\ell=4$:

$$
\lvert f(x)-4\rvert=\lvert4-4\rvert=0<\varepsilon.
$$

La condizione vale per **qualsiasi $\delta>0$**.

### 9.2. Funzione con un valore diverso in $x=0$

Poniamo $f(x)=4$ se $x\neq0$, ma $f(0)=7$.

Per ogni $x$ con $0<\lvert x\rvert<\delta$ abbiamo $x\neq0$, dunque:

$$
\lvert f(x)-4\rvert=0<\varepsilon.
$$

Quindi il limite è **$4$ e non $7$**: nella definizione di limite il punto $x=0$ è escluso. Analogamente, **modificare un numero finito di termini non cambia il limite di una successione**.

### 9.3. Funzione quadratica e scelta di delta

Per $f(x)=x^2$ vogliamo verificare:

$$
\lim_{x\to0}x^2=0.
$$

Fissiamo **$\varepsilon>0$**: è la tolleranza richiesta per i **valori della funzione**.

$$
\lvert f(x)-0\rvert=\lvert x^2\rvert=x^2<\varepsilon.
$$

Risolviamo questa disuguaglianza rispetto a $x$:

$$
x^2<\varepsilon
\quad\Longleftrightarrow\quad
\lvert x\rvert<\sqrt{\varepsilon}.
$$

La definizione di limite richiede invece una condizione sulla distanza di **$x$ da $0$**:

$$
0<\lvert x\rvert<\delta.
$$

Perciò possiamo **scegliere**:

$$
\delta=\sqrt{\varepsilon}.
$$

Allora, per ogni $x$ con $0<\lvert x\rvert<\delta$,

$$
\lvert f(x)-0\rvert=x^2<\delta^2=\varepsilon.
$$

### Perché compaiono sia epsilon sia delta?

| Successioni | Funzioni |
| :--- | :--- |
| **$\varepsilon$** è la tolleranza sui valori $a_n$; si ricava una soglia **$N$** sull'indice. | **$\varepsilon$** è la tolleranza sui valori $f(x)$; si ricava un raggio **$\delta$** per la distanza di $x$ da $x_0$. |
| Per $a_n=1/n^2$ basta $n>1/\sqrt{\varepsilon}$. | Per $f(x)=x^2$ basta $0<\lvert x\rvert<\sqrt{\varepsilon}$. |
| La scelta della soglia **dipende da $\varepsilon$**. | La scelta di **$\delta$ dipende da $\varepsilon$ e dalla funzione**. |

**Non stiamo scambiando $\varepsilon$ e $\delta$.** Prima scegliamo $\varepsilon$, poi troviamo un $\delta$ che garantisca quella tolleranza. Per $f(x)=x^2$ funziona $\delta=\sqrt{\varepsilon}$; per altre funzioni la scelta può essere diversa.

---

## 10. Funzioni continue — lezione 14/10, pagina 1 (slide 10/80)

Il **limite** descrive cosa succede ai valori $f(x)$ quando $x\to x_0$. La **continuità** collega il limite al valore **effettivo** della funzione nel punto $x_0$.

### Definizione

Sia $f:D\to\mathbb R$ e sia $x_0\in D$. La funzione è **continua in $x_0$** quando:

$$
\forall\varepsilon>0\quad\exists\delta>0
$$

tale che, per ogni $x\in D$,

$$
\lvert x-x_0\rvert<\delta
\quad\Longrightarrow\quad
\lvert f(x)-f(x_0)\rvert<\varepsilon.
$$

Quando **$x_0$ è punto di accumulazione di $D$**, questa definizione equivale a:

$$
\lim_{x\to x_0}f(x)=f(x_0).
$$

| Limiti di successioni — collegamento | Limiti di funzioni e continuità |
| :--- | :--- |
| Per $a_n\to\ell$, i termini si avvicinano al limite $\ell$ quando $n$ cresce. | Per $\lim_{x\to x_0}f(x)=\ell$, i valori si avvicinano a $\ell$ quando $x$ si avvicina a $x_0$. |
| Il limite di successione non deve coincidere con un termine della successione. | Per la **continuità** il valore $f(x_0)$ deve esistere e, se $x_0$ è di accumulazione, deve essere uguale a $\ell$. |
| Nella definizione di limite consideriamo $n>N$. | Nella definizione di continuità consideriamo $\lvert x-x_0\rvert<\delta$, **includendo il punto $x_0$**. |

### Esempi aggiuntivi

**Continuità di $f(x)=x^2$ in $x_0=2$:**

$$
f(2)=4,\qquad\lim_{x\to2}x^2=4.
$$

Il limite coincide con $f(2)$: la funzione è **continua in $2$**.

**Non continuità:** $f(0)=7$, mentre $f(x)=4$ per ogni $x\neq0$.

$$
\lim_{x\to0}f(x)=4\neq7=f(0).
$$

Il limite esiste, ma la funzione **non è continua in $0$**.

**Metodo negli esercizi (per un punto di accumulazione):** verifica che $f(x_0)$ sia definito; calcola il limite in $x_0$; confronta i due valori.

## 11. Continuità nei punti isolati — lezione 14/10, pagina 2 (appunti)

Gli appunti manoscritti illustrano un caso particolare: **ogni funzione è continua in un punto isolato del suo dominio**.

### Punto isolato

Un punto $x_0\in D$ è **isolato** se esiste un raggio $\delta>0$ per cui:

$$
(x_0-\delta,\ x_0+\delta)\cap D=\{x_0\}.
$$

Nell'intorno scelto, quindi, **non ci sono punti del dominio diversi da $x_0$**.

### Perché la continuità è automatica?

La continuità richiede che per tutti gli $x$ del dominio vicini a $x_0$ si abbia:

$$
\lvert f(x)-f(x_0)\rvert<\varepsilon.
$$

Ma se nell'intorno l'unico punto del dominio è $x_0$, l'unico caso da verificare è:

$$
\lvert f(x_0)-f(x_0)\rvert=0<\varepsilon.
$$

La disuguaglianza è vera **qualunque sia il valore $f(x_0)$**.

### Esempio aggiuntivo:

Consideriamo il dominio:

$$
D=\{0\}\cup[2,3].
$$

Vogliamo verificare se **$x_0=0$ è un punto isolato**.

1. **Il dominio resta sempre $D=\{0\}\cup[2,3]$.**
2. Per costruire un **intorno di $x_0=0$**, scegliamo ad esempio **$\delta=1$**:

$$
(x_0-\delta,\ x_0+\delta)=(-1,1).
$$

3. Calcoliamo **l'intersezione tra intorno e dominio**:

$$
(-1,1)\cap(\{0\}\cup[2,3])=\{0\}.
$$

L'intervallo $[2,3]$ fa parte del **dominio**; $(-1,1)$ è il **nuovo intorno di zero** scelto per la verifica. I due intervalli non hanno punti in comune, e il solo elemento del dominio dentro l'intorno è $0$.

Conclusione: **$0$ è isolato**; dunque ogni funzione $f:D\to\mathbb R$ è continua in $0$.

Il valore $\delta=1$ è una **scelta comoda, non obbligatoria**: basta scegliere un intorno abbastanza piccolo da non contenere il punto $2$.

### Parallelismo con le successioni

| Successioni | Funzioni |
| :--- | :--- |
| Una successione è una funzione $a:\mathbb N\to\mathbb R$ con $a(n)=a_n$. | Una funzione $f:D\to\mathbb R$ è continua automaticamente nei **punti isolati di $D$**. |
| Ogni $n\in\mathbb N$ è isolato: $(n-1/2,n+1/2)\cap\mathbb N=\{n\}$. | Quindi **ogni successione, vista come funzione su $\mathbb N$, è continua in ogni indice**, anche se non converge per $n\to+\infty$. |
| Il limite della successione riguarda il comportamento degli indici **all'infinito**. | In un punto isolato la continuità **non richiede di calcolare un limite nel punto**: quel limite non è definito secondo la definizione del corso. |

**Da ricordare:** un **punto di accumulazione** consente di avvicinarsi con altri punti del dominio; un **punto isolato** ha un intorno che non contiene altri punti del dominio.

---

*Prossima slide: limiti destro e sinistro (lezione 14/10, pagina 4, slide 11/80).*




