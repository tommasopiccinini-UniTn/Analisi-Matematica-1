# Derivate

Appunti di **Analisi Matematica 1** — lezioni del **21/10/2026** e **27/10/2026**, sezione **5.1: La derivata, definizione, prime proprietà ed esempi**.

> Sono raccolti **solo gli argomenti studiati finora** nella chat (slide 2–10 in `Lezione_20261021.pdf` e slide 11–12 in `Lezione_202621027.pdf`). I grafici qui sotto sono **schemi ricostruiti**, non scansioni delle slide originali.

## Indice

1. [Perché nasce la derivata — la retta tangente](#1-perché-nasce-la-derivata--la-retta-tangente)
2. [Definizione di derivata](#2-definizione-di-derivata)
3. [Rapporto incrementale](#3-rapporto-incrementale)
4. [Significato geometrico: dalla secante alla tangente](#4-significato-geometrico-dalla-secante-alla-tangente)
5. [Equazione della retta tangente](#5-equazione-della-retta-tangente)
6. [Riepilogo delle formule](#6-riepilogo-delle-formule)
7. [Retta tangente come migliore approssimante affine](#7-retta-tangente-come-migliore-approssimante-affine)
8. [Primi esempi: derivata di x² e retta tangente](#8-primi-esempi-derivata-di-x²-e-retta-tangente)
9. [Derivabilità e continuità](#9-derivabilità-e-continuità)
10. [Valore assoluto: continua ma non derivabile](#10-valore-assoluto-continua-ma-non-derivabile)
11. [Cuspidi e tangenti verticali](#11-cuspidi-e-tangenti-verticali)
12. [Funzione di Weierstrass: continua ovunque ma mai derivabile](#12-funzione-di-weierstrass-continua-ovunque-ma-mai-derivabile)
13. [Regole di derivazione — tabella sintetica](#13-regole-di-derivazione--tabella-sintetica)

## 1. Perché nasce la derivata — la retta tangente

**Slide 2/71, pagina 33.** Il calcolo differenziale nasce nel XVII secolo (Newton e Leibniz) anche per affrontare un problema geometrico: **determinare la retta tangente a una curva in un punto**.

![Curva blu e retta tangente rossa](../grafici/derivata-tangente.svg)

- **Curva blu:** grafico della funzione $f(x)$.
- **Punto P:** punto in cui cerchiamo la tangente.
- **Retta rossa:** tangente alla curva nel punto P, con la stessa **inclinazione locale**.
- La tangente **può anche attraversare** la curva: non deve necessariamente limitarsi a toccarla.

**Slide 3/71, pagina 34:** sommario della sezione; **slide 4/71, pagina 35:** titolo *La derivata: definizione, prime proprietà ed esempi*. Non introducono formule da memorizzare.

## 2. Definizione di derivata

**Slide 5/71, pagina 36.** Una funzione è **derivabile nel punto $x_0$** se esiste ed è **finito** il limite del rapporto incrementale:

$$
\boxed{f'(x_0)=\lim_{x\to x_0}\frac{f(x)-f(x_0)}{x-x_0}}
$$

Nel rapporto:

- $x_0$ è il **punto fissato** in cui vogliamo calcolare la derivata;
- $x$ è un punto che **si avvicina** a $x_0$;
- $f(x)-f(x_0)$ è la **variazione verticale** della funzione;
- $x-x_0$ è la **variazione orizzontale** della variabile indipendente.

Quando ci si avvicina a $x_0$ da entrambi i lati, i **limiti destro e sinistro del rapporto incrementale** devono coincidere e dare un valore finito.

## 3. Rapporto incrementale

Ponendo $h=x-x_0$, quindi $x=x_0+h$, la stessa definizione si scrive:

$$
\boxed{f'(x_0)=\lim_{h\to 0}\frac{f(x_0+h)-f(x_0)}{h}}
$$

Il rapporto incrementale, **prima di calcolare il limite**, è:

$$
\boxed{m_h=\frac{f(x_0+h)-f(x_0)}{h}},\qquad h\ne 0.
$$

Qui $h$ misura di quanto cambia l'ascissa rispetto a $x_0$.

## 4. Significato geometrico: dalla secante alla tangente

**Slide 6/71, pagina 38.** Consideriamo due punti del grafico:

$$
P=(x_0,f(x_0)),\qquad Q=(x_0+h,f(x_0+h)).
$$

La **secante** è la retta che passa per P e Q. Il suo coefficiente angolare è il rapporto incrementale:

$$
m_h=\frac{f(x_0+h)-f(x_0)}{h}.
$$

![Secante verde, tangente rossa, variazione h e variazione della funzione](../grafici/derivata-secante-tangente.svg)

- **Blu:** grafico di $f(x)$.
- **Verde:** secante per i due punti P e Q.
- **Rosso:** tangente in P.
- **$h$:** distanza orizzontale orientata da $x_0$ a $x_0+h$.
- **$\Delta f=f(x_0+h)-f(x_0)$:** variazione verticale.

Quando $h\to0$, Q si avvicina a P. **Se il limite del rapporto incrementale esiste ed è finito**, la pendenza della secante tende a quella della tangente:

$$
\boxed{m_{\mathrm{tangente}}=\lim_{h\to0}m_h=f'(x_0)}.
$$

**Idea da ricordare:** la derivata è il **coefficiente angolare della retta tangente**.

## 5. Equazione della retta tangente

L'equazione di una retta che passa per $(x_0,y_0)$ con coefficiente angolare $m$ è:

$$
y-y_0=m(x-x_0).
$$

Nel nostro caso $y_0=f(x_0)$ e $m=f'(x_0)$, quindi:

$$
\boxed{y=f(x_0)+f'(x_0)(x-x_0)}.
$$

Questa è **l'equazione della retta tangente al grafico** di $f$ nel punto di ascissa $x_0$.

## 6. Riepilogo delle formule

| Oggetto | Formula |
| --- | --- |
| Rapporto incrementale | $\displaystyle m_h=\frac{f(x_0+h)-f(x_0)}{h}$ |
| Derivata nel punto $x_0$ | $\displaystyle f'(x_0)=\lim_{h\to0}\frac{f(x_0+h)-f(x_0)}{h}$ |
| Derivata, forma con $x$ | $\displaystyle f'(x_0)=\lim_{x\to x_0}\frac{f(x)-f(x_0)}{x-x_0}$ |
| Pendenza della tangente | $m=f'(x_0)$ |
| Retta tangente | $y=f(x_0)+f'(x_0)(x-x_0)$ |

## 7. Retta tangente come migliore approssimante affine

**Slide 7/71 (pagina 39 del PDF).**

Una funzione **affine** è una funzione della forma

$
y=mx+q.
$

Fra tutte le rette che passano per $P_0=(x_0,f(x_0))$, se $f$ è derivabile in $x_0$, **la retta tangente è la migliore approssimante affine della funzione vicino a $x_0$**:

$
T(x)=f(x_0)+f'(x_0)(x-x_0).
$

Partiamo dalla definizione di derivata:

$
\lim_{x\to x_0}\frac{f(x)-f(x_0)}{x-x_0}=f'(x_0).
$

Sottrarre il limite $f'(x_0)$ equivale a scrivere

$
\lim_{x\to x_0}\left[\frac{f(x)-f(x_0)}{x-x_0}-f'(x_0)\right]=0.
$

Mettendo tutto sotto lo stesso denominatore:

$
\boxed{\lim_{x\to x_0}\frac{f(x)-[f(x_0)+f'(x_0)(x-x_0)]}{x-x_0}=0}.
$

Nel numeratore c'è l'**errore di approssimazione** $f(x)-T(x)$; al denominatore c'è $x-x_0$. Significa che l'errore tende a zero **più rapidamente** di $x-x_0$.

In forma compatta: $f(x)=T(x)+o(x-x_0)$ per $x\to x_0$.

## 8. Primi esempi: derivata di x² e retta tangente

**Slide 8/71 (pagina 40 del PDF).** La slide propone due esercizi sulla funzione $f(x)=x^2$.

### Esercizio 1 — derivata in $x_0=1$

Per definizione:

$
f'(1)=\lim_{x\to1}\frac{f(x)-f(1)}{x-1}
=\lim_{x\to1}\frac{x^2-1}{x-1}.
$

La sostituzione diretta dà la forma indeterminata $0/0$. Si usa la **differenza di quadrati**, non il raccoglimento di $x$:

$
x^2-1=(x-1)(x+1).
$

Quindi

$
f'(1)=\lim_{x\to1}\frac{(x-1)(x+1)}{x-1}
=\lim_{x\to1}(x+1)=\boxed{2}.
$

Dunque la tangente in $x_0=1$ ha **coefficiente angolare $m=f'(1)=2$**.

### Esercizio 2 — equazione della tangente nel punto $(1,1)$

La formula generale è

$
y=f(x_0)+f'(x_0)(x-x_0).
$

Per $f(x)=x^2$ e $x_0=1$:

- $f(1)=1^2=1$ si trova **sostituendo $x=1$ nella funzione**, senza calcolare alcuna derivata;
- $f'(1)=2$ è la **derivata**, trovata con il limite del rapporto incrementale.

L'equazione richiesta è

$
\boxed{y=1+2(x-1)}.
$

**Distinzione essenziale:** $f(1)$ è il valore della funzione nel punto, mentre $f'(1)$ è il coefficiente angolare della tangente in quel punto.

---

## 9. Derivabilità e continuità

**Slide 9, lezione 21 ottobre; ripresa nella slide 9/75 della lezione del 27 ottobre.**

**Teorema:** se una funzione è derivabile in un punto $x_0$, allora è continua in quel punto:

$
\boxed{f\text{ derivabile in }x_0\implies f\text{ continua in }x_0.}
$

**Idea della dimostrazione:** se $f$ è derivabile, il rapporto incrementale ha un limite finito $l=f'(x_0)$:

$
\lim_{x\to x_0}\frac{f(x)-f(x_0)}{x-x_0}=l.
$

Per $x\neq x_0$, possiamo scrivere:

$
f(x)-f(x_0)=\underbrace{\frac{f(x)-f(x_0)}{x-x_0}}_{\to l}\cdot
\underbrace{(x-x_0)}_{\to 0}.
$

Il primo fattore **è tutta la frazione**, non il denominatore da solo. Il secondo fattore tende a zero. Quindi

$
\lim_{x\to x_0}\big(f(x)-f(x_0)\big)=l\cdot 0=0,
$

ovvero $\lim_{x\to x_0}f(x)=f(x_0)$: è la definizione di continuità.

**Il contrario non è sempre vero:** una funzione può essere continua senza essere derivabile.

## 10. Valore assoluto: continua ma non derivabile

**Slide 10, ripresa nella slide 10/75 della lezione del 27 ottobre.**

La funzione $f(x)=|x|$ è continua in $0$:

$
\lim_{x\to0}|x|=0=f(0).
$

Ma nel punto $0$ ha uno **spigolo**. Il rapporto incrementale da sinistra e da destra dà risultati diversi:

$
f'_-(0)=\lim_{x\to0^-}\frac{|x|}{x}=-1,\qquad
f'_+(0)=\lim_{x\to0^+}\frac{|x|}{x}=+1.
$

Poiché i due limiti non coincidono, **non è derivabile in $0$**. Continuità significa assenza di salti; derivabilità richiede che la pendenza sia ben definita.

## 11. Cuspidi e tangenti verticali

**Slide 11/75, lezione del 27 ottobre (pagina 3 del PDF).** Mostra due ulteriori situazioni in cui una funzione può essere continua ma non derivabile.

- **Cuspide:** i rapporti incrementali da sinistra e destra tendono a infiniti di **segno opposto**. Un esempio è $f(x)=\sqrt{|x|}$ nel punto $0$:

$
\lim_{x\to0^-}\frac{\sqrt{|x|}}{x}=-\infty,\qquad
\lim_{x\to0^+}\frac{\sqrt{|x|}}{x}=+\infty.
$

- **Tangente verticale:** i rapporti incrementali tendono allo **stesso infinito**. Un esempio è $f(x)=\sqrt[3]{x}$ nel punto $0$:

$
\lim_{x\to0^-}\frac{\sqrt[3]{x}}{x}
=
\lim_{x\to0^+}\frac{\sqrt[3]{x}}{x}
=+\infty.
$

In entrambi i casi la **derivata ordinaria non esiste in $0$**, perché il limite del rapporto incrementale non è finito. Attenzione: anche nella cuspide i due rami hanno direzione verticale, ma le pendenze divergono con segni opposti.

**Distinzione importante:** può capitare che $f(x)\to0$ mentre il **rapporto incrementale** tende a $\pm\infty$. Il primo riguarda l'altezza del grafico, il secondo la sua inclinazione.

## 12. Funzione di Weierstrass: continua ovunque ma mai derivabile

**Slide 12/75, lezione del 27 ottobre (pagina 4 del PDF).**

Un caso particolarmente sorprendente è la **funzione di Weierstrass**, presentata nelle slide come

$
\boxed{f(x)=\sum_{n=0}^{+\infty}a^n\cos(b^n\pi x)}
$

con i parametri scelti in modo che

$
a\in(0,1),\qquad b\in\mathbb N\text{ dispari},\qquad
ab>1+\frac{3\pi}{2}.
$

**Proprietà:** la funzione è **continua in ogni punto**, ma **non è derivabile in alcun punto**.

**Intuizione:** i coseni introducono oscillazioni sempre più rapide (frequenze $b^n$), mentre le loro ampiezze diminuiscono (fattori $a^n$). Il grafico resta continuo, ma presenta irregolarità a ogni scala, senza una pendenza ben definita.

La slide presenta questo esempio per mostrare che **la continuità non garantisce la derivabilità, neppure in un singolo punto**. Non abbiamo affrontato la dimostrazione formale di questa proprietà.

---

## 13. Regole di derivazione — tabella sintetica

**Lezione del 27/10/2026, slide 14–18/75.** Formule viste fino alla regola di linearità; non sono ancora incluse le regole del prodotto e della catena.

| Regola | Funzione | Derivata | Condizioni |
| :--- | :--- | :--- | :--- |
| Costante | $f(x)=c$ | $\boxed{f'(x)=0}$ | $c\in\mathbb R$ |
| Potenza | $f(x)=x^n$ | $\boxed{f'(x)=nx^{n-1}}$ | $n\in\mathbb N^+$ |
| Reciproco | $f(x)=\dfrac{1}{x}=x^{-1}$ | $\boxed{f'(x)=-\dfrac{1}{x^2}}$ | $x\ne0$ |
| Esponenziale | $f(x)=e^x$ | $\boxed{f'(x)=e^x}$ | $x\in\mathbb R$ |
| Logaritmo naturale | $f(x)=\log x=\ln x$ | $\boxed{f'(x)=\dfrac{1}{x}}$ | $x>0$ |
| Seno | $f(x)=\sin x$ | $\boxed{f'(x)=\cos x}$ | $x$ in radianti |
| Coseno | $f(x)=\cos x$ | $\boxed{f'(x)=-\sin x}$ | $x$ in radianti |
| Linearità | $a f(x)+b g(x)$ | $\boxed{(af+bg)'=a f'+b g'}$ | $a,b$ costanti; $f,g$ derivabili |

**Notazione equivalente:** $f'(x)=D[f(x)]=\dfrac{d}{dx}f(x)$.

---

**Per proseguire:** slide 19/75 della lezione del 27 ottobre (regola del prodotto).
