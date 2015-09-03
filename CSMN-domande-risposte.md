#Calcolo Scientifico e Metodi Numerici
####Corso di Laurea in Informatica, A.A. 2014-2015
##Domande di ripasso

###Idee di base e richiami
**1. Qual è lo scopo della Matematica Numerica?** 

  - La risoluzione numerica (al calcolatore) e l'analisi della soluzione trovata.
  
  
**2. Attraverso quali fasi si passa nel risolvere un problema reale?**

  - 1 definizione del problema reale (Quanto impiego a raggiungere X?)
  - 2 costruzione del modello (Distanza = tot, velocità media = tot2)
  - 3 formulazione del problema matematico (formula *s = v$\cdot$t*)
  - 4 risoluzione (al calcolatore) del problema matematico (solve *t = s /  v*)
  - 5 analisi della soluzione trovata (errori, approssimazioni, conversioni)
  - 6 verifica che la soluzione trovata risolva il problema reale 
  
  
**3. Dove si colloca la Matematica Numerica nel processo di risoluzione di un problema reale?**

  - (4) risoluzione del problema al calcolatore
  - (5) analisi della soluzione trovata

  
**4. Cosa è uno spazio lineare, detto anche spazio vettoriale?**

  - Uno spazio lineare è un insieme dotato delle seguenti proprietà:
    - chiusura rispetto all'addizione: *v1 + v2 = v3*, con *v1, v2, v3$\in$**V***, con ***V*** spazio lineare;
    - chiusura rispetto al prodotto per uno scalare: *a$\in$**K***, campo di scalari, *a$\cdot$v1 = v2*, con *v1, v2$\in$**V***
    - commutatività dell'addizione
    - associatività dell'addizione
    - associatività del prodotto per uno scalare: *a$\cdot$(b$\cdot$v) = (a$\cdot$b)$\cdot$v*
    - proprietà distributiva del prodotto per uno scalare rispetto alla somma di vettori: *a$\cdot$(v1 + v2) = a$\cdot$v1 + a$\cdot$v2*
    - proprietà distributiva del prodotto per uno scalare rispetto alla somma di scalari: *(a + b)$\cdot$v = a$\cdot$v + b$\cdot$v*
    - esistenza dello zero come elemento neutro dell'addizione
    - esistenza dell'1 come elemento neutro del prodotto per uno scalare
    - esistenza dell'opposto: *$\forall$v$\in$**V** $\exists$-v* 


**5. Dai tre esempi di spazio lineare.**

  - Vettori di dimensione *n*
  - Matrici di dimensione m$\times$n
  - Funzioni continue in un intervallo \[a, b\] che ammettono derivata n-esima
  - Polinomi di grado massimo n

  
**6. Dimostra che l’insieme C[a,b] di tutte le funzioni continue nell’intervallo [a,b] è uno spazio lineare sull’insieme dei numeri reali $\mathbb{R}$.**
  
  - *N.B. sono dimostrate solo alcune proprietà a scopo esplicativo*
  - Sia **F** l'insieme delle funzioni continue in \[a,b\] e siano *f() e g()$\in$ **F***, *(f + g)(x) = f(x) + g(x)* quindi *(f + g)()$\in$**F***
  - Sia **K** un campo di scalari e *a$\in$**K***, *a$\cdot$f(x) = af(x)* quindi *af()$\in$**F***
  

**7. Dimostra che l’insieme P^n^ di tutti i polinomi di grado minore o uguale a n è uno
spazio lineare sull’insieme dei numeri reali $\mathbb{R}$.**

  - *N.B. sono dimostrate solo alcune proprietà a scopo esplicativo*
  - 


**8. Quando n elementi x 1 , x 2 , ...,x n di uno spazio lineare su $\mathbb{R}$ si dicono linearmente
indipendenti.**

 - N elementi si dicono linearmente indipendenti se la loro combinazione lineare è *0* **solo** se tutti i coefficienti sono *0*.
 
 
**9. Dai un esempio di tre elementi nello spazio lineare $\mathbb{R}$^2^ linearmente dipendenti.**

 - $\mathbb{R}$^2^ ha dimensione 2, quindi presi tre elementi questi saranno sempre dipendenti: *(0, 1)*, *(1, 0)*, *(1, 1)*


**10. Dai un esempio di tre elementi nello spazio lineare $\mathbb{R}$^3^ linearmente dipendenti.**

 - *v~1~=(1, 0, 0)*, *v~2~=(0, 1, 1)*, *v~3~=(6, 4, 4)* perchè *6v~1~ + 4v~2~ = v~3~*.
 
 
**11. Dai un esempio di tre elementi linearmente indipendenti nello spazio lineare C[a,b] di
tutte le funzioni continue in \[a,b\].**

 - *f()=sin(x)*, *g()=cos(x)*, *h()=x^2^*


**12. Le tre funzioni *y~1~(x)=cos(x)*, *y~2~(x)=-sen(x)* e *y~3~(x)=2cos(x)+4sen(x)*
sono linearmente indipendenti? Giustifica la risposta.**

 - No, poichè *2y~1~ + (-4y~2~) = y~3~*. 
 

**13. Le tre funzioni *y~1~(x)=e^x^* , *y~2~(x)=3x^2^* e *y~3~(x)=x-3ln(x)*
sono linearmente indipendenti? Giustifica la risposta.**

 - Si, poiché nessuna di esse può essere espressa come combinazione lineare delle altre.
 

**14. Che cosa è una base di uno spazio lineare?**

 - Sia **S** uno spazio lineare (vettoriale) di dimensione *n*, si dice base di 
**S** l'insieme di n elementi di **S** che siano generatori e linearmente indipendenti.


**15. Cosa significa dire che uno spazio lineare ha dimensione finita.**

 - $\exists$ un *n* tale che presi *n+1* elementi, questi saranno
necessariamente linearmente dipendenti.

**16. Dai tre esempi di spazi lineari di dimensione 3.**

 - Vettori su $\mathbb{R}$^3^
 - Polinomi di grado al più 3
 - ???
 
**17. L’insieme di tutti i polinomi di grado < 4 è uno spazio lineare di dimensione finita?
Se sì, fornisci una sua base.**

 - Si, *a~0~+a~1~x+a~2~x^2^+a~3~x^3^*

**18. L’insieme di tutti le matrici 2X2 è uno spazio lineare di dimensione finita? Se sì,
fornisci una sua base.**

 - $\left( \begin{array}{cc} 
1 & 0 \\
 0 & 0 \end{array} \right)$

 - $\left( \begin{array}{cc}
0 & 1 \\
0 & 0 \end{array} \right)$

 - $\left( \begin{array}{cc}
0 & 0 \\
1 & 0 \end{array} \right)$

 - $\left( \begin{array}{cc}
0 & 0 \\
0 & 1 \end{array} \right)$


**19. I vettori *(1, 2)* e *(2, 0)* costituiscono una base per lo spazio vettoriale $\mathbb{R}$^2^, ovvero con
una combinazione lineare di *(1, 2)* e *(2, 0)* puoi formare una qualsiasi coppia di
numeri reali?**

 - Proviamo ad ottenere la base canonica *(0, 1)*, *(1, 0)*. 
 - *$\frac{1}{2}$v~1~ - $\frac{1}{4}$v~2~ = (0, 1)*.
 - *0v~1~ - $\frac{1}{2}$v~2~ = (1, 0)*
 - Quindi è una base per $\mathbb{R}$^2^.
 

**20. Cosa è l’autovalore di una matrice.**

 - Dato uno spazio lineare *V* ed un'applicazione lineare (endomorfismo) *F: V $\to$ V*
esistono particolari vettori tali che *F(v) = $\lambda$v*. Chiamiamo $\lambda$ autovalore e *v* 
autovettore associato a tale autovalore. Si definisce autospazio relativo all'autovalore l'insieme dei vettori
generati generati da tale autovalore.
 
$\iffalse$
21. Cosa è il raggio spettrale di una matrice.
22. Come si definisce la norma in uno spazio lineare.
23. Dai tre esempi di norme definite in $\mathbb{R}$^n^ , lo spazio di tutte le n-ple di numeri reali.
24. Cosa è la disuguaglianza triangolare in uno spazio lineare normato. Vale sempre?
25. Come si può definire la distanza tra due elementi di uno spazio lineare normato.
26. Considera lo spazio $\mathbb{R}$^2^ . Indica graficamente la sfera unitaria S= $\mathbb{R}$^2^ | ||x||<=1
considerando la distanza relativa alla norma euclidea, la norma di Manhattan e la
norma del massimo.
27. Cosa significa dire che una norma è submoltiplicativa.
28. Come si definisce una norma matriciale.
29. Date le 2 matrici 3x3
1 1 2 3 
 2 3 4 
 4 5 6 
 0 1 2 




  7 8 9  
  5 6 7  
calcola la loro distanza secondo la norma del massimo || || .
30. Date le 2 matrici 3x3
 1 2 3 
 2 3 4 
 4 5 6 
 0 1 2 




  7 8 9  
  5 6 7  
calcola la loro distanza secondo la norma || || 1
31. Date le 2 matrici 3x3
 1 0 0 
 2 0 0 
 0 5 0 
 0 1 0 




  0 0 9  
  0 0 7  
calcola la loro distanza secondo la norma euclidea || || 2
32. Data la matrice 3x3
 1 2 3 
 4 5 6 


  7 8 9  
trova una matrice B la cui distanza da A è 1 secondo la norma || || 1
33. Data la matrice 3x3
 1 2 3 
 4 5 6 


  7 8 9  
trova una matrice B la cui distanza da A è 1 secondo la norma || || 
34. Dai due esempi di norme per lo spazio C[a,b] di tutte le funzioni continue in [a,b]
35. Data la funzione y(x)=sen(x), trova due funzioni continue in [-2, 2] la cui distanza
da y è uguale a 4 secondo la norma del massimo per funzioni.
36. Considera le funzioni y 1 (x)=1.5x e y 2 (x)=x definite nell’intervallo [0,1]. Quale è la
distanza tra le due funzioni se si considera come distanza quella associata alla norma
di funzione || f ||  max | f ( x ) | .
[ 0 , 1 ]
37. Considera le funzioni y 1 (x)=1.5x e y 2 (x)=x definite nell’intervallo [0,1]. Quale è la
distanza tra le due funzioni se si considera come distanza quella associata alla norma
1
di funzione || f ||  ( f ( x ) 2 dx ) 0 . 5 .
0
38. Cosa significa dire che una norma di una matrice nn è consistente o compatibile con
una norma di vettore in $\mathbb{R}$n .
39. Come si definisce una norma matriciale naturale.
40. Quanto vale la norma della matrice identità nn se la norma è naturale. Giustifica la
risposta.
41. Fornisci un esempio di norma non naturale di matrice.
42. Dati A, matrice nn e x vettore in $\mathbb{R}$n , verifica che per una norma naturale si ha
|| Ax ||  || A || || x || .
243. Determina la norma di matrice indotta dalla norma di vettore || x ||  max | x i |  (con
1  i  n
dimostrazione).
n
44. Determina la norma di matrice indotta dalla norma di vettore || x ||   | x i | (con
i  1
dimostrazione).
n
45. Quale è la norma di matrice indotta dalla norma di vettore || x ||  (  x i 2 ) 0 . 5 .
i  1
46. Perché è utile definire la norma in uno spazio lineare.
47. Considera lo spazio vettoriale $\mathbb{R}$ 2 in cui sia definita una norma ||||. Supponi che valga
la relazione lim || x ||  12 . Quanto vale la norma dell’elemento [2,3]. Giustifica la
x  [ 2 , 3 ]
risposta.
48. Quale relazione tra la norma ed il raggio spettrale vale per ogni norma naturale di
matrice nn (con dimostrazione).
49. Quando una matrice nn è detta convergente.
50. Dimostra che, se lim || A m ||  0 , allora la matrice A è convergente.
m  
51. Dimostra che se || A ||  1 , allora la matrice A è convergente.
52. Dai un esempio di spazio lineare a dimensione infinita.
53. Quando un insieme di elementi x 1 ,x 2 ,... di elementi di uno spazio normato è detto
chiuso in X.
54. Quando uno spazio lineare si dice separabile.
55. Lo spazio C[a,b] di tutte le funzioni continue in [a,b] è separabile?
56. Come si definisce il prodotto scalare in uno spazio lineare.
57. Dai un esempio di prodotto scalare definito in uno spazio lineare.
58. Dai un esempio di prodotto scalare definito nello spazio C[a,b] di tutte le funzioni
continue in [a,b].
59. Come si può ottenere una norma se si dispone di un prodotto scalare.
60. Verifica la proprietà di Cauchy-Schwartz nello spazio vettoriale $\mathbb{R}$^2^ .
61. Come si definisce l’angolo tra due elementi di uno spazio lineare dotato di prodotto
scalare.
Errori e rappresentazione dei numeri in un calcolatore
1. Cosa si intende per problema diretto e problema inverso.
2. Quando un problema si dice ben posto.
3. Quando un problema si dice ben condizionato
4. Quando un algoritmo si dice stabile.
5. Il condizionamento può dipendere dai dati in input?
6. Quale categoria di problemi riusciamo a risolvere in Matematica Numerica.
7. Cosa si intende per errore inerente.
8. Come è definito l’errore inerente del problema di valutare una funzione reale.
9. Cos’è il numero di condizionamento di un problema.
10. Come è definito il numero di condizionamento del problema di valutare una funzione
reale.
11. Dimostra che il numero di condizionamento  f del problema di valutare una funzione
xf ' ( x )
 x .
f ( x )
12. Cosa sono l’errore assoluto e l’errore relativo.
reale è equivalente a  f 
313. Illustra i vari tipi di errore che si possono incontrare nella risoluzione di un problema
reale al calcolatore.
14. Cosa è la rappresentazione posizionale dei numeri che utilizziamo.
15. Cosa è la base di un sistema di rappresentazione dei numeri naturali.
16. Fissata una base di numerazione, come si può rappresentare in modo univoco un
qualsiasi numero reale non nullo.
17. Rappresenta il numero 35 in base 2, in base 8 e in base 16.
18. Quanti sono i numeri reali definiti in Matematica.
19. Cosa è la mantissa e l’esponente nella rappresentazione normalizzata di un numero
reale.
20. Quale condizione soddisfa la mantissa nella rappresentazione normalizzata di un
numero reale.
21. Cosa è il sistema floating point, o sistema dei numeri macchina.
22. Illustra i parametri che definiscono un sistema floating point. Individua il numero
positivo più piccolo e il numero positivo più grande del sistema.
23. Che differenze ci sono tra la rappresentazione normalizzata di un numero reale e la
rappresentazione normalizzata di un numero macchina.
24. Poiché ogni calcolatore lavora con circuiti elettrici a due stati (ON/OFF), c’è una
qualche differenza ad utilizzare un sistema floating point a base 2 o a base 16.
25. Fissati i parametri di un sistema floating point, indicare quanti sono i numeri
rappresentabili (giustificare la risposta).
26. Elencare tutti i numeri macchina del sistema floating point F(2,2,-1,1).
27. Come si distribuiscono i numeri macchina positivi sulla retta reale.
28. In quali casi un numero reale viene rappresentato esattamente in un calcolatore.
29. In quali casi un numero reale non viene rappresentato esattamente in un calcolatore.
30. Cosa è l’underflow e l’overflow.
31. Cosa è il troncamento ed l’arrotondamento di un numero reale.
32. Nel sistema floating point F(10,6,-20,20), determina un numero reale la cui
rappresentazione sia esatta ed un numero reale la cui rappresentazione non sia esatta.
33. Nel sistema floating point F(10,6,-20,20), determina un numero reale la cui
approssimazione con arrotondamento sia differente dalla approssimazione con
troncamento.
34. Nel sistema floating point F(10,6,-20,20), determina un numero reale la cui
approssimazione con arrotondamento sia uguale alla approssimazione con
troncamento.
35. Nel sistema floating point F(2,4,-3,5), determina un numero reale la cui
rappresentazione sia esatta ed un numero reale la cui rappresentazione non sia esatta.
36. Nel sistema floating point F(2,4,-3,5), determina un numero reale la cui
approssimazione con arrotondamento sia differente dalla approssimazione con
troncamento.
37. Nel sistema floating point F(2,4,-3,5), determina un numero reale la cui
approssimazione con arrotondamento sia uguale alla approssimazione con
troncamento.
38. Nel caso classico in cui non vi sia underflow o overflow, qual’è il massimo errore
fl ( x ) x
relativo
che si commette approssimando un numero reale x  0 mediante
x
il suo valore floatging point fl(x).
39. Cos’è e che proprietà soddisfa l’epsilon macchina in un sistema floating point.
40. Cos’è e che proprietà soddisfa la precisione macchina in un sistema floating point.
41. Scrivi l’algoritmo che calcola l’epsilon macchina.
442. Scrivi l’algoritmo che calcola la precisione macchina in un sistema floating point con
arrotondamento.
43. Che relazione esista tra le operazione aritmetiche che definiamo in Matematica e
quelle che esegue il calcolatore.
44. Come viene fatta la somma in un sistema floating point (fornisci un esempio in un
sistema floating point a piacere).
45. In un sistema floating point con base 10 e 6 cifre per la mantissa, determina due
numeri macchina positivi a e b tali che a  b  a .
46. In un sistema floating point con base 10 e 5 cifre per la mantissa, determina due
numeri macchina positivi a e b tali che a  b  a e a 10 b  a .
47. In un sistema floating point con base 8 e 4 cifre per la mantissa, determina due
numeri macchina positivi a e b tali che a  b  a e a  8 b  a .
48. Riguardo all’errore commesso dal calcolo di una generica operazione aritmetica in un
calcolatore, illustrare, spiegandone il significato, quale condizione deve essere
soddisfatta quando l’operazione aritmetica viene eseguita tra numeri macchina.
49. Siano 0  a  b  c tre numeri macchina positivi. Tra i tre possibili algoritmi
( a  b )  c , a  ( b  c ) e ( a  c )  b , qual’è il modo migliore di effettuare la somma
a  b  c al calcolatore? Spiegare il perchè con un esempio in un sistema floating
point con base 10 e 6 cifre per la mantissa.
50. Considerando un particolare algoritmo per la valutazione di una funzione f(x) al
calcolatore, cosa si intende per errore algoritmico.
51. Che differenza sostanziale c’è tra l’errore inerente e l’errore algoritmico.
52. Quando si risolve un problema scientifico al calcolatore, cosa si intende per errore
totale commesso.
53. Cos’è la backward analysis o analisi all’indietro degli errori.
54. Utilizzando l’analisi all’indietro, come può essere interpretato il risultato di una
somma di due numeri macchina effettuata al calcolatore.
Esercizi sull’errore inerente e algoritmico.
1. Considerando il problema di valutare una funzione f(x), determinare l’errore inerente
provocato dalla perturbazione relativa  x dell’argomento x e dire, nei casi seguenti,
per quali valori di x il problema è mal condizionato:
a)
b)
c)
d)
e)
f)
f ( x )  x ( x  1 )
f ( x )  x ( x 1 )
f ( x )  x ( x 2 1 )
f ( x )  x ( x 2  1 )
f ( x )  x 2  2 x  1
f ( x )  x 2 2 x  1
f ( x )  x 2 ( x  1 )
f ( x )  x 2 ( x 1 )
f ( x )  x ( x 3 1 )
j) f ( x )  x ( x 3  1 )
k) f ( x )  x 2 ( x 2 1 )
l) f ( x )  x 2 ( x 2  1 )
m) f ( x )  ( 3 x 6 ) 3
g)
h)
i)
5n)
f ( x )  ( x 2 ) 2 x 3
2. Considerando il problema di valutare una funzione f(x,y), determinare l’errore
inerente provocato dalle perturbazioni relative  x e  y degli argomenti x ed y, e dire,
nei casi seguenti, per quali valori di x ed y il problema è mal condizionato:
a)
b)
c)
d)
f ( x , y )  3 x 5 xy
f ( x , y )  2 y 5 xy
f ( x , y )  x 2 y 2
f ( x , y )  x 2 y xy 2
3. Considerando il problema di valutare al calcolatore una funzione, determinare l’errore
algoritmico associato agli algoritmi seguenti e dire per quali valori in input
l’algoritmo risulta instabile:
a)
b)
c)
d)
e)
f)
g)
f ( x )  x 2 2 x  1
f ( x )  x 2 x
f ( x )  x ( x 1 )
f ( x )  x 2 ( 1  x )
f ( x )  x ( x  x 2 )
f ( x )  x 3 5 x 2
f ( x , y )  3 x 5 xy
4. Considerando il problema di valutare al calcolatore una funzione, determinare l’errore
algoritmico dei due algoritmi proposti (associati ad espressioni algebriche
matematicamente equivalenti) e dire quali sono gli algoritmi stabili e quali quelli
instabili, in funzione dei valori in input:
a)
b)
c)
d)
e)
f)
g)
h) f ( x )  x ( x 2 7 x )
f ( x )  x 2 6 x  9
f ( x )  x 2 ( x 7 )
f ( x , y )  x ( x  y )( x y ) e
e
e
e
e
e
e
e i)
j)
k)
l) f ( x , y )  x 3 xy 2
f ( x , y , z )  ( x  y )  z
f ( x , y , z )  ( x  y ) z
f ( x , y , z )  ( x  y ) z e
e
e
e f ( x , y )  x ( x  y )( x y )
f ( x , y , z )  x  ( y  z )
f ( x , y , z )  x  ( y z )
f ( x , y , z )  xz  yz
f ( x )  ( x  5 ) 2
f ( x )  x 2 ( x 3 )
f ( x )  x 4 8 x 2
f ( x )  x 2 ( x 2 5 )
f ( x , y )  x 2 y 2
f ( x )  ( x 3 ) 2
f ( x )  x 2  10 x  25
f ( x )  x 3 3 x 2
f ( x )  x 2 ( x 2 8 )
f ( x )  x ( x 3 5 x )
f ( x , y )  ( x  y )( x y )
f ( x , y )  x ( x 2 y 2 )
Sistemi lineari (Prima Parte)
61. Cosa significa risolvere un sistema lineare.
2. Quali sono le condizioni per l’esistenza e l’unicità della soluzione di un sistema
lineare.
3. Cosa sono i metodi diretti e cosa sono i metodi iterativi, per la risoluzione di un
sistema lineare.
4. Cosa è l’inversa di una matrice A di dimensione nn.
5. Fai vedere che, se si ha un metodo per risolvere un sistema lineare Ax=b, allora
utilizzando tale metodo si riesce a trovare l’inversa di A.
6. Cosa è lo scaling di un matrice.
7. A cosa servono le tecniche di scaling di un matrice.
8. Come si rappresentano, in notazione matriciale, lo scaling per righe e lo scaling per
colonne.
9. Scrivi la definizione di sistema triangolare superiore ed inferiore.
10. Scrivi l’algoritmo di sostituzione in avanti per la risoluzione del sistema triangolare
inferiore Ly=b, con L matrice triangolare inferiore di dimensione nn.
11. Scrivi l’algoritmo di sostituzione all’indietro per la risoluzione del sistema triangolare
superiore Ux=y, con U matrice triangolare superiore di dimensione nn.
12. Cosa si intende per complessità computazionale di un algoritmo.
13. In Matematica Numerica, quali operazioni vengono considerate al fine di valutare la
complessità computazionale di un algoritmo.
14. Calcola il numero di moltiplicazioni eseguite dall’algoritmo di sostituzione in avanti
che risolve un sistema triangolare inferiore.
15. Calcola il numero di moltiplicazioni eseguite dall’algoritmo di sostituzione
all’indietro che risolve un sistema triangolare superiore.
16. L’analisi all’indietro dell’errore commesso dall’algoritmo di sostituzione in avanti in
aritmetica
di
macchina
conduce
alla
maggiorazione
seguente
2
F  n  eps  L  O ( eps ) . Spiegarne il significato.
17. Scrivi l’algoritmo di Gauss senza scambio di righe, detto “naive”.
18. Cosa sono i minori principali di una matrice.
19. Perchè
vale
la
relazione
di
uguaglianza
( 1 )
( 2 )
( k )
det( A k )  a 1 , 1  a 2 , 2  ...  a k , k , k  1 , 2 ,  , n .
seguente
20. Quando si può applicare l’algoritmo di Gauss senza scambio di righe.
21. Risolvere il sistema lineare Ax=b mediante l’algoritmo di Gauss senza scambio di
 1 2 3 
 0 


righe, dove A   2 4 3 
e b    1   .
  3 2 1  
  2  
22. Quale è la complessità computazionale dell’algoritmo di Gauss.
23. Calcola il numero di moltiplicazioni eseguite dall’algoritmo di Gauss senza scambio
di righe.
for k=1,2,...,n-1
for i=k+1,...,n
m  a / a
ik
( k ) ( k )
ik kk
for j=k+1,...,n+1
7a
( k  1 )
ij
 a m a
( k )
ij
ik
( k )
kj
end
end
end
24. In che cosa consiste la strategia del pivoting parziale.
25. Scrivi l’algoritmo di Gauss con con pivoting parziale per lo scambio di righe.
26. Sotto quale condizione si può applicare il metodo di Gauss con pivoting parziale.
27. Risolvere il sistema lineare Ax=b mediante l’algoritmo di Gauss con pivoting
 4 8 1 
 10 


5
7 
parziale, dove A   6
e b    13   .
  0 10 2  
  6  
28. In che cosa consiste la strategia del pivoting totale.
29. Il pivoting parziale modifica l’ordine delle componenti del vettore contenete la
soluzione? Ed il pivoting totale?
30. Quali vantaggi produce la strategia del pivoting.
31. Cosa è la decomposizione LU di una matrice A di dimensione nn.
32. In quale modo il metodo di Gauss senza scambio di righe permette di ottenere la
decomposizione LU di una matrice.
33. Nel caso si utilizzi il metodo di Gauss con scambio di righe, quale fattorizzazione di
A si ottiene.
34. Che cosa è una matrice di permutazione.
35. Mostrare che la matrice non singolare
 0 1 
A  

 1 0 
non ammette decomposizione A=LU, ma ammette decomposizione PA=LU, dove P è
un’opportuna matrice di permutazione da determinare.
36. Supponendo di disporre della decomposizione A=LU, in che modo tale
decomposizione permette di risolvere il sistema lineare Ax=b.
37. Nel caso n=3, determinare le relazioni che, una volta risolte, permettono di
determinare gli elementi delle matrici L ed U della fattorizzazione A=LU secondo
l’algoritmo di Doolitle.
38. Quando un matrice A è simmetrica definita positiva.
39. Cosa si intende per algoritmo di Cholesky.
40. Scrivere le equazioni che, una volta risolte, pemettono di determinare i valori della
matrice $\mathbb{R}$della decomposizione A=R$\mathbb{R}$T di una matrice simmetrica definita positiva
di dimensione 3.
41. Dovendo risolvere un sistema lineare Ax=b con A simmetria definita positiva, in che
modo devo procedere?
42. L’analisi all’indietro dell’errore commesso dall’algoritmo di l’algoritmo di Cholesky
per risolvere un sistema lineare conduce alla maggiorazione seguente
E
2
 c n  eps  A 2 , con c n valore “piccolo”. Spiegarne il significato.
43. Quando una matrice viene detta sparsa.
44. Cosa è una matrice a banda.
45. Fare un esempio di matrice 66 a banda superiore 2 ed inferiore 3.
46. Si consideri la matrice A di ordine n, a banda superiore q e inferiore p. Supponendo
che esista la fattorizzazione A=LU, quali proprietà hanno le matrici L ed U.
47. Scrivi l’algoritmo che risolve il sistema triangolare inferiore Lx=b con L matrice
triangolare inferiore di dimensione n e a banda inferiore 4. Supponi n>4.
848. Cosa è il fenomeno del “fill-in” nella decomposizione LU di una matrice A. Quando
si verifica.
49. Se la matrice A è una matrice a banda e A=LU, che caratteristica hanno L ed U.
50. Illustra con un esempio numerico, per n=3, il fenomeno del fill-in.
51. Se la matrice A è una matrice a freccia, si presenta il fenomeno del “fill-in”? Perché?
Sistemi lineari (Seconda Parte)
1. Cosa è il numero di condizionamento di una matrice. Che ruolo ha nello studio dei
sistemi lineari.
2. Considerando una norma vettoriale e la corrispondente norma matriciale naturale,
 x
determinare una maggiorazione del rapporto
x
, dove x è soluzione del sistema
lineare Ax  b , e x   x è soluzione del sistema lineare perturbato
A  x   x   b   b , con  b perturbazione del termine noto.
3. Perché è importante conoscere il numero di condizionamento di una matrice.
4. Se la norma matriciale è una norma naturale, quanto vale il numero di
condizionamento della matrice identità I. Giustifica la risposta.
0
0 
 10

5. Quanto vale il numero di condizionamento della matrice A   0 0 . 5 0   rispetto
  0
0
3  
6.
7.
8.
9.
alla norma 1, rispetto alla norma infinito e rispetto alla norma 2.
Se la matrice A ha numero di condizionamento =6, qual è il numero di
condizionamento della matrice 5A. Giustifica la risposta.
Elenca le proprietà che conosci del numero di condizionamento di una matrice.
Dimostrare che il numero di condizionamento di una matrice in norma naturale è
sempre maggiore o uguale a 1.
Il determinante dà una buona stima del numero di condizionamento?
10. Considerando il sistema lineare Ax  b , se
 x
 10
x
 2
e
 b
 10
b
 5
cosa
possiamo dire del numero di condizionamento della matrice A.
11. Supponi che il metodo di Gauss con pivoting parziale eseguito al calcolatore ritorni le
matrici L e U come fattorizzazione di A. Se A è simmetrica definita positiva e di
dimensioni non grandi, il risultato è affidabile?
12. Fornire 3 esempi di matrice dotata di numero di condizionamento minore possibile.
13. Cosa è un metodo iterativo per la risoluzione di un sistema lineare.
14. Nel caso in cui ci sia convergenza, quale proprietà deve soddisfare un metodo
iterativo affinché esso possa essere utilizzato per risolvere un sistema lineare.
15. In quali casi i metodi iterativi risultano particolarmente efficienti?
16. Cosa sono i metodi iterativi di tipo splitting per la risoluzione di un sistema lineare.
17. Come si esprime l’iterata k-esima di un metodo iterativo di tipo splitting.
18. Quale è la matrice di iterazione di un metodo iterativo di tipo splitting, con splitting
A  M N .
19. Ad ogni iterazione di un metodo iterativo di tipo splitting, con splitting A  M N ,
quale sistema lineare occorre risolvere?
20. Nella rappresentazione matriciale classica dei metodi splitting, con splitting
A  M N , qual è lo schema del metodo iterativo di Jacobi per la risoluzione di un
9sistema lineare.
21. Nella rappresentazione matriciale classica dei metodi splitting, con splitting
A  M N , qual è lo schema del metodo iterativo di Gauss-Seidel per la risoluzione
di un sistema lineare.
22. Considerando lo schema iterativo Mx  k 1   Nx  k   b del metodo di Jacobi per la
 5 1 1 
 7 


risoluzione del sistema lineare Ax  b con A   4 8 2  e b    14   , calcolare
  6 3 9  
  18  
la matrice di iterazione M 1 N ed il vettore M 1 b utili all’esecuzione delle iterazioni.
23. Considerando lo schema iterativo Mx  k 1   Nx  k   b del metodo di Gauss-Seidel per
 5 1 1 
 7 


b    10   ,
la risoluzione del sistema lineare Ax  b con A   0 8 2 
e
  0 9 9  
  18  
calcolare la matrice di iterazione M 1 N ed il vettore M 1 b utili all’esecuzione delle
iterazioni.
24. Illustra due criteri mediante i quali è possibile arrestare un metodo iterativo.
25. Quando un metodo iterativo per la risoluzione di un sistema lineare basato sullo
( k  1 )
 Nx  b è convergente.
schema Mx
26. Dimostra che, posto e ( k )  x * x ( k ) , dove x * rappresenta la soluzione esatta del
( k )
sistema e x rappresenta l’iterata k-esima di un metodo iterativo con matrice di
iterazione B , allora si ha che e ( k )  B k e ( 0 ) .
27. Dimostra che se la matrice di iterazione è convergente allora il metodo iterativo è
convergente.
28. Dimostra che se la matrice di iterazione ha norma naturale minore di 1 allora il
metodo iterativo è convergente.
29. Fornisci una condizione sufficiente alla convergenza del metodo di Jacobi.
30. Fornisci una condizione sufficiente alla convergenza del metodo di Gauss-Seidel.
( k )
Approssimazione di funzioni
1. In che cosa consiste il problema dell’approssimazione di una funzione.
2. Nel caso in cui si conosca l'espressione analitica di una funzione, quando risulta
conveniente utilizzare una sua approssimazione?
3. Illustra due strategie per risolvere il problema dell’approssimazione di una funzione.
4. Dai la formulazione matematica del problema dell’approssimazione mediante
interpolazione.
5. Quando si parla di interpolazione lineare.
6. Dai due esempi di problemi di interpolazione.
7. In che cosa consiste l’approssimazione mediante interpolazione polinomiale.
8. Fai un grafico di carattere qualitativo del polinomio interpolatore di grado al più 2
interpolante i punti P1=(0,0), P2=(1,1), P3=(3,-2).
9. Fai un grafico di carattere qualitativo del polinomio interpolatore di grado al più 2
interpolante i punti P1=(0,0), P2=(1,1), P3=(2,2).
10. Fai un grafico di carattere qualitativo del polinomio interpolatore di grado al più 3
interpolante i punti P1=(0,0), P2=(1,1), P3=(3,-2), P4=(4,0).
11. Fai un grafico di carattere qualitativo del polinomio interpolatore di grado al più 4
interpolante i punti P1=(0,0), P2=(1,1), P3=(3,-2), P4=(4,0), P5=(5,0).
1012. Dimostra che il problema dell’interpolazione polinomiale ammette soluzione e questa
è unica.
13. Scrivi l’espressione dei polinomi interpolanti mediante la rappresentazione di
Lagrange. Fai un grafico di carattere qualitativo degli elementi della base di Lagrange
per n=1,2,3.
14. Quali valori assumono i polinomi della base di Lagrange nei nodi di interpolazione.
15. Scrivi l’espressione del polinomio interpolatore di grado 2, nella rappresentazione di
Lagrange, interpolante i punti P1=(0,0), P2=(1,1), P3=(3,-2). Fai un grafico di
carattere qualitativo degli elementi della base di Lagrange.
16. In che cosa consiste l’interpolazione di Hermite.
17. Dai un esempio grafico del problema dell’interpolazione di Hermite conivolgente la
derivata prima.
18. Dai la forma generale dell’interpolazione lineare.
19. Quali sono le condizioni sotto le quali il problema generale dell’interpolazione
ammette soluzione e questa è unica.
20. A cosa serve l'algoritmo di Neville.
21. Enunciare ed illustrare il significato del teorema di Weierstrass sull’approssimazione
di una funzione mediante un polinomio.
22. Cosa è una matrice di interpolazione.
23. Determinare le prime 5 righe della matrice di interpolazione relativa a nodi
equidistanti sull'intervallo [0,1].
24. Cosa dice il teorema di Faber sui polinomi di interpolazione.
25. Se f(x) è una funzione continua in un intervallo [a,b], aumentando i punti di
interpolazione la successione dei polinomi interpolanti converge sempre
uniformemente a f(x) ? Se la risposta è no, fornire un esempio.
26. Se f(x) è una funzione continua in un intervallo [a,b], puoi scegliere la matrice di
interpolazione in modo che la successione dei polinomi interpolanti converga
uniformemente a f(x) ? Se la risposta è si, fornire un esempio.
27. Dai l’espressione dell’errore di interpolazione associato all'interpolazione
polinomiale.
28. Dai una maggiorazione per l’errore di interpolazione associato all'interpolazione
polinomiale.
29. In quali condizioni si può dare l’espressione dell’errore di interpolazione associato
all'interpolazione polinomiale di grado n ?
30. Interpolando la funzione f ( x )  e x sull'intervallo [0,1] mediante polinomi,
determinare un numero di nodi di interpolazione sufficiente ad ottenere un errore di
interpolazione minore di 1/50.
31. Interpolando la funzione f ( x )  e 2 x sull'intervallo [0,1] mediante polinomi,
determinare un numero di nodi di interpolazione sufficiente ad ottenere un errore di
interpolazione minore di 1/50.
32. Interpolando la funzione f(x)=sin(x) sull'intervallo [0,1] mediante polinomi,
determinare un numero di nodi di interpolazione sufficiente ad ottenere un errore di
interpolazione minore di 1/100.
33. Approssimando la funzione f ( x )  e x mediante polinomi interpolatori, dimostra che
l’errore di interpolazione tende a zero al crescere del numero dei nodi di
interpolazione.
34. Cosa dice il teorema di Bernstein circa i polinomi di interpolazione su nodi di
Chebichev.
35. Supponi di dover necessariamente approssimare una funzione f  C 1  a , b  mediante
polinomi interpolanti di grado crescente. Come può essere scelta la matrice di
11interpolazione in modo da avere garantita la convergenza uniforme.
36. Fornisci un esempio di funzione f  C 1  a , b  e matrice di interpolazione tale che la
successione dei polinomi interpolatori non converge uniformemente ad f .
37. Individua tramite metodo grafico gli n=8 nodi di interpolazione nell’intervallo [-1,1]
corrispondenti agli zeri del polinomio di Chebichev di grado n=8.
38. Dopo aver definito la funzione di Runge, supponi di doverla approssimare mediante
polinomi interpolanti di grado crescente in [-5,5]. Individua una matrice di
interpolazione che non conduce a convergenza uniforme.
39. Dopo aver definito la funzione di Runge, supponi di doverla approssimare mediante
polinomi interpolanti di grado crescente in [-5,5]. Individua una matrice di
interpolazione che garantisca convergenza uniforme.
40. Se hai n nodi di Chebichev nell’intervallo [-1,1], come fai ad ottenere n nodi di
Chebichev nel generico intervallo [a,b].
41. Quali sono le difficoltà a cui conduce la classica interpolazione polinomiale.
42. In che cosa consiste l’approssimazione mediante funzioni spline.
43. Dai la definizione matematica di funzione spline.
44. Cosa sono le spline lineari a tratti. Che dimensione ha lo spazio delle splines lineari a
tratti costruite sull’insieme    a  x 0  x 1    x n  b  di n+1 nodi distinti.
45. Cosa sono le spline cubiche. Che dimensione ha lo spazio delle splines cubiche
costruite sull’insieme    a  x 0  x 1    x n  b  di n+1 nodi distinti.
46. Considerando lo spazio lineare delle funzioni spline di grado p sull’insieme
   a  x 0  x 1    x n  b  di n+1 nodi distinti, dimostrare che la dimensione
dello spazio, ossia il numero dei gradi di libertà, è n+p.
47. Cosa sono le funzioni spline interpolanti.
48. Quali sono i vantaggi dell’approssimazione mediante funzioni spline rispetto
all’approssimazione mediante polinomi.
49. Interpolando sull’insieme    a  x 0  x 1    x n  b  di n+1 nodi distinti con
spline lineari a tratti costruite sul medesimo insieme  , dire se la funzione spline
interpolatoria è unica.
50. Interpolando sull’insieme    a  x 0  x 1    x n  b  di n+1 nodi distinti con
spline cubiche costruite sul medesimo insieme  , dire se la funzione spline
interpolatoria è unica.
51. Supponi di dover approssimare una funzione f  C 2  a , b  mediante funzioni spline
lineari (p=1) interpolanti. Dai un esempio di matrice di interpolazione che garantisce
la convergenza uniforme.
52. Supponi di dover approssimare una funzione f  C 2  a , b  mediante funzioni spline
lineari (p=1) interpolanti. Dai un esempio di matrice di interpolazione che non
garantisce la convergenza uniforme.
53. In cosa consiste la migliore approssimazione.
54. Che differenze ci sono tra l’interpolazione e la migliore approssimazione.
55. Dai la formulazione matematica del problema della migliore approssimazione.
56. Dai un esempio di problema di migliore approssimazione.
57. Sotto quali ipotesi esiste la soluzione del problema della migliore approssimazione in
un generico spazio lineare normato.
58. Nel caso in cui si approssimi una funzione f  C  a , b  nel senso della migliore
approssimazione con norma infinito mediante un polinomio di grado fissato, è
garantita l’esistenza di tale polinomio? Tale polinomio è unico?
59. In che cosa consiste la migliore approssimazione nel senso dei minimi quadrati nel
12continuo.
60. In che cosa consiste la migliore approssimazione nel senso dei minimi quadrati nel
discreto.
61. Il sistema lineare V Va  y , dove V è la matrice di Vandermone, cosa permette di
dterminare. Cosa rappresenta il vettore a soluzione ? Che dimensioni hanno la
matrice V ed i vettori a e y ?
t
V t Va  V t y utile a determinare i coefficienti del
polinomio di grado n che approssima i dati ( x i , y i ) per i=0,...,m. Indicare come è
62. Si consideri il sistema lineare
definita la matrice V ed il vettore y, e le loro dimensioni.
V t Va  V t y utile a determinare i coefficienti del
polinomio di grado n che approssima i dati ( x i , y i ) per i=0,...,m. Se m=n il
63. Si consideri il sistema lineare
polinomio ottenuto conicide con il polinomio di interpolazione ? E se m<n ?
64. Scrivere il sistema lineare nella forma V Va  V y (senza risolverlo) utile a
determinare i coefficienti della retta ai minimi quadrati approssimante i punti
P1=(0,0), P2=(1,1), P3=(3,4), P4=(4,3).
t
t
65. Scrivere il sistema lineare nella forma V Va  V y (senza risolverlo) utile a
determinare i coefficienti della parabola ai minimi quadrati approssimante i punti
P1=(0,0), P2=(1,1), P3=(3,4), P4=(4,3).
t
t
Integrazione Numerica
1. A cosa servono le formule di quadratura ? Qual è la forma generale di una formula di
quadratura ?
2. Quando una formula di quadratura ha grado di esattezza r ?
3. Perché la somma dei pesi di una formula di quadratura vale b a ?
4. Scelti i nodi di quadratura x 0 , x 1 , ..., x n , illustrare come possono essere determinati i
pesi  0 ,  1 , ...,  n in modo tale che la formula di quadratura ottenuta abbia grado
di grado di esattezza n mediante il metodo dei coefficienti indeterminati.
5. Scelti tre nodi di quadratura x 0 , x 1 , x 3 , scrivere il sistema lineare nella forma
V t   c (senza effettuare i calcoli, né risolverlo) utile a determinare i pesi
 0 ,  1 ,  3 della formula di quadratura con grado di esattezza 3 secondo il metodo
dei coefficienti indeterminati.
6. Cosa si intende per formula di quadratura interpolatoria.
7. Dimostra che, scelti i nodi di quadratura x 0 , x 1 , ..., x n , in una formula di quadratura
interpolatoria i pesi  0 ,  1 , ...,  n sono i valori degli intergali definiti dei polinomi
L i (x ) , i  0 ,..., n , della base di Lagrange.
8. Spiega perché le formule di quadratura interpolatorie hanno gardo di esattezza
almeno n.
9. Cosa sono le formule di Newton-Cotes ?
10. Quando una formula di Newton-Cotes è detta chiusa e quando è detta aperta?
11. Dai un esempio di formula di Newton-Cotes aperta e un esempio di formula di
Newton-Cotes chiusa.
12. Calcola in maniera esplicita i pesi della formula di Newton-Cotes semplice dei
13rettangoli.
13. Calcola in maniera esplicita i pesi della formula di Newton-Cotes semplice dei
trapezi.
14. Scrivere gli integrali che permettono il calcolo dei pesi della formula di Newton-
Cotes semplice di Cavalieri-Simpson (non occorre svolgere i calcoli degli integrali).
15. Si approssimi mediante la formula di Newton-Cotes semplice dei rettangoli il valore


dell’integrale sin x dx .
0
16. Si approssimi mediante la formula di Newton-Cotes semplice dei trapezi il valore


dell’integrale sin x dx .
0
17. Si approssimi mediante la formula di Newton-Cotes semplice di Cavalieri-Simpson il


valore dell’integrale sin x dx .
0
18. Si approssimi mediante la formula di Newton-Cotes semplice dei rettangoli il valore


dell’integrale exp x dx .
0
19. Si approssimi mediante la formula di Newton-Cotes semplice dei trapezi il valore


dell’integrale exp x dx .
0
20. Si approssimi mediante la formula di Newton-Cotes semplice di Cavalieri-Simpson il


valore dell’integrale exp x dx .
0
21. Spegare perché le formule di Newton Cotes hanno i pesi simmetrici, ossia
 i   n i , per i  0 ,...,  n / 2  .
22. In generale, essendo formule di quadratura interpolatorie, le formule di Newton Cotes
di grado n hanno grado di esattezza n. Spiegare perché, se n è pari, allora la
corrispondente formula di Newton Cotes ha grado di esattezza n+1.
23. Perché generalmente non vengono mai usate formule di Newton-Cotes semplici di
grado elevato? Quale strategia si adotta per aumentare la precisione delle formule di
quadratura.
24. Scrivere e illustrare la formula di Newton-Cotes composita dei rettangoli.
25. Scrivere e illustrare la formula di Newton-Cotes composita dei trapezi.
26. Scrivere e illustrare la formula di Newton-Cotes composita di Simpson.
27. Senza effettuare i calcoli, si approssimi mediante la formula di Newton-Cotes


composita dei rettangoli il valore sin x dx suddividento l’intervallo di integrazione
0
in 5 parti.
28. Senza effettuare i calcoli, si approssimi mediante la formula di Newton-Cotes

composita dei trapezi il valore
 sin x dx
suddividento l’intervallo di integrazione in
0
5 parti.
1429. Senza effettuare i calcoli, si approssimi mediante la formula di Newton-Cotes

composita di Simpson il valore
 sin x dx
suddividento l’intervallo di integrazione in
0
6 parti.
30. Senza effettuare i calcoli, si approssimi mediante la formula di Newton-Cotes

composita dei rettangoli il valore
 exp x dx
suddividento l’intervallo di integrazione
0
in 5 parti.
31. Senza effettuare i calcoli, si approssimi mediante la formula di Newton-Cotes

composita dei trapezi il valore
 exp x dx
suddividento l’intervallo di integrazione in
0
5 parti.
32. Senza effettuare i calcoli, si approssimi mediante la formula di Newton-Cotes

composita di Simpson il valore
 exp x dx
suddividento l’intervallo di integrazione in
0
6 parti.

 sin x dx
33. Qual è l’errore massimo che si commette approssimando
mediante la
0
formula
di Newton-Cotes
M
E 0 ( f )  2 ( b a ) 3 .
24
semplice
dei
rettangoli
-
si
ricordi
che

34. Qual è l’errore massimo che si commette approssimando
 exp x dx
mediante la
0
formula di Newton-Cotes semplice dei trapezi - si ricordi che E 1 ( f ) 
M 2
( b a ) 3 .
12

35. Qual è l’errore massimo che si commette approssimando
 cos x dx
mediante la
0
formula
di Newton-Cotes
M 4
E 2 ( f ) 
(( b a ) / 2 ) 5 .
90
semplice
di
Simpson
-
si
ricordi
che

 x
36. Qual è l’errore massimo che si commette approssimando
2
dx mediante la
0
formula
di Newton-Cotes
M 4
E 2 ( f ) 
(( b a ) / 2 ) 5 .
90
semplice
di
Simpson
-
si
ricordi
che


 6
37. Quanti nodi di quadratura sono sufficienti ad approssimare sin x dx a meno di 10
0
utilizzando la la formula di Newton-Cotes composita dei rettangoli - si ricordi che
M
E 0 ( C ) ( f )  2 ( b a ) h 2 .
24
15

 6
38. Quanti nodi di quadratura sono sufficienti ad approssimare cos x dx a meno di 10
0
utilizzando la la formula di Newton-Cotes composita dei trapezi - si ricordi che
M
E 1 ( C ) ( f )  2 ( b a ) h 2 .
12


39. Quanti nodi di quadratura sono sufficienti ad approssimare exp x dx a meno di
0
 6
10 utilizzando la la formula di Newton-Cotes composita di Simpson - si ricordi che
E 2 ( C ) ( f ) 
M 4
( b a ) h 4 .
180
2

2
 6
40. Quanti nodi di quadratura sono sufficienti ad approssimare x dx a meno di 10
0
utilizzando la la formula di Newton-Cotes composita di Simpson - si ricordi che
M
E 2 ( C ) ( f )  4 ( b a ) h 4 .
180
Equazioni non lineari
1. Cosa si intende per equazione non lineare e sistema di equazioni non lineari. Fornire
due esempi.
2. In che modo sono definiti i metodi per la risoluzione di equazioni non lineari.
3. In assenza di errori di arrotondamento, i metodi per la risoluzione di equazioni non
lineari consentono di ottenere una soluzione esatta od una soluzione approssimata?
4. Cosa si intende per errore al passo k.
5. Spiega e scrivi l’algoritmo del metodo di bisezione.
6. Scelta una funzione a piacere, mostra graficamente il funzionamento del metodo di
bisezione (esegui tre iterazioni).
7. Spiega e scrivi l’algoritmo del metodo Regula Falsi.
8. Scelta una funzione a piacere, mostra graficamente il funzionamento del metodo
Regula Falsi (esegui tre iterazioni).
9. Cosa si intende con il termine linearizzazione.
10. Tramite la serie di Taylor arrestata al primo termine, scrivi la formula analitica per un
passo del metodo di Newton.
11. Spiega e scrivi l’algoritmo del metodo di Newton.
12. Scelta una funzione a piacere, mostra graficamente il funzionamento del metodo di
Newton (esegui tre iterazioni).
13. Cosa sono i metodi quasi-Newton.
14. Spiega e scrivi l’algoritmo del metodo delle corde.
15. Scelta una funzione a piacere, mostra graficamente il funzionamento del metodo delle
corde (esegui tre iterazioni).
16. Spiega e scrivi l’algoritmo del metodo delle secanti.
17. Scelta una funzione a piacere, mostra graficamente il funzionamento del metodo delle
secanti (esegui tre iterazioni).
18. I metrodi Regula Falsi e secanti hanno due formulazioni molto simili. Quali sono le
differenze tra i due metodi.
19. Quando un metodo iterativo è convergente.
20. Quando un metodo iterativo ha ordine p.
1621. Un metodo iterativo di ordine 2 è sempre più rapido di un metodo di ordine 1? Se no,
fornire un contresempio.
22. Un metodo iterativo di ordine 2 è generalmente più rapido di un metodo di ordine 1?
23. Il metodo di bisezione converge sempre? Perché?
24. Se esiste, fornire un esempio in cui il metodo di bisezione non converge.
25. Il metodo di Newton converge sempre? Perché?
26. Se esiste, fornire un esempio in cui il metodo di Newton non converge.
b a
27. Dimostra che per il metodo di bisezione vale e k  k .
2
28. Nel metodo di bisezione, quante iterazioni sono necessarie per ottenere un errore al
passo k minore di 1/1000 di [a,b].
29. Dimostra che, se f ' ' (  )  0 , allora il metodo di Newton ha ordine 2 in un intorno
della radice  .
30. La convergenza del metodo di bisezione dipende dal valore iniziale x 0 , ossia può
convergere o non convergere in funzione di x 0 ? Se si, fornire un esempio di non
convergenza.
31. La convergenza del metodo di Newton dipende dal valore iniziale x 0 , ossia può
convergere o non convergere in funzione di x 0 ? Se si, fornire un esempio di non
convergenza.
32. Spiegare, aiutandosi con un grafico, le condizioni (i) f(a)f(b)<0, (ii) f’(x) ≠ 0,
x[a,b], (iii) f’’(x)>=0 oppure f’’(x)<=0 x[a,b], (iv) |f(a)/f’(a)|<b-a e
|f(b)/f’(b)|<b-a del teorema di convergenza del metodo di Newton studiato a lezione.
33. Dimostra perché il
metodo di
Newton
applicato
alla
funzione
 x
se x  0
è stazionario. Inoltre spiega il funzionamento del metodo
f ( x )  
  x se x  0
graficamente.
34. Dimostra perché

 3 x 2 se
f ( x )   3 2

 x se
graficamente.
35. Dimostra perché
 3 x
se
f ( x )   3
  x se
il
metodo
di
Newton
applicato
alla
funzione
x  0
è convergente. Inoltre spiega il funzionamento del metodo
x  0
il
metodo di
Newton
applicato
alla
funzione
x  0
non è convergente. Inoltre spiega il funzionamento del
x  0
metodo graficamente.
17
$\fi$
