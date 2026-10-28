# Analisi 1 · Formulario

*Preliminari · Trigonometria · Limiti*

Trascrizione in Markdown delle due pagine di **Formulario_Analisi_1.pdf**. La numerazione delle sezioni è quella del PDF originale.

## 1 · Logica

| | |
| :--- | :--- |
| **Contronominale:** $(P\Rightarrow Q)\Leftrightarrow(\neg Q\Rightarrow\neg P)$ | **Negazione implicazione:** $\neg(P\Rightarrow Q)\Leftrightarrow P\land\neg Q$ |
| **De Morgan:** $\neg(P\land Q)\Leftrightarrow\neg P\lor\neg Q$ | **De Morgan:** $\neg(P\lor Q)\Leftrightarrow\neg P\land\neg Q$ |
| **Quantificatori:** $\neg(\forall x\,P(x))\Leftrightarrow\exists x\,\neg P(x)$ | $\neg(\exists x\,P(x))\Leftrightarrow\forall x\,\neg P(x)$ |
## 2 · Estremi e proprietà di R

| | |
| :--- | :--- |
| **Estremo superiore:** $\sup A=\min\{M\in\mathbb R:M\text{ maggiorante di }A\}$ | **Estremo inferiore:** $\inf A=\max\{m\in\mathbb R:m\text{ minorante di }A\}$ |
| **Archimede:** $\forall x\in\mathbb R\ \exists n\in\mathbb N:n>x$ | **Conseguenza:** $\forall\varepsilon>0\ \exists n\in\mathbb N:1/n<\varepsilon$ |
| **Densità di $\mathbb Q$ in $\mathbb R$:** $a,b\in\mathbb R,\ a<b\Rightarrow\exists q\in\mathbb Q:a<q<b$ | |
## 3 · Valore assoluto

**Attenzione:** $\sqrt{x^2}=\lvert x\rvert$.
## 4 · Funzioni

| | |
| :--- | :--- |
| **Iniettiva:** $\forall x_1,x_2\in A,\ x_1\neq x_2\Rightarrow f(x_1)\neq f(x_2)$ | **Suriettiva:** $\forall y\in B\ \exists x\in A:f(x)=y$ |
| **Composizione:** $(g\circ f)(x)=g(f(x))$ | **Dominio:** $\mathrm{Dom}(g\circ f)=\{x\in\mathrm{Dom}\,f:f(x)\in\mathrm{Dom}\,g\}$ |
| **Invertibile:** $f$ invertibile $\Leftrightarrow f$ biiettiva | **Inversa:** $f^{-1}(f(x))=x;\ f(f^{-1}(y))=y$ |
| **Grafico dell'inversa:** riflesso rispetto a $y=x$ | **Limitata:** $\exists M>0:\lvert f(x)\rvert\le M$ per ogni $x\in\mathrm{Dom}\,f$ |
| **Pari / dispari:** $f(-x)=f(x)$ / $f(-x)=-f(x)$ | **Crescente / decrescente:** $x_1<x_2\Rightarrow f(x_1)\le f(x_2)$ / $f(x_1)\ge f(x_2)$ |
| **Stretta monotonia:** disuguaglianze strette $\Rightarrow$ iniettività | **Continuità a tratti:** $\lim_{x\to a^-}f(x)=\lim_{x\to a^+}f(x)=f(a)$ |
| **Teorema degli zeri:** $f\in C([a,b]),\ f(a)f(b)<0\Rightarrow\exists c\in(a,b):f(c)=0$ | |
## 5 · Funzioni elementari

| | | |
| :--- | :--- | :--- |
| **Retta:** $y-y_0=m(x-x_0)$ | **Esponenziale:** $a^x$, $a>0,\ a\neq1$ | **Logaritmo:** $\log_a x$, inversa di $a^x$ |
| **Esponenziale:** dominio $\mathbb R$, immagine $(0,+\infty)$, $a^0=1$ | $a>1$: crescente; $0<a<1$: decrescente | **Logaritmo:** dominio $(0,+\infty)$, immagine $\mathbb R$, $\log_a1=0$, $\log_a a=1$ |
| $\log_a(xy)=\log_a x+\log_a y$ | $\log_a(x/y)=\log_a x-\log_a y$ | $\log_a(x^r)=r\log_a x$ |
| **Cambio di base:** $\log_a x=\frac{\log_b x}{\log_b a}=\frac{\ln x}{\ln a}$ | $\displaystyle\lim_{x\to0^+}\ln x=-\infty$ | |
| **Iperboliche:** $\sinh x=\frac{e^x-e^{-x}}2$ | $\cosh x=\frac{e^x+e^{-x}}2$ | $\cosh^2x-\sinh^2x=1$ |
## 5 Limiti · Forme indeterminate e procedure

$\displaystyle\lim_{x\to+\infty}f(x)=L\iff\forall\varepsilon>0,\ \exists M>0:\ x>M\Rightarrow|f(x)-L|<\varepsilon$ (per $x$ nel dominio).

**1.** Sostituzione diretta; **2.** se indeterminata, scegli il metodo; **3.** controlla dominio, segni e limiti laterali.

| Forma | Procedura | Forma | Procedura |
| :--- | :--- | :--- | :--- |
| $0/0$ | Fattorizza, semplifica, razionalizza o usa equivalenti/sviluppi | $\infty/\infty$ | Confronta crescite; dividi per il termine dominante |
| $0\cdot\infty$ | Trasforma in un quoziente | $\infty-\infty$ | Raccogli, denominatore comune o coniugato |
| $1^\infty$ | Base positiva: usa $e^{g\ln f}$ | $0^0,\ \infty^0$ | Base positiva: usa $e^{g\ln f}$ |

| **Polinomi** | **Prodotto / quoziente** | **Razionalizzazione** | **Potenze indeterminate** |
| :--- | :--- | :--- | :--- |
| $x\to\infty$: potenza maggiore; $x\to0$: potenza minore | $fg=\frac{f}{1/g}=\frac{g}{1/f}$ | $\sqrt A-\sqrt B=\frac{A-B}{\sqrt A+\sqrt B}$ | $f^g=e^{g\ln f}$; se $L=\lim(g\ln f)$, allora $\lim f^g=e^L$ |

**Promemoria $1^\infty$:** scrivi la base come $1+u$ ($u\to0$); poi $\ln(1+u)\sim u$. **Quozienti per $x\to\pm\infty$:** conviene dividere sopra e sotto per il termine dominante del denominatore; verifica prima le cancellazioni.
## 5B · Sviluppi notevoli — u → 0

| | | |
| :--- | :--- | :--- |
| $e^u=1+u+\frac{u^2}{2}+o(u^2)$ | $a^u=1+u\ln a+o(u)$, $a>0$ | $2^u=1+u\ln2+o(u)$ |
| $\ln(1+u)=u-\frac{u^2}{2}+o(u^2)$ | $\sin u=u-\frac{u^3}{6}+o(u^3)$ | $\sinh u=u+\frac{u^3}{6}+o(u^3)$ |
| $\cos u=1-\frac{u^2}{2}+o(u^2)$ | $\tan u=u+\frac{u^3}{3}+o(u^3)$ | $\sqrt{1+u}=1+\frac u2+o(u)$ |
| $\arccos u=\frac{\pi}{2}-u-\frac{u^3}{6}+o(u^3)$ | $(1+u)^\alpha=1+\alpha u+\frac{\alpha(\alpha-1)}2u^2+o(u^2)$ | |

**Conta che l'argomento $u$ tenda a $0$.** Esempi: per $x\to a$ usa $u=x-a\to0$; per $x\to\infty$ usa $u=1/x\to0$.

## 5C · Equivalenze asintotiche

|u → 0| | | |
| :--- | :--- | :--- | :--- |
| $\sin u\sim u$ | $\sinh u\sim u$ | $\tan u\sim u$ | $\arctan u\sim u$ |
| $1-\cos u\sim\frac{u^2}{2}$ | $\cos u-1\sim-\frac{u^2}{2}$ | $\ln(1+u)\sim u$ | $\ln(1-u)\sim-u$ |
| $\ln(\cos u)\sim-\frac{u^2}{2}$ | $\arccos u-\frac{\pi}{2}\sim-u$ | $e^u-1\sim u$ | $a^u-1\sim u\ln a$, $a>0,\ a\neq1$ |
| $(1+u)^\alpha-1\sim\alpha u$, $\alpha\neq0$ | $\sqrt{1+u}-1\sim\frac u2$ | $\sqrt{1-u}-1\sim-\frac u2$ |$x\to0^+\Rightarrow u=1/x\to+\infty\Rightarrow\arctan(1/x)\sim\frac{\pi}{2}$.|
|$\log(1+a^x)\sim x\log a$| | | |

| x → 1 | x → 1 | x → -1 |
| :--- | :--- | :--- |
| $\ln x\sim x-1$ | $\ln(x^2)\sim2(x-1)$ | $\ln(x^2)\sim-2(x+1)$ |

**Limiti notevoli**:

| | | |
| :--- | :--- | :--- |
| $\displaystyle\lim_{u\to0}\frac{\sin u}{u}=1$ | $\displaystyle\lim_{u\to0}\frac{\sinh u}{u}=1$ | $\displaystyle\lim_{u\to0}\frac{\sqrt{1+u}-1}{u}=\frac12$ |
| $\displaystyle\lim_{u\to0}(1+u)^{1/u}=e$ | $\displaystyle\lim_{n\to+\infty}\left(1+\frac1n\right)^n=e$ | $\displaystyle\frac{\sin(3x)}x=3\frac{\sin(3x)}{3x}\to3$ ($x\to0$) |
| $\displaystyle\lim_{n\to+\infty}\left(1+\frac{a}{n}\right)^n=e^a$, $a\in\mathbb R$ costante | | |

**Definizione:** $f\sim g\iff f/g\to1$. **Cambio:** per $x\to a$, poni $u=x-a\to0$, quindi $x=a+u$.

| Condizione | NON fare | Corretto |
| :--- | :--- | :--- |
| $x\to+\infty,\ a>1$ | $\log(1+a^x)\sim a^x$ | $\log(1+a^x)\sim x\log a$ |
| $u\to0$ | $\sin u-u=u-u=0$ | $\sin u-u\sim-\frac{u^3}{6}$ |

## 5C-bis · Equivalenze asintotiche — u → ±∞

| u → $\infty$ | u → $\infty$ | u → $-\infty$ |
| :--- | :--- | :--- |
| $\arctan u\sim\frac{\pi}{2}$ | $\ln(1+u)\sim\ln u$ | $\arctan u\sim-\frac{\pi}{2}$ |
| $e^u-1\sim e^u$ | $u+a\sim u$ ($a$ costante) | $\sqrt{u^2+1}\sim-u$ |
| $\sqrt{u^2+1}\sim u$ | $\log(1+a^x)\sim x\log a$ ($x\to+\infty,\ a>1$) | |

## 5D · Regole dei limiti

| | |
| :--- | :--- |
| $\lim(f\pm g)=\lim f\pm\lim g$ | $\lim(fg)=(\lim f)(\lim g)$ |
| $\displaystyle\lim(f/g)=\frac{\lim f}{\lim g}$, $\lim g\neq0$ | $\lim[f(x)]^\alpha=(\lim f)^\alpha$ (se definita) |
| **Parte intera:** $\lfloor x\rfloor=\max\{n\in\mathbb Z:n\le x\}$ | **Proprietà:** $\lfloor x\rfloor\le x<\lfloor x\rfloor+1$ |

**Sottosuccessioni:** se due sottosuccessioni hanno limiti diversi, il limite della successione non esiste.

## 5E · Calcolo dei limiti di funzioni

**Continuità e potenze (slide 35–36)**

| $x>0$ | $x\to0^+$ | $x\to+\infty$ |
| :--- | :--- | :--- |
| $\alpha>0$ | $x^\alpha\to0$ | $x^\alpha\to+\infty$ |
| $\alpha<0$ | $x^\alpha\to+\infty$ | $x^\alpha\to0$ |

**Esponenziali e logaritmi (slide 37)**

| Base | $a^x$, $x\to+\infty$ | $a^x$, $x\to-\infty$ | $\log_a x$, $x\to0^+$ | $\log_a x$, $x\to+\infty$ |
| :--- | :---: | :---: | :---: | :---: |
| $a>1$ | $+\infty$ | $0$ | $-\infty$ | $+\infty$ |
| $0<a<1$ | $0$ | $+\infty$ | $+\infty$ | $-\infty$ |

**Trigonometria, polinomi e rapporti (slide 38–40)**

| Trigonometria | Polinomi | Rapporti $P/Q$ |
| :--- | :--- | :--- |
| $\sin,\cos$ continue; $\tan$ continua se $\cos x\neq0$ | $x\to x_0$: sostituisci; $x\to\pm\infty$: $P(x)=a_nx^n+\cdots+a_0\sim a_nx^n$ | $\frac{P(x)}{Q(x)}\sim\frac{a_m}{b_n}x^{m-n}$, $x\to\pm\infty$; $m,n$ gradi, $a_m,b_n\neq0$ |
| $\displaystyle\lim_{x\to(\pi/2)^-}\tan x=+\infty$; $\displaystyle\lim_{x\to(-\pi/2)^+}\tan x=-\infty$ | | $m<n\Rightarrow0$; $m=n\Rightarrow a_m/b_n$; $m>n\Rightarrow$ infinito (controlla il segno) |

**Forma $1/0$:** **non indeterminata**; con numeratore non nullo studia il segno del denominatore e i limiti laterali.

| | | |
| :--- | :--- | :--- |
| $\displaystyle\lim_{x\to3}\frac1{(x-3)^4}=+\infty$ | $\displaystyle\lim_{x\to3^-}\frac1{(x-3)^3}=-\infty$ | $\displaystyle\lim_{x\to3^+}\frac1{(x-3)^3}=+\infty$ |

**Funzioni limitate:** se $\lvert g(x)\rvert\le M$ e $f(x)\to0$, allora $f(x)g(x)\to0$; esempio $\displaystyle\lim_{x\to0}x\sin\frac1x=0$.

## 5F · Cambio di variabile nei limiti

Se $f(x)\to y_0$ e $g$ è continua in $y_0$ (finito), O $g$ ammette lim per $y\to y_0$ ($y_0=\pm\infty$), allora $\displaystyle\lim_{x\to x_0}g(f(x))=\lim_{y\to y_0}g(y)$.

**Procedura:** poni $y=f(x)$, determina $y\to y_0$ e calcola il limite di $g(y)$.

| | | |
| :--- | :--- | :--- |
| $\displaystyle\lim_{x\to0^+}e^{1/x}=+\infty$ | $\displaystyle\lim_{x\to0^-}e^{1/x}=0$ | $\displaystyle\lim_{x\to+\infty}e^{1/x}=1$ |
| $\displaystyle\lim_{x\to1^+}\arctan\frac1{x-1}=\frac\pi2$ | $\displaystyle\lim_{x\to+\infty}\log\left(\sin\frac1x\right)=-\infty$ | |

**Trucco $t=1/x$ :** $t=\frac1x\Leftrightarrow x=\frac1t$. Utile per trasformare i limiti vicino a $0$ in limiti all'infinito (e viceversa).

| $x\to0^+$ | $x\to0^-$ | $x\to+\infty$ | $x\to-\infty$ |
| :--- | :--- | :--- | :--- |
| $t\to+\infty$ | $t\to-\infty$ | $t\to0^+$ | $t\to0^-$ |

| Confronto delle crescite ($x\to0^+$, $\alpha>0$) | Potenza indeterminata ($x\to0^+$) |
| :--- | :--- |
| $x^\alpha\log x=-\frac{\log t}{t^\alpha}\to0$ per $t=1/x\to+\infty$ | $\displaystyle\lim_{x\to0^+}x^x=\lim_{x\to0^+}e^{x\ln x}=e^0=1$ |

## 6 · Trigonometria

**Conversioni:** $\pi$ $\to $ grad : $\theta_{^\circ}=\theta_{\mathrm{rad}}\frac{180}{\pi}$; grad $\to \pi$ : $\theta_{\mathrm{rad}}=\theta_{^\circ}\frac{\pi}{180}$.

**Proprietà e domini**

| Seno e coseno | Tangente | Cotangente |
| :--- | :--- | :--- |
| $\sin:\mathbb R\to[-1,1]$ dispari; $\cos:\mathbb R\to[-1,1]$ pari | $\tan x=\frac{\sin x}{\cos x}$ | $\cot x=\frac{\cos x}{\sin x}$ |
| Periodo $2\pi$ | Dom: $\mathbb R\setminus\{\pi/2+k\pi:k\in\mathbb Z\}$; periodo $\pi$ | Dom: $\mathbb R\setminus\{k\pi:k\in\mathbb Z\}$; periodo $\pi$ |

**Identità e formule**

| | | |
| :--- | :--- | :--- |
| $\sin^2x+\cos^2x=1$ | $1+\tan^2x=\frac1{\cos^2x}$ | $1+\cot^2x=\frac1{\sin^2x}$ |
| $1-\cos x=\frac{\sin^2x}{1+\cos x}=2\sin^2\left(\frac x2\right)$ | $\sin(x\pm y)=\sin x\cos y\pm\cos x\sin y$ | $\cos(x\pm y)=\cos x\cos y\mp\sin x\sin y$ |
| $\tan(x\pm y)=\frac{\tan x\pm\tan y}{1\mp\tan x\tan y}$ | $\sin2x=2\sin x\cos x$ | $\cos2x=\cos^2x-\sin^2x=2\cos^2x-1=1-2\sin^2x$ |
| $\tan2x=\frac{2\tan x}{1-\tan^2x}$ | $\sin^2(x/2)=\frac{1-\cos x}{2}$ | $\cos^2(x/2)=\frac{1+\cos x}{2}$ |

La forma $\frac{\sin^2x}{1+\cos x}$ richiede $\cos x\neq-1$.

**Funzioni trigonometriche inverse**

| Arcoseno | Arcocoseno | Arcotangente |
| :--- | :--- | :--- |
| $\arcsin:[-1,1]\to[-\pi/2,\pi/2]$ | $\arccos:[-1,1]\to[0,\pi]$ | $\arctan(\tan x)=x$ per $x\in(-\pi/2,\pi/2)$ |
| $\arcsin(\sin x)=x$ per $x\in[-\pi/2,\pi/2]$ | $\arccos(\cos x)=x$ per $x\in[0,\pi]$ | |

## 6A · Numeri complessi — formule

| | | | |
| :--- | :--- | :--- | :--- |
| **Forma algebrica** | $z=x+iy,\ i^2=-1$ | $\mathrm{Re}\,z=x$ | $\mathrm{Im}\,z=y$ |
| **Coniugato e modulo** | $\bar z=x-iy,\ \lvert z\rvert=\sqrt{x^2+y^2}$ | $z\bar z=\lvert z\rvert^2$ | $\frac1z=\frac{\bar z}{\lvert z\rvert^2}$, $z\neq0$ |
| **Eulero** | $e^{i\theta}=\cos\theta+i\sin\theta$ | $z=re^{i\theta}=r(\cos\theta+i\sin\theta)$ | $r=\lvert z\rvert,\ x=r\cos\theta,\ y=r\sin\theta$ |
| **Operazioni** | $z_1\pm z_2=(x_1\pm x_2)+i(y_1\pm y_2)$ | $z_1z_2=r_1r_2e^{i(\theta_1+\theta_2)}$ | $\frac{z_1}{z_2}=\frac{r_1}{r_2}e^{i(\theta_1-\theta_2)}$, $z_2\neq0$ |
| **Potenze — De Moivre** | $z^n=r^ne^{in\theta}=r^n[\cos(n\theta)+i\sin(n\theta)]$ | $n\in\mathbb Z$ | $n<0\Rightarrow z\neq0$ |
| **Radici di $z^n=w$** | $z_k=\rho^{1/n}e^{i(\varphi+2k\pi)/n}$ | $w=\rho e^{i\varphi},\ \rho=\lvert w\rvert>0$ | $n\in\mathbb N,\ n\ge1;\ k=0,\ldots,n-1$ |
| **Argomento:** | $\cos\theta=\frac{a}{\lvert z\rvert}$, $\sin\theta=\frac{b}{\lvert z\rvert}$ |$x\neq0$ => $\alpha=\arctan(\lvert y/x\rvert)$ e scegli quadrante. <br> **I:** $\theta=\alpha$; **II:** $\theta=\pi-\alpha$; **III:** $\theta=\pi+\alpha$; **IV:** $\theta=2\pi-\alpha$ | |

## 7 · Circonferenza goniometrica e arctan

![Circonferenza goniometrica con angoli notevoli](grafici/circonferenza-formulario.svg)

**Arctan notevoli**:

| | | | |
| :--- | :--- | :--- | :--- |
| $-\sqrt3\mapsto-\pi/3$ | $-1\mapsto-\pi/4$ | $-\sqrt3/3\mapsto-\pi/6$ | $0\mapsto0$ |
| $\sqrt3/3\mapsto\pi/6$ | $1\mapsto\pi/4$ | $\sqrt3\mapsto\pi/3$ | |

**Arco tangente:** $\arctan t\in(-\pi/2,\pi/2)$; $\displaystyle\lim_{x\to\pm\infty}\arctan x=\pm\frac\pi2$.

---
