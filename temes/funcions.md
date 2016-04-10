#Tema 8: Funcions

##Aplicació entre dos conjunts

S'anomena aplicació entre un conjunt $A$ i un conjunt $B$ a tot criteri o llei mitjançant la qual a cada element $a \in A$ li fa correspondre un **únic** element $b \in B$:

\begin{align}
f:& A \rightarrow B \\
&a \rightarrow b
\end{align}

$A$ és el conjunt inicial o de partida i i $B$ és el conjunt final o d'arribada. $a$ és l'element original o antiimatge, i $b$ és l'element final o imatge.

No tots els elements del conjunt final són imatges. Només o són els que tenen associat algun element del conjunt inicial.

**Exemple 1**

Considerem l'aplicació $f$ entre el conjunt dels naturals $\mathbb{N}$ i els racionals $\mathbb{Q}$ de tal manera que a cada nombre natural $n$ li fa correspondre la meitat de la suma de $n$ i 5. Doneu alguns elements del conjunt inicial i del conjunt final. Doneu algun element que no pertanyi al conjunt inicial. Doneu algun element que no pertanyi al conjunt final.

\begin{align}
f:& \mathbb{N} \rightarrow \mathbb{Q} \\
&n \rightarrow f(n)=\frac{n+5}{2}\\
&1 \rightarrow 3\\
&2 \rightarrow \frac{7}{2}\\
&3 \rightarrow 4\\
&.\\
&.\\
&.\\
\end{align}

Per exemple el $-5$ no pertany al conjunt inicial perquè no és natural, i el $\frac{9}{4}$ no pertany al conjunt final perquè no té antiimatge:

$$\frac{9}{4}=\frac{n+5}{2}\Rightarrow n=-\frac{1}{2}$$

###Tipus d'aplicacions

####Aplicació injectiva

Una aplicació és injectiva quan els elements del conjunt final tenen **com a màxim** una antiimatge:

>f és injectiva $\Longleftrightarrow f(a)=f(b)\rightarrow a=b$

Això és, si hi ha dues imatges iguals necessàriament han de tenir la mateixa antiimatge.

**Exemple 2**

Demostra que l'aplicació de l'exemple 1 és injectiva.

Anem a calcular la imatge de dos punts diferents, els igualem i arribarem a la conclusió que necessàriament les antiimatges han de ser iguals:

$$
\left.\begin{aligned}
f(a)=\frac{a+5}{2}\\
f(b)=\frac{b+5}{2}\\
\end{aligned}
\right\}
\rightarrow f(a)=f(b)\rightarrow \frac{a+5}{2}=\frac{b+5}{2} \rightarrow a+5=b+5 \rightarrow a=b
$$

####Aplicació exhaustiva

Una aplicació és exhaustiva quan tot element del conjunt final té **com a mínim** una antiimatge.

> f és exhaustiva $\Longleftrightarrow \forall y \in B \quad \exists x \in A \quad | f(x)=y$

**Exemple 3**

Demostra que l'aplicació del primer exemple no és exhaustiva.

\begin{cases}
f(x)=y\\
\frac{x+5}{2}=y\\
x+5=2y\\
x=2y-5
\end{cases}

i si prenem $y=1$ veiem que $x=-3$, que no és un nombre natural. Per tant, hem trobat un punt que no té antiimatge.

####Aplicació bijectiva

>Una aplicació és bijectiva quan és injectiva i exhaustiva alhora.


##Definició de funció real de variable real

Una funció real de variable real és una aplicació entre un subconjunt $A$ de nombres reals $\mathbb{R}$ i el conjunt $\mathbb{R}$. Veiem-ne un exemple:

\begin{align}
f:& A \rightarrow \mathbb{R} \\
f:& {\mathbb{R}_0}^+ \rightarrow \mathbb{R} \\
& x \rightarrow y=f(x)=+\sqrt{x}
&1 \rightarrow 1\\
&\frac{2}{3} \rightarrow \sqrt{\frac{2}{3}}\\
&.\\
&.\\
&.\\
\end{align}



##Domini d'una funció

Anomenem domini d'una funció al conjunt de tots els elements originals, és a dir, el conjunt o subconjunt dels nombres reals que aplicant l'equació associada obtenim una imatge real.

###Domini de funcions polinòmiques

El domini de funcions polinòmiques és tot el conjunt dels nombres reals:

$$D=\mathbb{R}$$

###Domini de funcions amb fraccions algebraiques

Aquestes funcions són del tipus: $y=f(x)=\frac{P(x)}{Q(x)}$ on $P(x)$ i $Q(x)$ són polinomis.

$$D=\mathbb{R}-\{\text{zeros del denominador}\}$$

**Exemple 4**

Calcula el domini de la funció $y=f(x)=\frac{x^2-2}{x^2-2x+1}$.

$$x^2-2x+1=0 \rightarrow x=\pm 1$$

$$D=\mathbb{R}-\{1\}$$

###Domini de funcions irracionals

Són funcions del tipus:

$$y=f(x)=\sqrt[i]{P(x)}$$

si $i$ és parell el domini seran tots els reals que facin el radicand positiu i si $i$ és senar, el domini seran tots els nombres reals.

**Exemple 5**

Calcula el domini de la funció $y=f(x)=\sqrt{x^2-1}$

\begin{align}
x^2-1 \ge 0\\
x \in (- \infty, -1] U [1, +\infty)\\
D=\mathbb{R}-(-1,1)
\end{align}




##Recorregut d'una funció

El recorregut d'una funció és el conjunt de totes les imatges. També s'anomena conjunt imatge. És difícil veure quin és el recorregut a partir de l'equació d'una funció. El millor és fer-ho a partir de la gràfica i projectar-la sobre l'eix $y$. El recorregut serà l'interval de l'eix $y$ que queda *pintat* per la gràfica.


##Funcions a trossos



##Operacions amb funcions

###Suma i diferència de funcions

###Producte de funcions

###Quocient de funcions

###Composició de funcions

##Funció inversa

###Teorema

###Càlcul de la inversa

###Representació gràfica de la inversa
