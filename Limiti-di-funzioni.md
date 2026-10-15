# Limiti di funzioni

Appunti della **lezione del 12/10/2026**, confrontati con i **limiti di successioni** delle lezioni precedenti.

Le due colonne affiancano gli stessi concetti, **quando il parallelismo è corretto**. Le formule sono mantenute brevi per facilitare la lettura su GitHub.

## 1. Esempio introduttivo: teorema del confronto

| Limiti di successioni — lezione 07/10 | Limiti di funzioni — lezione 12/10, pagina 15 |
| :--- | :--- |
| Consideriamo $a_n=\frac{(-1)^n}{n}$. | Consideriamo $f(x)=x\sin\left(\frac{1}{x}\right)$, con $x\neq 0$. |
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

$
\boxed{\forall\delta>0\ \exists x\in D:\ 0<|x-x_0|<\delta.}
$

**Collegamento tramite successioni (conseguenza della definizione):** $x_0$ è di accumulazione per $D$ se e solo se esiste **una successione** $(x_n)$ di elementi di $D\setminus\{x_0\}$ tale che $x_n\to x_0$. Non è necessario che *ogni* successione di punti di $D$ converga a $x_0$.

## 4. Esempi di punti di accumulazione (pagina 21 del PDF)

### Esempio A: intervallo e punto isolato

$
A=(1,4]\cup\{6\},
\qquad \boxed{\operatorname{Acc}(A)=[1,4].}
$

| Successioni — parallelismo | Punti di accumulazione — spiegazione |
| :--- | :--- |
| $x_n=1+\frac1n\to1$, con $x_n\in A$ e $x_n\neq1$. | **$1$ è di accumulazione**, anche se $1\notin A$: i punti di $A$ si avvicinano a $1$ da destra. |
| $y_n=4-\frac1n\to4$, con $y_n\in A$ e $y_n\neq4$. | **$4$ è di accumulazione**: ci sono punti di $A$ arbitrariamente vicini a $4$ da sinistra. |
| Non può esistere una successione di punti di $A\setminus\{6\}$ che converga a $6$. | **$6$ è isolato**, perché $(5,7)\cap A=\{6\}$: togliendo il punto $6$, l'intorno non contiene altri punti di $A$. |
| Anche ogni $c\in(1,4)$ può essere avvicinato con punti distinti di $A$. | Tutti i punti tra $1$ e $4$ sono di accumulazione. |

### Esempio B: i reciproci dei naturali

$
B=\left\{\frac1n:n=1,2,3,\ldots\right\}.
$

| Successioni — parallelismo | Punti di accumulazione — spiegazione |
| :--- | :--- |
| $b_n=\frac1n\to0$. | **$0$ è di accumulazione**: esistono elementi di $B$ arbitrariamente vicini a $0$, anche se $0\notin B$. |
| Per ogni termine fissato $b_m=\frac1m$ ci sono un precedente e un successivo distinti, salvo il primo. | Ogni $\frac1m$ è un **punto isolato** di $B$: esiste un suo intorno abbastanza piccolo senza altri elementi di $B$. |
| Il limite della successione è $0$. | Il **solo** punto di accumulazione di $B$ è $0$: $\boxed{\operatorname{Acc}(B)=\{0\}}$. |

**Attenzione:** il fatto che la successione $1/n$ converga a $0$ non rende ogni suo termine un punto di accumulazione dell'insieme dei suoi valori.

## 5. Verifica con la definizione (pagina 22 del PDF)

La pagina dimostra che $0$ è di accumulazione per $B$ scegliendo un elemento $1/n$ sufficientemente vicino a $0$.

| Successioni — limite già conosciuto | Insieme $B$ — verifica del punto di accumulazione |
| :--- | :--- |
| $\frac1n\to0$: fissato $\varepsilon>0$, per **tutti** gli $n>1/\varepsilon$ vale $\lvert\frac1n-0\rvert<\varepsilon$. | Fissato $\delta>0$, basta **scegliere un** $n\in\mathbb N$, $n\ge1$, con $n>1/\delta$: allora $0<\frac1n<\delta$. |
| La condizione riguarda **tutti i termini da una certa soglia in poi**. | La definizione richiede **l'esistenza di un punto** di $B$ nell'intorno, diverso da $0$. |

Passaggi:

$
0<\frac1n<\delta
\quad\Longleftrightarrow\quad
n>\frac1\delta.
$

Per la proprietà di Archimede esiste sempre un naturale che supera $1/\delta$. Quindi

$
\boxed{0\in\operatorname{Acc}(B).}
$

**Perché gli altri punti sono isolati?** Per $m\ge2$ i due termini adiacenti a $1/m$ sono ordinati così:

$
\frac{1}{m+1}<\frac1m<\frac{1}{m-1}.
$

Possiamo scegliere un intorno sufficientemente piccolo di $1/m$ che non raggiunga i termini vicini (e quindi nessun altro punto di $B$). Anche $1$ è isolato.

---

*Prossimo argomento della lezione: definizione formale di limite finito di una funzione (pagina 24 del PDF).*

