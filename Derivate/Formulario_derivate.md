# Formulario delle derivate

Formulario sintetico di definizioni, derivate note, regole operative e teoremi principali.

## Definizioni fondamentali

| Oggetto | Formula | Condizioni / significato |
| --- | --- | --- |
| Derivata in (x_0) | (displaystyle f'(x_0)=lim_{x	o x_0}rac{f(x)-f(x_0)}{x-x_0}) | Il limite deve esistere ed essere finito |
| Derivata con incremento (h) | (displaystyle f'(x_0)=lim_{h	o0}rac{f(x_0+h)-f(x_0)}h) | (h
eq0) prima del limite |
| Derivate laterali | (displaystyle f'_pm(x_0)=lim_{h	o0^pm}rac{f(x_0+h)-f(x_0)}h) | (f'(x_0)) esiste se coincidono e sono finite |
| Retta tangente | (displaystyle y=f(x_0)+f'(x_0)(x-x_0)) | (f'(x_0)) è la pendenza |
| Approssimazione lineare | (displaystyle f(x)=f(x_0)+f'(x_0)(x-x_0)+o(x-x_0)) | Per (x	o x_0) |
| Derivabilità e continuità | (displaystyle f	ext{ derivabile in }x_0Rightarrow f	ext{ continua in }x_0) | Il contrario non vale sempre |

## Derivate note

| Funzione (f(x)) | Derivata (f'(x)) | Condizioni |
| --- | --- | --- |
| (c) | (0) | (cinmathbb R) |
| (x) | (1) | (xinmathbb R) |
| (x^alpha) | (alpha x^{alpha-1}) | In generale (x>0) per (alphainmathbb R) |
| (sqrt{x}) | (displaystylerac1{2sqrt{x}}) | (x>0) |
| (displaystylerac1x) | (displaystyle-rac1{x^2}) | (x
eq0) |
| (e^x) | (e^x) | (xinmathbb R) |
| (a^x) | (a^xln a) | (a>0) |
| (ln x) | (displaystylerac1x) | (x>0) |
| (ln|x|) | (displaystylerac1x) | (x
eq0) |
| (log_a x) | (displaystylerac1{xln a}) | (x>0, a>0, a
eq1) |
| (sin x) | (cos x) | (xinmathbb R) |
| (cos x) | (-sin x) | (xinmathbb R) |
| (	an x) | (displaystylerac1{cos^2x}=1+	an^2x) | (cos x
eq0) |
| (arcsin x) | (displaystylerac1{sqrt{1-x^2}}) | (-1<x<1) |
| (arccos x) | (displaystyle-rac1{sqrt{1-x^2}}) | (-1<x<1) |
| (arctan x) | (displaystylerac1{1+x^2}) | (xinmathbb R) |
| (sinh x) | (cosh x) | (xinmathbb R) |
| (cosh x) | (sinh x) | (xinmathbb R) |

## Regole di derivazione

| Regola | Formula | Nota |
| --- | --- | --- |
| Linearità | ((af+bg)'=af'+bg') | (a,b) costanti |
| Prodotto | ((fg)'=f'g+fg') | Entrambi i fattori devono essere derivabili nel punto |
| Quoziente | (displaystyleleft(rac fgight)'=rac{f'g-fg'}{g^2}) | (g(x)
eq0) |
| Catena | ((fcirc g)'(x)=f'(g(x))g'(x)) | La funzione esterna deve essere derivabile in (g(x)) |
| Inversa | (displaystyle(f^{-1})'(y_0)=rac1{f'(x_0)}) | (y_0=f(x_0)), (f'(x_0)
eq0) |
| Potenza composta | ((g(x))^alpha{}'=alpha(g(x))^{alpha-1}g'(x)) | Dove la potenza è definita |
| Esponenziale composta | ((e^{g(x)})'=e^{g(x)}g'(x)) | Regola della catena |
| Logaritmo composto | ((ln g(x))'=displaystylerac{g'(x)}{g(x)}) | (g(x)>0) |
| Seno composto | ((sin g(x))'=cos(g(x))g'(x)) | Regola della catena |
| Coseno composto | ((cos g(x))'=-sin(g(x))g'(x)) | Regola della catena |

## Teoremi principali

| Teorema | Ipotesi | Formula / conclusione |
| --- | --- | --- |
| Weierstrass | (f) continua su ([a,b]) | (exists x_m,x_Min[a,b]) tali che (f(x_m)le f(x)le f(x_M)) |
| Bolzano | (f) continua su ([a,b]), (f(a)f(b)<0) | (exists cin(a,b)) tale che (f(c)=0) |
| Fermat | (x_0) estremo relativo interno, (f) derivabile in (x_0) | (f'(x_0)=0) |
| Rolle | (f) continua su ([a,b]), derivabile su ((a,b)), (f(a)=f(b)) | (exists cin(a,b)) tale che (f'(c)=0) |
| Lagrange | (f) continua su ([a,b]), derivabile su ((a,b)) | (displaystyleexists cin(a,b): f'(c)=rac{f(b)-f(a)}{b-a}) |
| Cauchy | (f,g) continue su ([a,b]), derivabili su ((a,b)) | (exists cin(a,b): [f(b)-f(a)]g'(c)=[g(b)-g(a)]f'(c)) |
| De l’Hôpital | Forma (0/0) oppure (infty/infty), ipotesi sulle derivate soddisfatte | (displaystylelimrac{f(x)}{g(x)}=limrac{f'(x)}{g'(x)}), se il secondo limite esiste |
| Funzione costante | (f) derivabile su un intervallo (I) | (f'(x)=0 orall xin Iiff f) è costante su (I) |

## Studio tramite le derivate

| Obiettivo | Criterio |
| --- | --- |
| Funzione crescente | (f'(x)ge0) sull’intervallo |
| Funzione decrescente | (f'(x)le0) sull’intervallo |
| Minimo relativo | (f') cambia segno da (-) a (+) |
| Massimo relativo | (f') cambia segno da (+) a (-) |
| Convessità | (f''(x)ge0), quindi (f') è non decrescente |
| Concavità | (f''(x)le0), quindi (f') è non crescente |
| Candidato a flesso | (f''(x_0)=0) oppure (f''(x_0)) non esiste |
| Flesso | La concavità cambia ai due lati di (x_0) e il grafico ha una tangente |

## Funzione parte intera

Per

[
f(x)=lfloor g(x)floor,
]

(lfloor yfloor) è il più grande intero minore o uguale a (y).

| Situazione in (x_0) | Che cosa fare | Conclusione |
| --- | --- | --- |
| (g(x_0)
otinmathbb Z) e (g) è continua | Controllare che (g(x)) resti tra gli stessi due interi vicino a (x_0) | (lfloor g(x)floor) è localmente costante, quindi (f'(x_0)=0) |
| (g(x_0)inmathbb Z) | Studiare (g(x)) a destra e a sinistra di (x_0) | Non si può applicare automaticamente la regola della catena |
| Serve verificare la derivabilità | Determinare prima i valori di (lfloor g(x)floor) vicino a (x_0) | Usare, se necessario, (displaystyle f'(x_0)=lim_{x	o x_0}rac{f(x)-f(x_0)}{x-x_0}) |
| Si calcola (g'(x)) | La derivata descrive soltanto la funzione interna | (g'(x)) da sola non determina la derivata di (lfloor g(x)floor) |

Esempi di parte intera:

| Espressione | Valore |
| --- | --- |
| (lfloor2.7floor) | (2) |
| (lfloor2floor) | (2) |
| (lfloor-0.2floor) | (-1) |
