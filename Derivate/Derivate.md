# Derivate

Appunti di **Analisi Matematica 1** — lezione del **21/10/2026**, sezione **5.1: La derivata, definizione, prime proprietà ed esempi**.

> Sono raccolti **solo gli argomenti studiati finora** nella chat (slide 2–6 della sezione, pagine 33–38 del PDF `Lezione_20261021.pdf`). I grafici qui sotto sono **schemi ricostruiti**, non scansioni delle slide originali.

## Indice

1. [Perché nasce la derivata — la retta tangente](#1-perché-nasce-la-derivata--la-retta-tangente)
2. [Definizione di derivata](#2-definizione-di-derivata)
3. [Rapporto incrementale](#3-rapporto-incrementale)
4. [Significato geometrico: dalla secante alla tangente](#4-significato-geometrico-dalla-secante-alla-tangente)
5. [Equazione della retta tangente](#5-equazione-della-retta-tangente)
6. [Riepilogo delle formule](#6-riepilogo-delle-formule)

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

**Per proseguire:** continuare dalla slide successiva alla 6/71, senza anticipare altri argomenti.
