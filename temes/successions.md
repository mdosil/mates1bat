#Tema 8: Successions

##Introducció

Segur que tots coneixeu la [successió de Fibonacci](https://ca.wikipedia.org/wiki/Successi%C3%B3_de_Fibonacci), que comença amb dos uns i cada terme s'obté sumant els dos anteriors:

$$1,1,3,5,8,13,21,34,55,...$$

En aquest tema estudiarem en profunditat el món de les successions o també conegudes com a progressions. Segur que algunes coses ja us sonaran de l'eso, però hi afegirem coses noves com és ara el concepte de *límit* que apareixerà també al llarg dels temes següents.

###Definició

Una successió és una llista ordenada de nombres reals. De fet, tècnicament és una **aplicació entre el conjunt dels nombres naturals i els nombres reals**, de tal manera que a cada nombre natural $n$ i fa correspondre un nombre real $a_n$:

\begin{align}
f:\mathbb{N} &\rightarrow \mathbb{R}\\
n &\rightarrow a_n
\end{align}

$n$ és l'índex de l'element de la successió que estem parlant (lloc, per entendre'ns), i $a_n$ és el **terme** de la successió que ocupa el lloc $n$.



**Exemple 1**

Anem a veure alguns exemples de successions:

1. $2,4,6,8,10,12,14,.....$
2. $3,6,12,24,48,96,......$
3. $1, \frac{1}{2}, \frac{1}{3}, \frac{1}{4}, \frac{1}{5},...$

En la primera successió, $a_1=2$, $a_2=4$ i així successivament. En la segona, $a_1=3$ i $a_2=6$ i en la tercera, $a_1=1$, $a_2=\frac{1}{2}$.

###Terme general

El terme general d'una successió és l'expressió algebraica que em dóna el terme $a_n$ en funció del paràmetre $n$. D'aquesta manera, el terme general ens permet trobar qualsevol terme de la successió. Només ens cal substituir $n$ pel nombre natural desitjat.

**Exemple 2**

En l'exemple anterior, podem trobar el terme general fàcilment sense haver de pensar gaire:

1. $a_n=2n$
2. $a_n=3\cdot 2^{n-1}$
3. $a_n=\frac{1}{n}$


De fet, una sucessió es pot definir de 3 maneres diferents:

1. Donant una sèrie de termes, com a l'exemple 1
2. Donant el terme general
3. Donant una *relació de recurrència*, com a la sucessió de Fibonacci, en la qual ens permet obtenir un terme a partir dels anteriors

A continuació veurem les característiques de dues de les successions més típiques, les aritmètiques i les geomètriques.

##Successions aritmètiques

Una successió aritmètica és aquella que cada terme s'obté sumant una quantitat fixa anomenada **diferència** a l'anterior:

$$a_n=a_{n-1}+d$$

Donada una successió de termes, sabrem que és una progressió aritmètica si restant dos termes consecutius sempre obtenim el mateix valor.

###Terme general

Anem a veure com obtenim el terme general d'una progressió aritmètica.

\begin{align}
a_1&=a_1\\
a_2&=a_1+d\\
a_3&=a_2+d=a_1+2d\\
a_4&=a_3+d=a_1+3d\\
&................\\
a_n&=a_{n-1}+d=a_1+(n-1)d
\end{align}

Per tant, el terme general d'una successió aritmètica és:

>$$a_n=a_{n-1}+d=a_1+(n-1)d$$

###Suma dels $n$ termes

De la mateixa manera podem deduir la fòrmula de la suma dels $n$ termes d'una successió geomètrica. Per sumar els $n$ primers termes d'una successió aritmètica tenim:

\begin{align}
S_n&=a_1+a_2+a_3+...+a_{n-2}+a_{n-1}+a_n\\
S_n&=a_n+a_{n-1}+a_{n-2}+...+a_3+a_2+a_1\\
\hline
2S_n&=(a_1+a_n)+(a_2+a_{n-1})+(a_3+a_{n-2})+...+(a_{n-2}+a_3)+(a_{n-1}+a_2)+(a_1+a_n)
\end{align}

Fixem-nos amb les sumes dels termes entre parèntesi. Veiem que la primera suma i la última són iguals. Anem a veure què passa amb les del mig:

\begin{align}
a_2&=a_1+d\\
a_{n-1}&=a_n-d\\
\hline
a_2+a_{n-1}&=a_1+a_n
\end{align}

El mateix passa amb els altres termes:


\begin{align}
a_3&=a_2+d\\
a_{n-2}&=a_{n-1}-d\\
\hline
a_3+a_{n-2}&=a_2+a_{n-1}=a_1+a_n
\end{align}

Per tant, si anem sumant termes equidistants de la successió sempre ens dóna com a resultat $a_1+a_n$. Amb això, aplicat a la primera operació obtenim:

$$2S_n=(a_1+a_n)n$$

Per tant, la **suma dels n termes d'una successió aritmètica és**:

>$$S_n=\frac{a_1+a_n}{2}\cdot n$$

##Successions geomètriques

Una successió geomètrica és una successió de nombres reals en els quals el quocient entre dos termes consecutius de la successió és constant i s'anomena **raó**. El que és el mateix, obtenim un terme multiplicant l'anterior per la raó:

$$a_{n+1}=a_n\cdot r$$

###Terme general

Anem a veure com obtenim el terme general d'una progressió geomètrica.

\begin{align}
a_1&=a_1\\
a_2&=a_1\cdot r\\
a_3&=a_2\cdot r=a_1 \cdot r^2\\
a_4&=a_3\cdot r=a_1\cdot r^3\\
&................\\
a_n&=a_1 \cdot r^{n-1}
\end{align}

Per tant, el terme general d'una successió geomètrica és:

>$$a_n=a_1 \cdot r^{n-1}$$

###Suma dels $n$ termes

Anem a deduir ara la suma dels $n$ termes d'una successió geomètrica:

$$S_n=a_1+a_2+a_3+...+a_{n-2}+a_{n-1}+a_n$$

Multipliquem a banda i banda per la raó $r$:

\begin{align}
S_n\cdot r&=a_1\cdot r+a_2\cdot r+a_3\cdot r+...+a_{n-2}\cdot r+a_{n-1}\cdot r+a_n \cdot r\\
S_n\cdot r&=a_2+a_3+a_4+...+a_{n-1}+a_n+a_n\cdot r
\end{align}

Si restem les dues expressions anteriors:

\begin{align}
S_n\cdot r&=a_2+a_3+a_4+...+a_{n-1}+a_n+a_n\cdot r\\
-S_n&=-a_1-a_2-a_3-...-a_{n-2}-a_{n-1}-a_n\\
\hline
S_n\cdot r-S_n&=-a_1+a_n\cdot r\\
S_n(r-1)&=a_n\cdot r-a_1
\end{align}

Per tant, la suma dels $n$ termes d'una progressió geomètrica és:

>$$S_n=\frac{a_n\cdot r-a_1}{r-1}=\frac{a_1\cdot r^n-a_1}{r-1}=\frac{a_1(r^n-1)}{r-1}$$

###Suma dels infinits termes amb $|r|<1$

Recordem l'expressió de la suma dels $n$ termes d'una progressió geomètrica:

$$S_n=\frac{a_1(r^n-1)}{r-1}$$

Si $n$ es fa molt gran, com que $|r|<1$, quan l'elevem a un nombre molt gran, $r^n\rightarrow 0$. Per tant, la **suma dels infinits termes** d'una progressió geomètrica si $|r|<1$ esdevé:

>$$S_{\infty}=\frac{-a_1}{r-1}=\frac{a_1}{1-r}$$



##Successions monòtones

##Límit d'una successió


###Operacions amb Successions

###Límit d'una successió

###Càlcul de límits
