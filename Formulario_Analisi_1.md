# Analisi 1 · Formulario

*Preliminari · Trigonometria · Limiti*

Formulario in Markdown basato su **Formulario_Analisi_1.pdf**, con integrazioni dalle lezioni e dagli altri formulari.

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

Per $A\subseteq\mathbb R$ non vuoto:

| Estremo | Caratterizzazione |
| :--- | :--- |
| **Minimo** | $m=\min A$ se e solo se $m\in A$ e $\forall x\in A:\ m\le x$. |
| **Massimo** | $M=\max A$ se e solo se $M\in A$ e $\forall x\in A:\ x\le M$. |
| **Superiore con $\varepsilon$** | $s=\sup A$ se e solo se $\forall x\in A:\ x\le s$ e $\forall\varepsilon>0\ \exists x\in A:\ s-\varepsilon<x$. |
| **Inferiore con $\varepsilon$** | $i=\inf A$ se e solo se $\forall x\in A:\ i\le x$ e $\forall\varepsilon>0\ \exists x\in A:\ x<i+\varepsilon$. |

Le caratterizzazioni con $\varepsilon$ valgono per estremi finiti. Se $\sup A\in A$, allora $\max A=\sup A$; se $\inf A\in A$, allora $\min A=\inf A$.

## 3 · Valore assoluto

**Attenzione:** $\sqrt{x^2}=\lvert x\rvert$.

## 3A · Algebra

**Prodotti notevoli e scomposizioni**

| Prodotto o metodo | Formula |
| :--- | :--- |
| Differenza di quadrati | $a^2-b^2=(a-b)(a+b)$. |
| Quadrato di un binomio | $(a\pm b)^2=a^2\pm2ab+b^2$. |
| Cubo di un binomio | $(a\pm b)^3=a^3\pm3a^2b+3ab^2\pm b^3$. |
| Somma e differenza di cubi | $a^3\pm b^3=(a\pm b)(a^2\mp ab+b^2)$. |
| Quadrato di un trinomio | $(a+b+c)^2=a^2+b^2+c^2+2ab+2ac+2bc$. |
| Differenza di potenze | $a^n-b^n=(a-b)\sum_{k=0}^{n-1}a^{n-1-k}b^k$, $n\ge1$ intero. Per $n$ dispari si ottiene la somma $a^n+b^n$ sostituendo $b$ con $-b$. |
| Raccoglimento totale / parziale | $ab+ac=a(b+c)$; $ax+ay+bx+by=(a+b)(x+y)$. |
| Trinomio di secondo grado | $x^2+(a+b)x+ab=(x+a)(x+b)$. In generale, se $P(r)=0$, allora $P(x)=(x-r)Q(x)$ per un polinomio $Q$. |

**Binomio di Newton** ($n\ge0$ intero)

| | |
| :--- | :--- |
| **Coefficiente binomiale:** $\displaystyle\binom nk=\frac{n!}{k!(n-k)!}$, $0\le k\le n$ | **Sviluppo:** $\displaystyle(a+b)^n=\sum_{k=0}^{n}\binom nk a^{n-k}b^k$ |
| **Simmetria:** $\binom nk=\binom n{n-k}$ | **Regola di Pascal:** $\binom nk=\binom{n-1}{k-1}+\binom{n-1}{k}$, $1\le k<n$ |

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
| **Cambio di base:** $\log_a x=\frac{\log_b x}{\log_b a}=\frac{\ln x}{\ln a}$ | | |
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
| $(1+u)^\alpha-1\sim\alpha u$, $\alpha\neq0$ | $\sqrt{1+u}-1\sim\frac u2$ | $\sqrt{1-u}-1\sim-\frac u2$ | $\arcsin u\sim u$ |
| $1-\cos^n(a u^m)\sim\frac{na^2}{2}u^{2m}$, $a\ne0$ e $n,m\ge1$ interi | | | |

| $x\to1$ | $x\to1$ | $x\to1$ | $x\to-1$ |
| :--- | :--- | :--- | :--- |
| $\ln x\sim x-1$ | $\ln(x^2)\sim2(x-1)$ | $x^2-1\sim2(x-1)$ | $\ln(x^2)\sim-2(x+1)$ |

| u → $\infty$ | u → $\infty$ | u → $-\infty$ |
| :--- | :--- | :--- |
| $\arctan u\sim\frac{\pi}{2}$ | $\ln(1+u)\sim\ln u$ | $\arctan u\sim-\frac{\pi}{2}$ |
| $e^u-1\sim e^u$ | $u+a\sim u$ ($a$ costante) | $\sqrt{u^2+1}\sim-u$ |
| $\sqrt{u^2+1}\sim u$ | $\log(1+a^x)\sim x\log a$ ($x\to+\infty,\ a>1$) | |

Per $x\to+\infty$ oppure $x\to-\infty$: $(1+1/x)^a-1\sim a/x$ se $a\ne0$, e $a^{1/x}\to1$ se $a>0$.

Con $u=1/x$, si ha $\arctan(1/x)\to\pi/2$ per $x\to0^+$ e $\arctan(1/x)\to-\pi/2$ per $x\to0^-$.

**Limiti notevoli per $u\to0$**:

| | | |
| :--- | :--- | :--- |
| $\displaystyle\lim_{u\to0}\frac{\sin u}{u}=1$ | $\displaystyle\lim_{u\to0}\frac{\tan u}{u}=1$ | $\displaystyle\lim_{u\to0}\frac{1-\cos u}{u^2}=\frac12$ |
| $\displaystyle\lim_{u\to0}\frac{\arcsin u}{u}=1$ | $\displaystyle\lim_{u\to0}\frac{\arctan u}{u}=1$ | $\displaystyle\lim_{u\to0}\frac{\sinh u}{u}=1$ |
| $\displaystyle\lim_{u\to0}\frac{\ln(1+u)}{u}=1$ | $\displaystyle\lim_{u\to0}\frac{\log_a(1+u)}{u}=\frac1{\ln a}$ | $\displaystyle\lim_{u\to0}\frac{u}{\log_a(1+u)}=\ln a$ |
| $\displaystyle\lim_{u\to0}\frac{e^u-1}{u}=1$ | $\displaystyle\lim_{u\to0}\frac{a^u-1}{u}=\ln a$ ($a>0$) | $\displaystyle\lim_{u\to0}\frac{(1+u)^\alpha-1}{u}=\alpha$ ($\alpha\in\mathbb R$) |
| $\displaystyle\lim_{u\to0}\frac{\sqrt{1+u}-1}{u}=\frac12$ | $\displaystyle\lim_{u\to0}\frac{\sin(au)}{bu}=\frac ab$ ($b\ne0$) | $\displaystyle\frac{\sin(3x)}x=3\frac{\sin(3x)}{3x}\to3$ ($x\to0$) |
| $\displaystyle\lim_{u\to0^+}\ln u=-\infty$ | | |

Per $\log_a$ si assume $a>0,\ a\ne1$.

**Limite di Nepero e varianti** (i parametri $a,b$ sono costanti reali)

| Avvicinamento | Limiti |
| :--- | :--- |
| $u\to0$ | $(1+u)^{1/u}\to e$; $\displaystyle(1+au)^{b/u}\to e^{ab}$ (in particolare $(1+au)^{1/u}\to e^a$). |
| $x\to+\infty$ oppure $x\to-\infty$ | $\displaystyle\left(1+\frac1x\right)^x\to e$; $\displaystyle\left(1+\frac ax\right)^{bx}\to e^{ab}$; $\displaystyle\left(\frac{x}{x+1}\right)^{bx}\to e^{-b}$. |
| $n\to+\infty$ | $\displaystyle\left(1+\frac1n\right)^n\to e$; $\displaystyle\left(1+\frac an\right)^n\to e^a$. |

**Definizione:** $f\sim g\iff f/g\to1$. **Cambio:** per $x\to a$, poni $u=x-a\to0$, quindi $x=a+u$.

| Condizione | NON fare | Corretto |
| :--- | :--- | :--- |
| $x\to+\infty,\ a>1$ | $\log(1+a^x)\sim a^x$ | $\log(1+a^x)\sim x\log a$ |
| $u\to0$ | $\sin u-u=u-u=0$ | $\sin u-u\sim-\frac{u^3}{6}$ |

## 5D · Regole dei limiti

| | |
| :--- | :--- |
| $\lim(f\pm g)=\lim f\pm\lim g$ | $\lim(fg)=(\lim f)(\lim g)$ |
| $\displaystyle\lim(f/g)=\frac{\lim f}{\lim g}$, $\lim g\neq0$ | $\lim[f(x)]^\alpha=(\lim f)^\alpha$ (se definita) |
| **Parte intera:** $\lfloor x\rfloor=\max\{n\in\mathbb Z:n\le x\}$ | **Proprietà:** $\lfloor x\rfloor\le x<\lfloor x\rfloor+1$ |

**Sottosuccessioni:** se due sottosuccessioni hanno limiti diversi, il limite della successione non esiste.

## 5E · Calcolo dei limiti di funzioni

**Continuità e potenze**

| $x>0$ | $x\to0^+$ | $x\to+\infty$ |
| :--- | :--- | :--- |
| $\alpha>0$ | $x^\alpha\to0$ | $x^\alpha\to+\infty$ |
| $\alpha<0$ | $x^\alpha\to+\infty$ | $x^\alpha\to0$ |

**Esponenziali e logaritmi**

| Base | $a^x$, $x\to+\infty$ | $a^x$, $x\to-\infty$ | $\log_a x$, $x\to0^+$ | $\log_a x$, $x\to+\infty$ |
| :--- | :---: | :---: | :---: | :---: |
| $a>1$ | $+\infty$ | $0$ | $-\infty$ | $+\infty$ |
| $0<a<1$ | $0$ | $+\infty$ | $+\infty$ | $-\infty$ |

**Trigonometria, polinomi e rapporti**

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

## 5G · Successioni

| Teorema o formula | Ipotesi e conclusione |
| :--- | :--- |
| **Confronto** | Se $a_n\le b_n$ da un certo indice in poi e i limiti esistono, allora $\lim a_n\le\lim b_n$. Inoltre $a_n\to+\infty\Rightarrow b_n\to+\infty$ e $b_n\to-\infty\Rightarrow a_n\to-\infty$. |
| **Due carabinieri** | Se $a_n\le c_n\le b_n$ da un certo indice in poi e $a_n,b_n\to L$, allora $c_n\to L$. |
| **Criterio del rapporto** | Se $a_n>0$ da un certo indice in poi e $\dfrac{a_{n+1}}{a_n}\to L$, allora $a_n\to0$ per $L<1$ e $a_n\to+\infty$ per $L>1$. Per $L=1$ il criterio non conclude. |
| **Successioni monotone** | Se $(a_n)$ è crescente, $\lim a_n=\sup_n a_n$ (finito se è limitata superiormente, altrimenti $+\infty$). Se è decrescente, $\lim a_n=\inf_n a_n$ (finito se è limitata inferiormente, altrimenti $-\infty$). |
| **Somma geometrica finita** | $\displaystyle\sum_{k=0}^{n}q^k=\frac{1-q^{n+1}}{1-q}$ per $q\neq1$; per $q=1$ la somma vale $n+1$. |

## 5H · Continuità e asintoti

**Discontinuità** (quando $x_0$ è raggiungibile da entrambi i lati del dominio)

| Tipo | Come riconoscerlo |
| :--- | :--- |
| **Eliminabile** | Esiste $L=\lim_{x\to x_0}f(x)\in\mathbb R$, ma $f(x_0)\ne L$ oppure $f(x_0)$ non è definita. Si ottiene la continuità ponendo $f(x_0)=L$. |
| **A salto** | I limiti $\lim_{x\to x_0^-}f(x)$ e $\lim_{x\to x_0^+}f(x)$ sono entrambi finiti e diversi. |
| **Essenziale** | Almeno uno dei due limiti laterali è infinito oppure non esiste. |

| Asintoto | Condizione |
| :--- | :--- |
| **Verticale** $x=x_0$ | Almeno uno tra $\lim_{x\to x_0^-}f(x)$ e $\lim_{x\to x_0^+}f(x)$ vale $+\infty$ o $-\infty$. |
| **Orizzontale** $y=L$ | $\lim_{x\to+\infty}f(x)=L$ oppure $\lim_{x\to-\infty}f(x)=L$, con $L\in\mathbb R$. I due versi possono dare rette diverse. |

| Teorema | Ipotesi e conclusione |
| :--- | :--- |
| **Valori intermedi** | Se $f$ è continua su $[a,b]$, per ogni $y$ compreso tra $f(a)$ e $f(b)$ esiste $c\in[a,b]$ con $f(c)=y$. Più in generale, l'immagine di un intervallo per una funzione continua è un intervallo. |
| **Weierstrass** | Se $f$ è continua su un intervallo chiuso e limitato $[a,b]$, esistono $x_m,x_M\in[a,b]$ tali che $f(x_m)=\min_{[a,b]}f$ e $f(x_M)=\max_{[a,b]}f$. |

## 6 · Trigonometria

**Conversioni tra gradi e radianti**

| Conversione | Formula |
| :--- | :--- |
| Radianti → gradi | $\theta_{\mathrm{gradi}}=\theta_{\mathrm{rad}}\cdot\frac{180}{\pi}$ |
| Gradi → radianti | $\theta_{\mathrm{rad}}=\theta_{\mathrm{gradi}}\cdot\frac{\pi}{180}$ |

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
| $\sin x\cos x=\frac12\sin2x$ | $\sin^2 x=\frac{1-\cos2x}{2}$ | $\cos^2 x=\frac{1+\cos2x}{2}$ |
| $\sin^2 x\cos^2 x=\frac14\sin^2(2x)$ | | |

La forma $\frac{\sin^2x}{1+\cos x}$ richiede $\cos x\neq-1$. Le formule con la tangente valgono dove tutti i termini sono definiti.

**Funzioni trigonometriche inverse**

| Arcoseno | Arcocoseno | Arcotangente |
| :--- | :--- | :--- |
| $\arcsin:[-1,1]\to[-\pi/2,\pi/2]$ | $\arccos:[-1,1]\to[0,\pi]$ | $\arctan(\tan x)=x$ per $x\in(-\pi/2,\pi/2)$ |
| $\arcsin(\sin x)=x$ per $x\in[-\pi/2,\pi/2]$ | $\arccos(\cos x)=x$ per $x\in[0,\pi]$ | |

**Equazioni trigonometriche** ($k\in\mathbb Z$)

| Equazione | Soluzioni e condizioni |
| :--- | :--- |
| $\sin x=a$ | $x=\arcsin a+2k\pi$ oppure $x=\pi-\arcsin a+2k\pi$, se $\lvert a\rvert\le1$. |
| $\cos x=a$ | $x=\pm\arccos a+2k\pi$, se $\lvert a\rvert\le1$. |
| $\tan x=a$ | $x=\arctan a+k\pi$, per ogni $a\in\mathbb R$. |
| $a\sin^2 x+b\sin x\cos x+c\cos^2 x=0$ | Se $\cos x\ne0$, dividi per $\cos^2 x$ e poni $t=\tan x$: $at^2+bt+c=0$. Controlla separatamente i punti con $\cos x=0$. |

## 6A · Numeri complessi — formule

| | | | |
| :--- | :--- | :--- | :--- |
| **Forma algebrica** | $z=x+iy,\ i^2=-1$ | $\mathrm{Re}\,z=x$ | $\mathrm{Im}\,z=y$ |
| **Coniugato e modulo** | $\bar z=x-iy,\ \lvert z\rvert=\sqrt{x^2+y^2}$ | $z\bar z=\lvert z\rvert^2$ | $\frac1z=\frac{\bar z}{\lvert z\rvert^2}$, $z\neq0$ |
| **Eulero** | $e^{i\theta}=\cos\theta+i\sin\theta$ | $z=re^{i\theta}=r(\cos\theta+i\sin\theta)$ | $r=\lvert z\rvert,\ x=r\cos\theta,\ y=r\sin\theta$ |
| **Operazioni** | $z_1\pm z_2=(x_1\pm x_2)+i(y_1\pm y_2)$ | $z_1z_2=r_1r_2e^{i(\theta_1+\theta_2)}$ | $\frac{z_1}{z_2}=\frac{r_1}{r_2}e^{i(\theta_1-\theta_2)}$, $z_2\neq0$ |
| **Potenze — De Moivre** | $z^n=r^ne^{in\theta}=r^n[\cos(n\theta)+i\sin(n\theta)]$ | $n\in\mathbb Z$ | $n<0\Rightarrow z\neq0$ |
| **Argomento** ($z\ne0$) | $\cos\theta=\frac{x}{\lvert z\rvert}$, $\sin\theta=\frac{y}{\lvert z\rvert}$ | Se $x,y\ne0$, $\alpha=\arctan(\lvert y/x\rvert)$: **I** $\theta=\alpha$; **II** $\theta=\pi-\alpha$; **III** $\theta=\pi+\alpha$; **IV** $\theta=2\pi-\alpha$. | Sugli assi usa la circonferenza della sezione 7. |

**Proprietà del coniugato, del modulo e dell'argomento**

| | |
| :--- | :--- |
| $\overline{z\pm w}=\bar z\pm\bar w$; $\overline{zw}=\bar z\,\bar w$ | $\overline{z/w}=\bar z/\bar w$ se $w\ne0$ |
| $\lvert\bar z\rvert=\lvert z\rvert$; $\lvert zw\rvert=\lvert z\rvert\lvert w\rvert$ | $\lvert z/w\rvert=\lvert z\rvert/\lvert w\rvert$ se $w\ne0$ |
| $\lvert z+w\rvert\le\lvert z\rvert+\lvert w\rvert$ | $\bigl\lvert\lvert z\rvert-\lvert w\rvert\bigr\rvert\le\lvert z-w\rvert$ |
| $\arg(zw)\equiv\arg z+\arg w\pmod{2\pi}$ | $\arg(z/w)\equiv\arg z-\arg w\pmod{2\pi}$ (in entrambe: $z,w\ne0$) |

**Radici di $z^n=w$**: se $w=\rho e^{i\varphi}$ con $\rho=\lvert w\rvert>0$ e $n\ge1$ è intero, poni $\beta_k=(\varphi+2k\pi)/n$, con $k=0,\ldots,n-1$.

| Forma esponenziale | Forma trigonometrica |
| :--- | :--- |
| $z_k=\rho^{1/n}e^{i\beta_k}$ | $z_k=\rho^{1/n}\bigl(\cos\beta_k+i\sin\beta_k\bigr)$ |

Se $w=0$, l'unica soluzione è $z=0$.

## 7 · Circonferenza goniometrica e arctan

<a href="grafici/circonferenza-formulario.svg"><img src="grafici/circonferenza-formulario.svg" alt="Circonferenza goniometrica con angoli notevoli" width="400"></a>

**Arctan notevoli**:

| | | | |
| :--- | :--- | :--- | :--- |
| $-\sqrt3\mapsto-\pi/3$ | $-1\mapsto-\pi/4$ | $-\sqrt3/3\mapsto-\pi/6$ | $0\mapsto0$ |
| $\sqrt3/3\mapsto\pi/6$ | $1\mapsto\pi/4$ | $\sqrt3\mapsto\pi/3$ | |

**Arco tangente:** $\arctan t\in(-\pi/2,\pi/2)$; $\displaystyle\lim_{x\to\pm\infty}\arctan x=\pm\frac\pi2$.

---
