# Formulario delle derivate

Formulario sintetico di definizioni, derivate note, regole operative e teoremi principali.

## Definizioni fondamentali

| Oggetto | Formula | Condizioni / significato |
| --- | --- | --- |
| Derivata in $x_0$ | $\displaystyle f'(x_0)=\lim_{x\to x_0}\frac{f(x)-f(x_0)}{x-x_0}$ | Il limite deve esistere ed essere finito |
| Derivata con incremento $h$ | $\displaystyle f'(x_0)=\lim_{h\to0}\frac{f(x_0+h)-f(x_0)}{h}$ | $h\neq0$ prima del limite |
| Derivate laterali | $f'_+(x_0)=\lim_{h\to 0^+}\frac{f(x_0+h)-f(x_0)}{h}$; $f'_-(x_0)=\lim_{h\to 0^-}\frac{f(x_0+h)-f(x_0)}{h}$ | $f'(x_0)$ esiste se coincidono e sono finite |
| Retta tangente | $\displaystyle y=f(x_0)+f'(x_0)(x-x_0)$ | $f'(x_0)$ è la pendenza |
| Approssimazione lineare | $\displaystyle f(x)=f(x_0)+f'(x_0)(x-x_0)+o(x-x_0)$ | Per $x\to x_0$ |
| Derivabilità e continuità | $f\text{ derivabile in }x_0\Rightarrow f\text{ continua in }x_0$ | Il contrario non vale sempre |

## Derivate note

| Funzione | Derivata | Condizioni | Funzione | Derivata | Condizioni |
| --- | --- | --- | --- | --- | --- |
| $c$ | $0$ | $c\in\mathbb R$ | $x$ | $1$ | $x\in\mathbb R$ |
| $x^\alpha$ | $\alpha x^{\alpha-1}$ | In generale $x>0$ | $\sqrt{x}$ | $\displaystyle\frac1{2\sqrt{x}}$ | $x>0$ |
| $\displaystyle\frac1x$ | $\displaystyle-\frac1{x^2}$ | $x\neq0$ | $\ln\lvert x\rvert$ | $\displaystyle\frac1x$ | $x\neq0$ |
| $e^x$ | $e^x$ | $x\in\mathbb R$ | $a^x$ | $a^x\ln a$ | $a>0$ |
| $\ln x$ | $\displaystyle\frac1x$ | $x>0$ | $\log_a x$ | $\displaystyle\frac1{x\ln a}$ | $x>0,\ a>0,\ a\neq1$ |
| $\sin x$ | $\cos x$ | $x\in\mathbb R$ | $\cos x$ | $-\sin x$ | $x\in\mathbb R$ |
| $\tan x$ | $\displaystyle\frac1{\cos^2x}$ | $\cos x\neq0$ | $\arctan x$ | $\displaystyle\frac1{1+x^2}$ | $x\in\mathbb R$ |
| $\arcsin x$ | $\displaystyle\frac1{\sqrt{1-x^2}}$ | $-1<x<1$ | $\arccos x$ | $\displaystyle-\frac1{\sqrt{1-x^2}}$ | $-1<x<1$ |
| $\sinh x$ | $\cosh x$ | $x\in\mathbb R$ | $\cosh x$ | $\sinh x$ | $x\in\mathbb R$ |
| $f(x)^{g(x)}$ | Prima $e^{g(x)\ln f(x)}$ | $f(x)>0$ |  |  |  |

## Regole di derivazione

| Regola | Formula | Nota |
| --- | --- | --- |
| Moltiplicazione per una costante | $(cf(x))'=c\cdot f'(x)$ | $c$ è costante e $c'=0$ |
| Linearità | $(af+bg)'=af'+bg'$ | $a,b$ costanti |
| Prodotto | $(fg)'=f'g+fg'$ | Entrambi i fattori devono essere derivabili nel punto |
| Quoziente | $\displaystyle\left(\frac fg\right)'=\frac{f'g-fg'}{g^2}$ | $g(x)\neq0$ |
| Catena | $(f\circ g)'(x)=f'(g(x))\cdot g'(x)$ | La funzione esterna deve essere derivabile in $g(x)$ |
| Inversa | $\displaystyle(f^{-1})'(y_0)=\frac1{f'(x_0)}$ | $y_0=f(x_0)$ e $f'(x_0)\neq0$ |
| Potenza composta | $\bigl(g(x)^\alpha\bigr)'=\alpha g(x)^{\alpha-1}g'(x)$ | Dove la potenza è definita |
| Radice composta | $\displaystyle(\sqrt{g(x)})'=\frac{g'(x)}{2\sqrt{g(x)}}$ | $g(x)>0$; se $g(x)=0$ va studiata separatamente |
| Esponenziale composta | $(e^{g(x)})'=e^{g(x)}g'(x)$ | Regola della catena |
| Logaritmo composto | $\displaystyle(\ln g(x))'=\frac{g'(x)}{g(x)}$ | $g(x)>0$ |
| Seno composto | $(\sin g(x))'=\cos(g(x))g'(x)$ | Regola della catena |
| Coseno composto | $(\cos g(x))'=-\sin(g(x))g'(x)$ | Regola della catena |

## Teoremi principali

| Teorema | Ipotesi | Formula / conclusione |
| --- | --- | --- |
| Weierstrass | $f$ continua su $[a,b]$ | $\exists x_m,x_M\in[a,b]$ tali che $f(x_m)\le f(x)\le f(x_M)$ |
| Bolzano | $f$ continua su $[a,b]$ e $f(a)f(b)<0$ | $\exists c\in(a,b)$ tale che $f(c)=0$ |
| Fermat | $x_0$ estremo relativo interno e $f$ derivabile in $x_0$ | $f'(x_0)=0$ |
| Rolle | $f$ continua su $[a,b]$, derivabile su $(a,b)$ e $f(a)=f(b)$ | $\exists c\in(a,b)$ tale che $f'(c)=0$ |
| Lagrange | $f$ continua su $[a,b]$ e derivabile su $(a,b)$ | $\displaystyle\exists c\in(a,b):\ f'(c)=\frac{f(b)-f(a)}{b-a}$ |
| Cauchy | $f,g$ continue su $[a,b]$ e derivabili su $(a,b)$ | $\exists c\in(a,b):\ [f(b)-f(a)]g'(c)=[g(b)-g(a)]f'(c)$ |
| De l’Hôpital | Forma $0/0$ oppure $\infty/\infty$ e ipotesi sulle derivate soddisfatte | $\displaystyle\lim\frac{f(x)}{g(x)}=\lim\frac{f'(x)}{g'(x)}$, se il secondo limite esiste |
| Funzione costante | $f$ derivabile su un intervallo $I$ | $f'(x)=0\ \forall x\in I\iff f$ è costante su $I$ |

## Studio tramite le derivate

| Obiettivo | Criterio |
| --- | --- |
| Funzione crescente | $f'(x)\ge0$ sull’intervallo |
| Funzione decrescente | $f'(x)\le0$ sull’intervallo |
| Minimo relativo | $f'$ cambia segno da $-$ a $+$ |
| Massimo relativo | $f'$ cambia segno da $+$ a $-$ |
| Convessità | $f''(x)\ge0$, quindi $f'$ è non decrescente |
| Concavità | $f''(x)\le0$, quindi $f'$ è non crescente |
| Candidato a flesso | $f''(x_0)=0$ oppure $f''(x_0)$ non esiste |
| Flesso | La concavità cambia ai due lati di $x_0$ e il grafico ha una tangente |

## Funzione parte intera

Per

$$
f(x)=\lfloor g(x)\rfloor,
$$

$\lfloor y\rfloor$ è il più grande intero minore o uguale a $y$.

| Situazione in $x_0$ | Che cosa fare | Conclusione |
| --- | --- | --- |
| $g(x_0)\notin\mathbb Z$ e $g$ è continua | Controllare che $g(x)$ resti tra gli stessi due interi vicino a $x_0$ | $\lfloor g(x)\rfloor$ è localmente costante, quindi $f'(x_0)=0$ |
| $g(x_0)\in\mathbb Z$ | Studiare $g(x)$ a destra e a sinistra di $x_0$ | Non si può applicare automaticamente la regola della catena |
| Serve verificare la derivabilità | Determinare prima i valori di $\lfloor g(x)\rfloor$ vicino a $x_0$ | Usare, se necessario, $\displaystyle f'(x_0)=\lim_{x\to x_0}\frac{f(x)-f(x_0)}{x-x_0}$ |
| Si calcola $g'(x)$ | La derivata descrive soltanto la funzione interna | $g'(x)$ da sola non determina la derivata di $\lfloor g(x)\rfloor$ |

### Esempi di parte intera

| Espressione | Valore |
| --- | --- |
| $\lfloor2.7\rfloor$ | $2$ |
| $\lfloor2\rfloor$ | $2$ |
| $\lfloor-0.2\rfloor$ | $-1$ |

## Funzione inversa: punto e retta tangente

Se

$$
y_0=f(x_0),
$$

allora

$$
f^{-1}(y_0)=x_0.
$$

Il punto sul grafico di $f^{-1}$ è quindi $(y_0,x_0)$. Se $f$ è invertibile vicino a $x_0$ e $f'(x_0)\neq0$, allora

$$
(f^{-1})'(y_0)=\frac{1}{f'(x_0)}.
$$

La retta tangente al grafico di $f^{-1}$ nel punto $(y_0,x_0)$ è

$$
y=x_0+\frac{1}{f'(x_0)}(x-y_0).
$$

**Attenzione:** nella parentesi compare $x-y_0$, non $x-x_0$, perché l'ascissa del punto sul grafico dell'inversa è $y_0$.
