#Tema 6: Rectes en el pla

Aquest curs començarem amb la [geometria analítica](https://es.wikipedia.org/wiki/Geometr%C3%ADa_anal%C3%ADtica) en el pla. Aquesta part de la geometria estudia els objectes geoomètrics en el pla cartesià.

##Equacions de la recta

En cursos anteriors ja havíem representat rectes en el pla cartesià mitjançant la seva expressió afí $y=f(x)=mx+n$, on $m$ era el pendent de la recta i $n$ l'ordenada a l'origen. Aquest curs veurem altres expressions de la recta que ens seran útils en situacions analítiques diferents.

### Equació vectorial
Podem expressar qualsevol punt d'una recta donat un punt qualsevol d'aquesta i la seva direcció. Sigui $P=(x_0,y_0)$ un punt qualsevol d'una recta $r$ i $\vec{v}=(v_1,v_2)$ un vector amb la direcció de la recta, qualsevol punt $X=(x,y)$ d'aquesta recta es pot expressar com:

>$$(x,y)=(x_0,y_0)+\lambda(v_1,v_2)$$

on $\lambda$ és un nombre real. Anomenem aquesta expressió l'**equació vectorial de la recta**, i el vector $\vec{v}=(v_1,v_2)$ és el seu **vector director**.

<iframe scrolling="no" src="https://www.geogebra.org/material/iframe/id/2403711/width/1600/height/951/border/888888/rc/false/ai/false/sdz/true/smb/false/stb/false/stbh/true/ld/false/sri/true/at/auto" width="800px" height="500px" style="border:0px;"> </iframe>

### Equacions paramètriques

Si desenvolupem l'equació vectorial component a component, obtenim les **equacions paramètriques de la recta**:

>$$\begin{cases} x = x_0+\lambda v_1 \\ y = y_0 + \lambda v_2
\end{cases}$$

### Equació contínua

Si aïllem el paràmetre $\lambda$ de les dues equacions i les igualem, obtenim l'**equació contínua de la recta**:

>$$\frac{x-x_0}{v_1}=\frac{y-y_0}{v_2}$$

Aquesta forma de l'equació només és possible si les coordenades del vector director de la recta $\vec{v}=(v_1,v_2)$ són diferents de zero.

### Equació general o implícita

Si continuem operant, i ho passem tot al costat esquerra i igualem a zero obtenim que:

$$v_2(x-x_0)=v_1(y-y_0)\rightarrow v_2 x-v_1 y-v_2 x_0 + v_1 y_0=0$$

I si fem les definicions següents:

$$\begin{cases} A \equiv v_2 \\
B \equiv -v_1 \\
C \equiv (-v_2 x_0+v_1 y_0)
\end{cases}
$$

tenim l'**equació general o implícita** de la recta:

>$$Ax+By+C=0$$

Per trobar un punt que pertanyi a aquesta recta n'hi ha prou per donar un valor arbitrari a $x$ i calcular-ne la $y$. El vector director de la recta serà (tenint en compte la substitució anteriorment feta):

$$\vec{v}=(-B,A)$$


### Equació explícita

A partir d'aquí podem aïllar $y$ en un costat i trobar l'equació explícita de la recta amb la que començàvem el capítol:

$$y=-\frac{A}{B}x-\frac{C}{B}$$

Si redefinim els coeficients obtenim:

$$y=mx+n \begin{cases} m \equiv -\frac{A}{B} \\
n \equiv -\frac{C}{B} \\
\end{cases}
$$

Anem a veure ara què representa el pendent $m$:

$$m=-\frac{A}{B}=\frac{v_2}{v_1}$$

El pendent és el quocient entre les components $y$ i $x$ del vector director de la recta, i si mirem el gràfic següent:
<iframe scrolling="no" src="https://www.geogebra.org/material/iframe/id/2413717/width/1920/height/933/border/888888/rc/false/ai/false/sdz/true/smb/false/stb/false/stbh/true/ld/false/sri/true/at/auto" width="800px" height="500px" style="border:0px;"> </iframe>

Veiem que **el pendent $m$ és la tangent de l'angle que forma el vector director de la recta amb l'eix $OX$**. Això vol dir que per rectes paral.leles a l'eix $OX$ el seu pendent serà $tg (0^o)=0$ i per rectes paral.leles a l'eix $OY$ el seu pendent serà màxim: $tg ( 90^0)=\infty$.



##Posicions relatives entre dues rectes
### Rectes paral.leles
En cursos anteriors havíem vist que dues rectes eren paral.leles si tenien el mateix pendent, o sigui, igual $m$. Ara que ja coneixem els vectors també podem dir que dues rectes són paral.leles **si tenen el mateix vector director o si els seus vectors directors són linealment dependents** (l'un és l'altre multiplicat per un nombre).
Anem-ho a veure algebraicament:

\begin{align}
    r:& \quad Ax+By+C=0 \Rightarrow \vec{v_r}=(-B,A) \Rightarrow m_r=\frac{A}{-B}=\frac{-A}{B}\\
    s:& \quad A^\prime x+ B^\prime y+ C^ \prime= 0 \Rightarrow \vec{v_s}=(-B^\prime,A^\prime) \Rightarrow m_s=\frac{A^\prime}{-B^\prime}=\frac{-A^\prime}{B^\prime}
\end{align}

Seran **paral.leles** si:

\begin{align}
m_r&=m_s\\
-\frac{A}{B}&=-\frac{A^\prime}{B^\prime} \\
\frac{A}{A^\prime}&=\frac{B}{B^\prime}
\end{align}

Òbviament si aquesta igualtat no es compleix les rectes seran **secants** i caldrà buscar el seu punt de tall resolent el sistema d'equacions.

### Rectes coincidents

Si a més a més es compleix:

$$\frac{A}{A^\prime}=\frac{B}{B^\prime}=\frac{C}{C^\prime}$$

$r$ i $s$ seran la mateixa recta.

**Exemple 1**

Troba l'equació de la recta $s$ que passa pel punt $P(4,3)$ i és paral.lela a la recta $r$: $5x+3y+6=0$.

El vector director de la recta $r$ és $\vec{v_r}=(-B,A)=(-3,5)$. Si la recta $s$ és paral.lela necessàriament ha de tenir el mateix vector director, pertant, $A$ i $B$ seran les mateixes:

$$5x+3y+C=0$$

La $C$ la trobarem subtituint a l'equació el punt donat:

$$P(3,4)\Rightarrow 5\cdot 4+3\cdot 3+C=0 \Rightarrow C=-29$$

Per tant, l'equació de la recta és: $5x+3y-29=0$
<iframe scrolling="no" src="https://www.geogebra.org/material/iframe/id/2450005/width/1938/height/951/border/888888/rc/false/ai/false/sdz/true/smb/false/stb/false/stbh/true/ld/false/sri/true/at/auto" width="600px" height="300px" style="border:0px;"> </iframe>


### Rectes perpendiculars
## Angle entre dues rectes

##Distàncies
### Distància entre dos punts
### Distància d'un punt a una recta
### Distància entre dues rectes
