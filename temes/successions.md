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

**Exemple 3**

Troba el terme general de la successió: $2,4,6,8,...$ troba també la suma dels $50$ primers nombres parells.

Per la successió anterior veiem que és aritmètica de diferència $d=2$. Per tant, anem a trobar-ne el terme general:

\begin{align}
a_n&=a_1+(n-1)d\\
a_n&=2+(n-1)2\\
a_n&=2n
\end{align}

Per trobar la suma dels 50 primers nombres parells només cal aplicar la fòrmula:

\begin{align}
S_n&=\frac{a_1+a_n}{2}\cdot n \\
S_n&=\frac{2+2n}{2}\cdot n\\
S_n&=(1+n)\cdot n=n^2+n\\
S_50&=50^2+50=2550
\end{align}

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

**Exemple 4**

Troba el terme general de la successió: $2,6,18,54,...$ troba també la suma dels $10$ primers termes de la successió

Per la successió anterior veiem que és geomètrica de raó $r=3$. Per tant, anem a trobar-ne el terme general:

\begin{align}
a_n&=a_1 \cdot r^{n-1}\\
a_n&=2\cdot 3^{n-1}\\
\end{align}

Per trobar la suma dels 10 primers termes només cal aplicar la fòrmula:

\begin{align}
S_n&=\frac{a_1(r^n-1)}{r-1}\\
S_n&=\frac{2(3^n-1)}{2}\\
S_n&=3^n-1\\
S_10&=3^10-1=59048
\end{align}

###Suma dels infinits termes amb $|r|<1$

Recordem l'expressió de la suma dels $n$ termes d'una progressió geomètrica:

$$S_n=\frac{a_1(r^n-1)}{r-1}$$

Si $n$ es fa molt gran, com que $|r|<1$, quan l'elevem a un nombre molt gran, $r^n\rightarrow 0$. Per tant, la **suma dels infinits termes** d'una progressió geomètrica si $|r|<1$ esdevé:

>$$S_{\infty}=\frac{-a_1}{r-1}=\frac{a_1}{1-r}$$

**Exemple 5**

Troba el terme general de la successió: $\frac{1}{2},\frac{1}{4}, \frac{1}{8}, \frac{1}{16}...$ troba també la suma dels $\infty$ termes.

Per la successió anterior veiem que és geomètrica de raó $r=\frac{1}{2}$. Per tant, anem a trobar-ne el terme general:

\begin{align}
a_n&=a_1 \cdot r^{n-1}\\
a_n&=\frac{1}{2}\cdot \big(\frac{1}{2}\big)^{n-1}\\
a_n&=\big(\frac{1}{2}\big)^n
\end{align}

Per trobar la suma dels $\infty$ primers termes només cal aplicar la fòrmula:

\begin{align}
S_{\infty}&=\frac{a_1}{1-r}\\
S_{\infty}&=\frac{\frac{1}{2}}{1-\frac{1}{2}}\\
S_{\infty}&=2\\
\end{align}


##Successions monòtones

Anem a veure com són les successions estudiant-ne els seus termes. Ens podem trobar en diferents casos:

1. Diem que una successió $a_n$ és **creixent** si $a_{n+1}>a_{n}$ per a qualsevol valor de $n$.
2. Diem que una successió $a_n$ és **decreixent** si $a_{n+1}<a_{n}$ per a qualsevol valor de $n$.
3. Diem que una successió $a_n$ és **constant** si $a_{n+1}=a_{n}$ per a qualsevol valor de $n$.
4. Diem que una sucessió és **oscil.lant** si per exemple $a_1<a_2$, $a_2>a_3$, $a_3<a_4$, $a_4>a_5$, etc.
5. Podem trobar també sucessions que no siguin cap de les anteriors.

>Si una successió és creixent o decreixent direm que és una sucessió **monótona**.

També podeu sentir que una sucessió és **estrictament** creixent (o decreixent). Ho serà si $a_{n+1}>a_n$ ($a_{n+1}<a_n$), en canvi si es compleix que $a_{n+1}\ge a_n$ ($a_{n+1} \le a_n$) llavors diem que la successió és creixent (o decreixent).

**Exemple 6**

Demostreu que la successió $a_n=\frac{n}{n+1}$ és monòtona creixent.

Per fer-ho, hem de veure que:

\begin{align}
a_{n+1}&\ge a_n\\
\frac{n+1}{(n+1)+1} &\ge \frac{n}{n+1}\\
\frac{n+1}{n+2} &\ge \frac{n}{n+1}\\
(n+1)^2 &\ge n(n+2)\\
n^2+2n+1&\ge n^2+n\\
1&\ge0
\end{align}

Veiem que sí que es compleix la desigualtat. Per tant, és una successió monòtona creixent.

##Successions fitades

Anem a definir un parell de conceptes:

1. Diem que una successió està **fitada inferiorment** si tots els membres de la successió són més grans o iguals que un nombre real $k$: $a_n\ge k, \forall n \in \mathbb{N}, k\in \mathbb{R}$.Diem que $k$ és una **fita inferior** de la successió.
2. Diem que una successió està **superiorment** si tots els membres de la successió són més petits o iguals que un nombre real $k$: $a_n\le k, \forall n \in \mathbb{N}, k\in \mathbb{R}$. Diem que $k$ és una **fita superior** de la successió.
3. Si una successió està fitada superiorment i inferiorment diem que és una successió **fitada**.
4. Una successió **no està fitada** si per qualsevol valor de $k$ arbitràriament gran podem trobar un valor de $n$ tal que $|an|>k$: $\forall k \in \mathbb{R} \exists n\in \mathbb{N} | |a_n|>k$.

**Exemple 7**

Demostreu que la successió $a_n=\frac{n^2+1}{n}$ no està fitada.

Per demostrar això hem de veure que donat un valor de $k$ arbitràriament gran sempre podem trobar un valor de $n$ pel qual el terme $a_n$ sigui més gran que $k$.

Veiem que:

$$a_n=\frac{n^2+1}{n}=n+\frac{1}{n}$$

Dels dos sumands anteriors, ja veiem que el segon es fa molt petit fins arribar quasi a $0$, però el primer sumand, $n$ pot créixer arbritràriament. Per tant, acabem de demostrar que la successió anterior no està fitada.


##Límit d'una succesió


###Operacions amb Successions



###Càlcul de límits
