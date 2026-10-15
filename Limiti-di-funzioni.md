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

*Prossimo argomento della lezione: punti di accumulazione (pagina 19 del PDF).*
