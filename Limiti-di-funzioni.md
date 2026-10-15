# Limiti di funzioni

Appunti di **Analisi matematica 1** basati sulla lezione del **12 ottobre 2026** (`Lezione_20261012.pdf`).

## 1. Esempio introduttivo (pagina 15 del PDF)

Consideriamo la funzione

$$
f(x)=x\sin\left(\frac{1}{x}\right),
\qquad D=\mathbb{R}\setminus\{0\}.
$$

Vogliamo studiare il comportamento di \(f(x)\) quando \(x\to 0\).

Poiché il seno assume sempre valori compresi tra \(-1\) e \(1\), abbiamo

$$
\left|\sin\left(\frac{1}{x}\right)\right|\leq 1.
$$

Moltiplicando entrambi i membri per \(|x|\), otteniamo

$$
\left|x\sin\left(\frac{1}{x}\right)\right|\leq |x|,
$$

ossia

$$
-|x|\leq x\sin\left(\frac{1}{x}\right)\leq |x|.
$$

Dato che

$$
\lim_{x\to 0}(-|x|)=\lim_{x\to 0}|x|=0,
$$

**per il teorema del confronto** concludiamo che

$$
\boxed{\lim_{x\to 0}x\sin\left(\frac{1}{x}\right)=0}.
$$

**Osservazione:** una funzione può ammettere limite in un punto anche quando non è definita in quel punto. Qui \(f(0)\) non esiste, ma il limite per \(x\to 0\) esiste ed è uguale a zero.

## 2. Intorni (pagina 18 del PDF)

Per definire il limite di una funzione dobbiamo precisare matematicamente cosa significa che \(x\) è **vicino** a un punto fissato \(x_0\).

### Intorno di un punto reale

Dato \(x_0\in\mathbb{R}\) e un raggio \(r>0\), l'**intorno di \(x_0\) di raggio \(r\)** è l'intervallo aperto

$$
\boxed{(x_0-r,\ x_0+r)=\{x\in\mathbb{R}:|x-x_0|<r\}}.
$$

In altre parole, contiene i punti che distano da \(x_0\) meno di \(r\), **esclusi gli estremi** dell'intervallo.

**Esempio:** se \(x_0=3\) e \(r=0{,}5\), l'intorno è

$$
(3-0{,}5,\ 3+0{,}5)=(2{,}5,\ 3{,}5).
$$

### Intorni di infinito

- Un **intorno di \(+\infty\)** è un qualunque intervallo della forma \((a,+\infty)\), con \(a\in\mathbb{R}\).
- Un **intorno di \(-\infty\)** è un qualunque intervallo della forma \(( -\infty,a)\), con \(a\in\mathbb{R}\).

**Da ricordare:** per gli intorni di un punto reale il raggio \(r\) può essere piccolo quanto si vuole, purché \(r>0\). Per \(\pm\infty\), invece, gli intorni sono semirette.

---

*Prossimo argomento della lezione: punti di accumulazione (pagina 19 del PDF).*
