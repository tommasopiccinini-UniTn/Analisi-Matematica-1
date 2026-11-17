# Formulario delle derivate

Formulario sintetico di definizioni, derivate note, regole operative e teoremi principali.

## Definizioni fondamentali

| Oggetto | Formula | Condizioni / significato |
| --- | --- | --- |
| Derivata in $x_0$ | $\displaystyle f^{\prime}(x_0)=\lim_{x\to x_0}\frac{f(x)-f(x_0)}{x-x_0}$ | Il limite deve esistere ed essere finito |
| Derivata con incremento $h$ | $\displaystyle f^{\prime}(x_0)=\lim_{h\to0}\frac{f(x_0+h)-f(x_0)}{h}$ | $h\neq0$ prima del limite |
| Derivate laterali | $\displaystyle f^{\prime}_\pm(x_0)=\lim_{h\to0^\pm}\frac{f(x_0+h)-f(x_0)}{h}$ | $f^{\prime}(x_0)$ esiste se coincidono e sono finite |
| Retta tangente | $\displaystyle y=f(x_0)+f^{\prime}(x_0)(x-x_0)$ | $f^{\prime}(x_0)$ è la pendenza |
| Approssimazione lineare | $\displaystyle f(x)=f(x_0)+f^{\prime}(x_0)(x-x_0)+o(x-x_0)$ | Per $x\to x_0$ |
| Derivabilità e continuità | $f\text{ derivabile in }x_0\Rightarrow f\text{ continua in }x_0$ | Il contrario non vale sempre |

## Derivate note

| Funzione $f(x)$ | Derivata $f^{\prime}(x)$ | Condizioni |
| --- | --- | --- |
| $c$ | $0$ | $c\in\mathbb R$ |
| $x$ | $1$ | $x\in\mathbb R$ |
| $x^\alpha$ | $\alpha x^{\alpha-1}$ | In generale $x>0$ per $\alpha\in\mathbb R$ |
| $\sqrt{x}$ | $\displaystyle\frac1{2\sqrt{x}}$ | $x>0$ |
| $\displaystyle\frac1x$ | $\displaystyle-\frac1{x^2}$ | $x\neq0$ |
| $e^x$ | $e^x$ | $x\in\mathbb R$ |
| $a^x$ | $a^x\ln a$ | $a>0$ |
| $\ln x$ | $\displaystyle\frac1x$ | $x>0$ |
| $\ln\lvert x\rvert$ | $\displaystyle\frac1x$ | $x\neq0$ |
| $\log_a x$ | $\displaystyle\frac1{x\ln a}$ | $x>0,\ a>0,\ a\neq1$ |
| $\sin x$ | $\cos x$ | $x\in\mathbb R$ |
| $\cos x$ | $-\sin x$ | $x\in\mathbb R$ |
| $\tan x$ | $\displaystyle\frac1{\cos^2x}=1+\tan^2x$ | $\cos x\neq0$ |
| $\arcsin x$ | $\displaystyle\frac1{\sqrt{1-x^2}}$ | $-1<x<1$ |
| $\arccos x$ | $\displaystyle-\frac1{\sqrt{1-x^2}}$ | $-1<x<1$ |
| $\arctan x$ | $\displaystyle\frac1{1+x^2}$ | $x\in\mathbb R$ |
| $\sinh x$ | $\cosh x$ | $x\in\mathbb R$ |
| $\cosh x$ | $\sinh x$ | $x\in\mathbb R$ |

## Regole di derivazione

| Regola | Formula | Nota |
| --- | --- | --- |
| Linearità | $(af+bg)'=af^{\prime}+bg^{\prime}$ | $a,b$ costanti |
| Prodotto | $(fg)'=f^{\prime}g+fg^{\prime}$ | Entrambi i fattori devono essere derivabili nel punto |
| Quoziente | $\displaystyle\left(\frac fg\right)'=\frac{f^{\prime}g-fg^{\prime}}{g^2}$ | $g(x)\neq0$ |
| Catena | $(f\circ g)'(x)=f^{\prime}(g(x))g^{\prime}(x)$ | La funzione esterna deve essere derivabile in $g(x)$ |
| Inversa | $\displaystyle(f^{-1})'(y_0)=\frac1{f^{\prime}(x_0)}$ | $y_0=f(x_0)$ e $f^{\prime}(x_0)\neq0$ |
| Potenza composta | $\bigl(g(x)^\alpha\bigr)'=\alpha g(x)^{\alpha-1}g^{\prime}(x)$ | Dove la potenza è definita |
| Esponenziale composta | $(e^{g(x)})'=e^{g(x)}g^{\prime}(x)$ | Regola della catena |
| Logaritmo composto | $\displaystyle(\ln g(x))'=\frac{g^{\prime}(x)}{g(x)}$ | $g(x)>0$ |
| Seno composto | $(\sin g(x))'=\cos(g(x))g^{\prime}(x)$ | Regola della catena |
| Coseno composto | $(\cos g(x))'=-\sin(g(x))g^{\prime}(x)$ | Regola della catena |

## Teoremi principali

| Teorema | Ipotesi | Formula / conclusione |
| --- | --- | --- |
| Weierstrass | $f$ continua su $[a,b]$ | $\exists x_m,x_M\in[a,b]$ tali che $f(x_m)\le f(x)\le f(x_M)$ |
| Bolzano | $f$ continua su $[a,b]$ e $f(a)f(b)<0$ | $\exists c\in(a,b)$ tale che $f(c)=0$ |
| Fermat | $x_0$ estremo relativo interno e $f$ derivabile in $x_0$ | $f^{\prime}(x_0)=0$ |
| Rolle | $f$ continua su $[a,b]$, derivabile su $(a,b)$ e $f(a)=f(b)$ | $\exists c\in(a,b)$ tale che $f^{\prime}(c)=0$ |
| Lagrange | $f$ continua su $[a,b]$ e derivabile su $(a,b)$ | $\displaystyle\exists c\in(a,b):\ f^{\prime}(c)=\frac{f(b)-f(a)}{b-a}$ |
| Cauchy | $f,g$ continue su $[a,b]$ e derivabili su $(a,b)$ | $\exists c\in(a,b):\ [f(b)-f(a)]g^{\prime}(c)=[g(b)-g(a)]f^{\prime}(c)$ |
| De l’Hôpital | Forma $0/0$ oppure $\infty/\infty$ e ipotesi sulle derivate soddisfatte | $\displaystyle\lim\frac{f(x)}{g(x)}=\lim\frac{f^{\prime}(x)}{g^{\prime}(x)}$, se il secondo limite esiste |
| Funzione costante | $f$ derivabile su un intervallo $I$ | $f^{\prime}(x)=0\ \forall x\in I\iff f$ è costante su $I$ |

## Studio tramite le derivate

| Obiettivo | Criterio |
| --- | --- |
| Funzione crescente | $f^{\prime}(x)\ge0$ sull’intervallo |
| Funzione decrescente | $f^{\prime}(x)\le0$ sull’intervallo |
| Minimo relativo | $f^{\prime}$ cambia segno da $-$ a $+$ |
| Massimo relativo | $f^{\prime}$ cambia segno da $+$ a $-$ |
| Convessità | $f^{\prime\prime}(x)\ge0$, quindi $f^{\prime}$ è non decrescente |
| Concavità | $f^{\prime\prime}(x)\le0$, quindi $f^{\prime}$ è non crescente |
| Candidato a flesso | $f^{\prime\prime}(x_0)=0$ oppure $f^{\prime\prime}(x_0)$ non esiste |
| Flesso | La concavità cambia ai due lati di $x_0$ e il grafico ha una tangente |

## Funzione parte intera

Per

$$
f(x)=\lfloor g(x)\rfloor,
$$

$\lfloor y\rfloor$ è il più grande intero minore o uguale a $y$.

| Situazione in $x_0$ | Che cosa fare | Conclusione |
| --- | --- | --- |
| $g(x_0)\notin\mathbb Z$ e $g$ è continua | Controllare che $g(x)$ resti tra gli stessi due interi vicino a $x_0$ | $\lfloor g(x)\rfloor$ è localmente costante, quindi $f^{\prime}(x_0)=0$ |
| $g(x_0)\in\mathbb Z$ | Studiare $g(x)$ a destra e a sinistra di $x_0$ | Non si può applicare automaticamente la regola della catena |
| Serve verificare la derivabilità | Determinare prima i valori di $\lfloor g(x)\rfloor$ vicino a $x_0$ | Usare, se necessario, $\displaystyle f^{\prime}(x_0)=\lim_{x\to x_0}\frac{f(x)-f(x_0)}{x-x_0}$ |
| Si calcola $g^{\prime}(x)$ | La derivata descrive soltanto la funzione interna | $g^{\prime}(x)$ da sola non determina la derivata di $\lfloor g(x)\rfloor$ |

### Esempi di parte intera

| Espressione | Valore |
| --- | --- |
| $\lfloor2.7\rfloor$ | $2$ |
| $\lfloor2\rfloor$ | $2$ |
| $\lfloor-0.2\rfloor$ | $-1$ |
