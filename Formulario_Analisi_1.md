# Analisi 1 · Formulario

*Preliminari · Trigonometria · Limiti*

Trascrizione in Markdown delle due pagine di **Formulario_Analisi_1.pdf**. La numerazione delle sezioni è quella del PDF originale.

## 1 · Logica

- **Contronominale:** $(P\Rightarrow Q)\Leftrightarrow(\neg Q\Rightarrow\neg P)$.
- **Negazione dell'implicazione:** $\neg(P\Rightarrow Q)\Leftrightarrow P\land\neg Q$.
- **De Morgan:** $\neg(P\land Q)\Leftrightarrow\neg P\lor\neg Q$.
- **De Morgan:** $\neg(P\lor Q)\Leftrightarrow\neg P\land\neg Q$.
- **Negazione dei quantificatori:** $\neg(\forall x\,P(x))\Leftrightarrow\exists x\,\neg P(x)$; $\neg(\exists x\,P(x))\Leftrightarrow\forall x\,\neg P(x)$.

## 2 · Estremi e proprietà di R

- **Estremo superiore:** $\sup A=\min\{M\in\mathbb R:M\text{ maggiorante di }A\}$.
- **Estremo inferiore:** $\inf A=\max\{m\in\mathbb R:m\text{ minorante di }A\}$.
- **Archimede:** $\forall x\in\mathbb R\ \exists n\in\mathbb N:n>x$.
- **Conseguenza:** $\forall\varepsilon>0\ \exists n\in\mathbb N:1/n<\varepsilon$.
- **Densità di Q in R:** $a,b\in\mathbb R,\ a<b\Rightarrow\exists q\in\mathbb Q:a<q<b$.

## 3 · Valore assoluto

**Attenzione:**

$$
\sqrt{x^2}=\lvert x\rvert
$$

## 3A · De Moivre

$$
z=r(\cos\theta+i\sin\theta)
$$

$$
z^n=r^n[\cos(n\theta)+i\sin(n\theta)],\qquad n\in\mathbb Z
$$

Per $n<0$ occorre $z\neq0$.

## 4 · Funzioni

- **Iniettiva:** $\forall x_1,x_2\in A,\ x_1\neq x_2\Rightarrow f(x_1)\neq f(x_2)$.
- **Suriettiva:** $\forall y\in B\ \exists x\in A:f(x)=y$.
- **Composizione:** $(g\circ f)(x)=g(f(x))$.
- **Dominio della composizione:** $\mathrm{Dom}(g\circ f)=\{x\in\mathrm{Dom}\,f:f(x)\in\mathrm{Dom}\,g\}$.
- **Invertibile:** $f$ invertibile $\Leftrightarrow f$ biiettiva.
- **Inversa:** $f^{-1}(f(x))=x$; $f(f^{-1}(y))=y$.
- **Grafico dell'inversa:** riflesso del grafico di $f$ rispetto alla retta $y=x$.
- **Limitata:** $\exists M>0:\lvert f(x)\rvert\le M$ per ogni $x\in\mathrm{Dom}\,f$.
- **Pari:** $f(-x)=f(x)$; **dispari:** $f(-x)=-f(x)$.
- **Crescente:** $x_1<x_2\Rightarrow f(x_1)\le f(x_2)$.
- **Decrescente:** $x_1<x_2\Rightarrow f(x_1)\ge f(x_2)$.

Con le disuguaglianze strette si ottiene la **stretta monotonia**, che implica l'iniettività.

**Teorema degli zeri:**

$$
f\in C([a,b]),\quad f(a)f(b)<0\ \Rightarrow\ \exists c\in(a,b):f(c)=0
$$

## 5 · Funzioni elementari

**Retta** passante per $(x_0,y_0)$ con coefficiente angolare $m$:

$$
y-y_0=m(x-x_0)
$$

**Esponenziale:** $f(x)=a^x$, $a>0$, $a\neq1$.

- Dominio: $\mathbb R$; immagine: $(0,+\infty)$; $a^0=1$.
- $a>1$: crescente; $0<a<1$: decrescente.

**Logaritmo:** $\log_a x$, inversa di $a^x$.

- Dominio: $(0,+\infty)$; immagine: $\mathbb R$.
- $\log_a1=0$; $\log_a a=1$.

$$
\log_a(xy)=\log_a x+\log_a y
$$

$$
\log_a(x/y)=\log_a x-\log_a y
$$

$$
\log_a(x^r)=r\log_a x
$$

**Cambio di base:**

$$
\log_a x=\frac{\log_b x}{\log_b a}=\frac{\ln x}{\ln a}
$$

**Funzioni iperboliche:**

$$
\sinh x=\frac{e^x-e^{-x}}2,\qquad\cosh x=\frac{e^x+e^{-x}}2
$$

$$
\cosh^2x-\sinh^2x=1
$$

## 5A · Sviluppi notevoli — u → 0

$$
e^u=1+u+\frac{u^2}{2}+o(u^2)
$$

$$
\ln(1+u)=u-\frac{u^2}{2}+o(u^2)
$$

$$
\sin u=u-\frac{u^3}{6}+o(u^3)
$$

$$
\cos u=1-\frac{u^2}{2}+o(u^2)
$$

$$
(1+u)^\alpha=1+\alpha u+\frac{\alpha(\alpha-1)}2u^2+o(u^2)
$$

$$
\sqrt{1+u}=1+\frac u2+o(u)
$$

**Conta che l'argomento $u$ tenda a $0$.** Esempi: per $x\to a$ usa $u=x-a\to0$; per $x\to\infty$ usa $u=1/x\to0$.

## 5B · Equivalenti notevoli — u → 0

$$
\sin u\sim u;\qquad\tan u\sim u;\qquad\arctan u\sim u
$$

$$
1-\cos u\sim\frac{u^2}{2}\qquad\cos u-1\sim-\frac{u^2}{2}
$$

$$
\ln(1+u)\sim u;\qquad e^u-1\sim u
$$

$$
a^u-1\sim u\ln a,\qquad a>0,\ a\neq1
$$

$$
(1+u)^\alpha-1\sim\alpha u,\qquad\alpha\neq0
$$

$$
\sqrt{1+u}-1\sim\frac u2
$$

**Definizione:**

$$
f\sim g\ \Leftrightarrow\ \frac fg\to1
$$

Le equivalenze asintotiche si possono sostituire nei **prodotti e quozienti**. Nelle **somme e differenze** controllare le cancellazioni; se il primo termine si cancella, usare più termini dello sviluppo.

## 6 · Trigonometria

- $\sin:\mathbb R\to[-1,1]$ è dispari; $\cos:\mathbb R\to[-1,1]$ è pari.
- Periodo di seno e coseno: $2\pi$.
- $\tan x=\sin x/\cos x$; dominio $\mathbb R\setminus\{\pi/2+k\pi:k\in\mathbb Z\}$.
- $\cot x=\cos x/\sin x$; dominio $\mathbb R\setminus\{k\pi:k\in\mathbb Z\}$.
- Periodo di tangente e cotangente: $\pi$.

**Identità:**

$$
\sin^2x+\cos^2x=1
$$

$$
1+\tan^2x=\frac1{\cos^2x};\qquad1+\cot^2x=\frac1{\sin^2x}
$$

**Addizione e sottrazione:**

$$
\sin(x\pm y)=\sin x\cos y\pm\cos x\sin y
$$

$$
\cos(x\pm y)=\cos x\cos y\mp\sin x\sin y
$$

$$
\tan(x\pm y)=\frac{\tan x\pm\tan y}{1\mp\tan x\tan y}
$$

**Angolo doppio:**

$$
\sin2x=2\sin x\cos x
$$

$$
\cos2x=\cos^2x-\sin^2x=2\cos^2x-1=1-2\sin^2x
$$

$$
\tan2x=\frac{2\tan x}{1-\tan^2x}
$$

**Angolo metà:**

$$
\sin^2(x/2)=\frac{1-\cos x}2;\qquad
\cos^2(x/2)=\frac{1+\cos x}2
$$

**Funzioni trigonometriche inverse:**

$$
\arcsin:[-1,1]\to[-\pi/2,\pi/2]
$$

$$
\arccos:[-1,1]\to[0,\pi]
$$

$$
\arctan:\mathbb R\to(-\pi/2,\pi/2)
$$

$$
\arcsin(\sin x)=x\quad\text{per }x\in[-\pi/2,\pi/2]
$$

$$
\arccos(\cos x)=x\quad\text{per }x\in[0,\pi]
$$

$$
\arctan(\tan x)=x\quad\text{per }x\in(-\pi/2,\pi/2)
$$

## 6A · Numeri complessi — formule

**Forma algebrica:**

$$
z=x+iy,\quad i^2=-1,\quad\mathrm{Re}\,z=x,\quad\mathrm{Im}\,z=y
$$

**Coniugato e modulo:**

$$
\bar z=x-iy,\quad\lvert z\rvert=\sqrt{x^2+y^2}
$$

$$
z\bar z=\lvert z\rvert^2,\qquad
\frac1z=\frac{\bar z}{\lvert z\rvert^2}\quad(z\neq0)
$$

**Eulero:**

$$
e^{i\theta}=\cos\theta+i\sin\theta
$$

$$
z=re^{i\theta}=r(\cos\theta+i\sin\theta),\qquad r=\lvert z\rvert
$$

$$
x=r\cos\theta,\qquad y=r\sin\theta
$$

**Operazioni:**

$$
z_1\pm z_2=(x_1\pm x_2)+i(y_1\pm y_2)
$$

$$
z_1z_2=r_1r_2e^{i(\theta_1+\theta_2)}
$$

$$
\frac{z_1}{z_2}=\frac{r_1}{r_2}e^{i(\theta_1-\theta_2)},\qquad z_2\neq0
$$

**Potenza (z noto):**

$$
z^n=r^ne^{in\theta}
$$

**Radici di $z^n=w$**, con $w=\rho e^{i\varphi}$, $\rho=\lvert w\rvert>0$, $n\in\mathbb N$, $n\ge1$:

$$
z_k=\rho^{1/n}e^{i(\varphi+2k\pi)/n},\qquad k=0,\ldots,n-1
$$

Per scegliere $\theta$ (con $z\neq0$), usare il quadrante: sezione 7. Se $w=0$, l'unica soluzione è $z=0$.

## 7 · Circonferenza goniometrica e arctan

$$
P(\theta)=(\cos\theta,\sin\theta),\qquad r=1
$$

Angoli in senso antiorario.

![Circonferenza goniometrica con angoli notevoli](grafici/circonferenza-formulario.svg)

**Angoli notevoli:**

| Radianti | Gradi | Coordinate $(\cos\theta,\sin\theta)$ |
| :---: | :---: | :---: |
| $0,\ 2\pi$ | $0^\circ,\ 360^\circ$ | $(1,0)$ |
| $\pi/6$ | $30^\circ$ | $(\sqrt3/2,\ 1/2)$ |
| $\pi/4$ | $45^\circ$ | $(\sqrt2/2,\ \sqrt2/2)$ |
| $\pi/3$ | $60^\circ$ | $(1/2,\ \sqrt3/2)$ |
| $\pi/2$ | $90^\circ$ | $(0,1)$ |
| $2\pi/3$ | $120^\circ$ | $(-1/2,\ \sqrt3/2)$ |
| $3\pi/4$ | $135^\circ$ | $(-\sqrt2/2,\ \sqrt2/2)$ |
| $5\pi/6$ | $150^\circ$ | $(-\sqrt3/2,\ 1/2)$ |
| $\pi$ | $180^\circ$ | $(-1,0)$ |
| $7\pi/6$ | $210^\circ$ | $(-\sqrt3/2,\ -1/2)$ |
| $5\pi/4$ | $225^\circ$ | $(-\sqrt2/2,\ -\sqrt2/2)$ |
| $4\pi/3$ | $240^\circ$ | $(-1/2,\ -\sqrt3/2)$ |
| $3\pi/2$ | $270^\circ$ | $(0,-1)$ |
| $5\pi/3$ | $300^\circ$ | $(1/2,\ -\sqrt3/2)$ |
| $7\pi/4$ | $315^\circ$ | $(\sqrt2/2,\ -\sqrt2/2)$ |
| $11\pi/6$ | $330^\circ$ | $(\sqrt3/2,\ -1/2)$ |

**Arctan notevoli:**

| $t$ | $\arctan t$ |
| :---: | :---: |
| $-\sqrt3$ | $-\pi/3$ |
| $-1$ | $-\pi/4$ |
| $-\sqrt3/3$ | $-\pi/6$ |
| $0$ | $0$ |
| $\sqrt3/3$ | $\pi/6$ |
| $1$ | $\pi/4$ |
| $\sqrt3$ | $\pi/3$ |

$$
\arctan t\in(-\pi/2,\pi/2)
$$

Per l'angolo del punto $P(x,y)$, con $x\neq0$:

$$
\alpha=\arctan(\lvert y/x\rvert)
$$

| Quadrante | Angolo |
| :--- | :--- |
| I | $\theta=\alpha$ |
| II | $\theta=\pi-\alpha$ |
| III | $\theta=\pi+\alpha$ |
| IV | $\theta=2\pi-\alpha$ |

Sugli assi usare gli angoli della circonferenza.

## 8 · Regole dei limiti

$$
\lim(f\pm g)=\lim f\pm\lim g
$$

$$
\lim(fg)=(\lim f)(\lim g)
$$

$$
\lim(f/g)=\frac{\lim f}{\lim g},\qquad\lim g\neq0
$$

$$
\lim[f(x)]^\alpha=(\lim f)^\alpha\quad\text{(se definita)}
$$

## 9 · Forme indeterminate e procedura

**Forme:** $0/0$, $\infty/\infty$, $0\cdot\infty$, $\infty-\infty$, $1^\infty$, $0^0$, $\infty^0$.

**1. Sostituzione diretta.** Se la forma non è indeterminata, concludi.

**2. Se è indeterminata, scegli la trasformazione:**

| Forma | Procedura |
| :--- | :--- |
| $0/0$ | Fattorizza e semplifica i fattori comuni; usa limiti notevoli, equivalenti o sviluppi. Con le radici, razionalizza. |
| $\infty/\infty$ | Confronta gli ordini di crescita. Nei polinomi, dividi numeratore e denominatore per la potenza più alta presente. |
| $0\cdot\infty$ | Trasforma il prodotto in un quoziente. |
| $\infty-\infty$ | Raccogli il termine dominante, usa il denominatore comune oppure il coniugato delle radici. |
| $1^\infty,\ 0^0,\ \infty^0$ | Con base positiva, passa al logaritmo e studia il prodotto. |

**Prodotto trasformato in quoziente:**

$$
fg=\frac{f}{1/g}=\frac{g}{1/f}
$$

**Razionalizzazione:**

$$
\sqrt A-\sqrt B=\frac{A-B}{\sqrt A+\sqrt B}
$$

**Potenze indeterminate, base positiva:**

$$
f^g=e^{g\ln f};\qquad L=\lim(g\ln f)\Rightarrow\lim f^g=e^L
$$

**3. Controlla il dominio, il segno e i limiti laterali.**

## 10 · Limiti notevoli — u → 0

$$
\frac{\sin u}u\to1,\qquad\frac{\tan u}u\to1
$$

$$
\frac{1-\cos u}{u^2}\to\frac12
$$

$$
\frac{\ln(1+u)}u\to1
$$

$$
\frac{e^u-1}u\to1
$$

$$
\frac{(1+u)^\alpha-1}u\to\alpha
$$

$$
\frac{a^u-1}u\to\ln a,\qquad a>0
$$

$$
(1+1/n)^n\to e,\qquad n\to+\infty
$$

$$
(1+u)^{1/u}\to e,\qquad u\to0
$$

## 13 · Gerarchia di crescita — n → +∞

$$
\ln n\ll n^\alpha\ll a^n\ll n!\ll n^n,\qquad\alpha>0,\ a>1
$$

---

*Fonte: Formulario_Analisi_1.pdf, pagine 1–2. Circonferenza goniometrica riprodotta in SVG e coordinate trascritte anche in tabella.*
