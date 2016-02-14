#Tema 7: Llocs geomètrics

##Introducció

Un lloc geomètric és un conjunt de punts que compleixen una certa propietat. Per exemple, la bisectriu d'un segment és el lloc geomètric dels punts que equidisten dels 2 extrems del segment. En aquest tema estudiarem 4 llocs geomètrics: la circumferència, l'el.lipse, la paràbola i l'hipèrbola. Segurament alguns d'aquests llocs geomètrics ja els coneixeu des de primària, però els estudiarem des d'una perspectiva geomètrica diferent.

Aquests llocs geomètrics també s'anomenen [Còniques](https://ca.wikipedia.org/wiki/C%C3%B2nica). Això és perquè es poden obtenir tallant una superfície cònica doble mitjançant diversos plans.

##La circumferència

La circumferència és el lloc geomètric dels punts del pla que equidisten d'un mateix punt anomenat centre.

<iframe scrolling="no" src="https://www.geogebra.org/material/iframe/id/2575689/width/1938/height/951/border/888888/rc/false/ai/false/sdz/true/smb/false/stb/false/stbh/true/ld/false/sri/true/at/auto" width="800px" height="500px" style="border:0px;"> </iframe>

Considerem ara una circumferència de centre $C(a,b)$ i radi $r$. Anem a veure quina equació han de complir els punts d'aquesta circumferència, $P(x,y)$. Si pensem en el triangle rectangle anterior, el catet de la base mesura necessàriament $x-a$ i el catet de l'altura $y-b$. Si apliquem el teorema de Pitàgores es compleix que:

>$$(x-a)^2+(x-b)^2=r^2$$

Aquesta és l'**equació reduïda de la circumferència de centre $C(a,b)$ i radi $r$**.

Si desenvolupem aquesta equació fent els quadrats obtenim:

$$
\left.\begin{aligned}
x^2+y^2-2ax-2by+a^2+b^2-r^2&=0\\
m \equiv -2a \\
n \equiv -2b \\
p \equiv a^2+b^2-r^2
\end{aligned}
\right\}
\rightarrow x^2+y^2+mx+ny+p=0
$$

Per tant, amb aquesta nova forma de l'equació d'una circumferència, **l'equació general**, els coeficients de $x$ i $y$ ens donen el centre de la circumferència $C(a,b)$ i el terme independent $p$ ens donarà el radi.

**Exemple 1**

Troba el centre i el radi de la circumferència: $x^2+y^2-4x+2y-4=0$.

Els coeficients de $x$ i de $y$ ens donaran el centre de la circumferència:

\begin{align}
-4=-2a \rightarrow a=2\\
2=-2b \rightarrow b=-1
\end{align}

El centre és doncs el punt $C(2,-1)$. Anem a veure quin serà el radi. Això bé donat pel terme independent de l'equació:

$$-4=a^2+b^2-r^2 \rightarrow -4= 4+1-r^2 \rightarrow r=\sqrt{9}=3$$


###Posicions relatives entre recta i circumferència

Donades una recta i una circumferència, ens podem trobar en 3 situacions diferents. El que farem serà resoldre el sistema de dues equacions i dues incògnites format per l'equació de la circumferència per una banda i l'equació de la recta per l'altra. Si considerem que la circumferència té centre $C(a,b)$ i radi $r$ i la recta l'anomenem $s$ tenim que una circumferència i una recta poden ser:

1. **Exteriors**, no es tallen:
    1. el sistema no té solució
    2. $d(C,s)>r$

2. **Tangents**, la recta toca a la circumferència en només un punt:
    1. el sistema té només una solució (parella de valors $(x,y)$
    2. $d(C,s)=r$

3. **Secants**, la recta talla a la circumferència en dos punts:
    1. El sistema té dues solucions o parelles de valors $(x,y)$
    2. $d(C,s)<r$
    3. En aquest cas, diem que la distància entre la circumferència i la recta és $0$ perquè són secants.





<iframe scrolling="no" src="https://www.geogebra.org/material/iframe/id/2577927/width/1938/height/951/border/888888/rc/false/ai/false/sdz/true/smb/false/stb/false/stbh/true/ld/false/sri/true/at/auto" width="800px" height="500px" style="border:0px;"> </iframe>


###Posicions relatives entre circumferències

Considerem dues circumferències amb centres $C$ i $C^\prime$ i radis $r$ i $r^\prime$ respectivament. Les seves equacions formen un sistema de segon grau. Ens podem trobar amb 5 casos diferents:

1. Les circumferències són **exteriors**, no es tallen:
    1. el sistema no té solució
    2. $d(C,C^\prime)>r+r^\prime$

2. Les circumferències són **interiors**:
    1. el sistema no té solució
    2. $d(C,C^\prime)<r-r^\prime$
    3. Un cas particular serien les circumferències concèntriques si $C=C^\prime$

3. Les circumferències són **tangents exteriors**:
    1. El sistema té una solució
    2. $d(C,C^\prime)=r+r^\prime$
4. Les circumferències són **tangents interiors**:
    1. El sistema té una solució
    2. $d(C,C^\prime)=r-r^\prime$
5. Les circumferències són **secants**:
    1. El sistema té dues solucions
    2. $r-r^\prime<d(C,C^\prime)<r+r^\prime$

<iframe scrolling="no" src="https://www.geogebra.org/material/iframe/id/2607485/width/1920/height/941/border/888888/rc/false/ai/false/sdz/true/smb/false/stb/false/stbh/true/ld/false/sri/true/at/auto" width="800px" height="500px" style="border:0px;"> </iframe>

**Exemple 2**

Trobeu la posició relativa entre les circumferències $x^2+y^2=4$ i $(x-3)^2+(y+5)^2=5$.

La primera circumferència té centre el punt $C(0,0)$ i radi "r=2" i la segona té centre el punt $C^\prime(3,-5)$ i radi $r^\prime=\sqrt{5}$. Si solucionem el sistema veurem que és incompatible. Com que no té solució ara només ens cal veure si són exteriors o interiors:



$$
\left.\begin{aligned}
d(C,C^\prime)=|\vec{C C^\prime}|=\sqrt{(3-0)^2+(-5-0)^2}=\sqrt{34}\sim 5.83\\
r+r^\prime=2+\sqrt{5}\sim 4.47
\end{aligned}
\right\}
\rightarrow d(C,C^\prime) > r+r^\prime \rightarrow \text{són exteriors}
$$

<iframe scrolling="no" src="https://www.geogebra.org/material/iframe/id/2607581/width/1920/height/933/border/888888/rc/false/ai/false/sdz/true/smb/false/stb/false/stbh/true/ld/false/sri/true/at/auto" width="800px" height="500px" style="border:0px;"> </iframe>


###Posicions relatives entre un punt i una circumferència

En el cas d'un punt $P(x,y)$ i una circumferència de radi $r$ i centre $C(a,b)$ ens podem trobar 3 casos:

1. El punt és exterior a la circumferència: $d(P,C)>r$
2. El punt pertany a la circumferència: $d(P,C)=r$
3. El punt és interior a la circumferènccia: $d(P,C)<r$

**Exemple 3**

Donat el punt $P(9,-1)$ exterior a la circumferència $x^2+(y+4)^2=9$, trobeu les rectes tangents a la circumferència des d'aquest punt.

Anem a veure si entenem el problema. Sempre que tinguem  un punt exterior a una circumferència es poden traçar dues rectes tangents des del punt fins a la circumferència.


1. Per començar ens cal trobar l'equació del *feix de rectes* que passen pel punt $P(9,-1)$:

    * Sabem que l'equació de la recta té la forma $y=mx+n$. Totes les rectes que passen pel punt $P(9,-1)$ tenen la forma:

    $$-1=9m+n \Rightarrow n=-1-9m \Rightarrow y=mx-1-9m \Rightarrow y=m(x-9)+1 \Rightarrow m(x-9)-y-1=0$$

2. Una manera de solucionar el problema és **exigir que la distància de la recta al centre de la circumferència sigui igual al radi** i d'aquesta manera ens assegurem que recta i circumferència són tangents.

    * Anem a imposar aquesta condició:

      $$d(recta, C)=\frac{|m(0-9)+4-1|}{\sqrt{m^2+(-1)^2}}=3$$


    * Per a solucionar una equació amb valors absolut hem de considerar els 2 casos possibles:

      $$\frac{|3-9m|}{\sqrt{m^2+1}}=3 \begin{cases} \frac{3-9m}{\sqrt{m^2+1}}=3 \\ \frac{3-9m}{\sqrt{m^2+1}}=-3
      \end{cases}$$

    * Agafem i desenvolupem la solució positiva:

      \begin{align}
      \frac{3-9m}{\sqrt{m^2+1}}&=3\\
      (3-9m)^2&=(3\sqrt{m^2+1})^2\\
      81m^2-54m+9&=9m^2+9\\
      72m^2-54m&=0\\
      18m(4m-3)&=0 \begin{cases} m=0 \\ m=\frac{3}{4} \end{cases}
      \end{align}

    * Fixeu-vos que si agafem l'opció negativa obtenim les mateixes solucions, ja que a l'elevar al quadrat el signe negatiu esdevé positiu.




2. Una altra manera de resoldre el problema és, fer que **el sistema format per les equacions de la recta tangent i la circumferència tingui solució única**, perquè si tingués solució doble voldria dir que la recta és secant i no tangent a la circumferència.

    * Solucionem el sistema per substitució:

    $$
    \left.\begin{aligned}
    y=m(x-9)-1\\
    x^2+(y+4)^2=9
    \end{aligned}
    \right\}
    \Rightarrow x^2+\Big( m(x-9)-1+4 \Big)^2=9 \Rightarrow ... \Rightarrow (1+m^2)x^2+2m(3-9m)x+(3-9m)^2-9=0
    $$

    * Ara ens cal exigir que només hi hagi una parella de valors $(x,y)$ que siguin solució. Per fer-ho, igualarem el discriminant de l'equació de segon grau ($b^2-4ac$) a zero:

    \begin{align}
    \Big(2m(3-9m)\Big)^2-4(1+m^2)\Big((3-9m)^2-9\Big)&=0\\
    4m^2(3-9m)^2-(4+4m^2)(9+81m^2-54m-9)&=0\\
    4m^2(9+81m^2-54m)-324 m^2+216m-324 m^4+216 m^3&=0\\
    36m^2+324m^4-216m^3-324 m^2+216m-324 m^4+216m^3&=0\\
    216m-288m^2&=0\\
    -72m(4m-3)&=0\\
    m(4m-3)&=0 \begin{cases} m=0 \\ m=\frac{3}{4} \end{cases}
    \end{align}

    * Evidentment obtenim la mateixa solució.

3. Tant si triem l'opció 1 o la 2, ens caldrà finalment trobar l'equacions de les rectes tangents:

$$
y=m(x-9)-1 \begin{cases} m=0 \Rightarrow n=-1 \Rightarrow y= -1 \\ m=\frac{3}{4} \Rightarrow n=-\frac{31}{4} \Rightarrow y= \frac{3}{4}x-\frac{31}{4} \end{cases}
$$

<iframe scrolling="no" src="https://www.geogebra.org/material/iframe/id/2625505/width/1920/height/933/border/888888/rc/false/ai/false/sdz/true/smb/false/stb/false/stbh/true/ld/false/sri/true/at/auto" width="800px" height="500px" style="border:0px;"> </iframe>

####Potència d'un punt respecte d'una circumferència

Considerem un punt exterior a una circumferència i tracem dues secants d'aquest punt a la circumferència tal i com mostra el dibuix.

<iframe scrolling="no" src="https://www.geogebra.org/material/iframe/id/2639115/width/1920/height/934/border/888888/rc/false/ai/false/sdz/true/smb/false/stb/false/stbh/true/ld/false/sri/true/at/auto" width="800px" height="500px" style="border:0px;"> </iframe>

Considerem els triangles $PAB^\prime$ i $PA^\prime B$. Els angles inscrits a la circumferència $B^\prime$ i $A^\prime$ són iguals, $B^\prime=A^\prime$ ja que abarquen el mateix arc de circumferència $\widehat{BA}$. Com que els dos triangles comparteixen un angle $P$, i tenen 2 angles iguals, el tercer ha de ser necessàriament igual (la suma d'angles d'un triangle és sempre $180^o$): $B=A$.

Per tant, si dos triangles tenen els seus 3 angles iguals 2 a 2 vol dir que són [triangles semblants](http://recursostic.educacion.es/secundaria/edad/4esomatematicasB_cat/semejanza/quincena6_contenidos_1c.htm) i en conseqüència els seus costats seran proporcionals:

$$\frac{PA}{PB}=\frac{PB^\prime}{PA^\prime}\Rightarrow PA\cdot PA^\prime=PB\cdot PB^\prime$$

Aquest producte de distàncies es defineix com a la **potència d'un punt respecte una circumferència**:

$$p=PA\cdot PA^\prime$$

Considerem ara una recta secant des d'un punt exterior $P(x_0,y_0)$ que passi pel centre d'una circumferència de centre $C(a,b)$ i radi $r$. Definim $d$ com la distància del punt $P$ al centre $C$.

<iframe scrolling="no" src="https://www.geogebra.org/material/iframe/id/2642273/width/1920/height/933/border/888888/rc/false/ai/false/sdz/true/smb/false/stb/false/stbh/true/ld/false/sri/true/at/auto" width="800px" height="500px" style="border:0px;"> </iframe>

La potència del punt $P$ respecte la circumferència és:

$$
\left.\begin{aligned}
p&=PA\cdot PA^\prime=(d-r)(d+r)=d^2-r^2\\
d&=|\vec{CP}|=\sqrt{(x_0-a)^2+(y_0-b)^2}
\end{aligned}
\right\}
\Rightarrow p=d^2-r^2=(x_0-a)^2+(y_0-b)^2-r^2
$$

Per tant, la potència d'un punt respecte una circumferència ens dóna idea de la situació del punt respecte la circumferència:

$$  p=d^2-r^2=(x_0-a)^2+(y_0-b)^2-r^2 \begin{cases} d>r\rightarrow p>0 \Rightarrow \text{p és exterior} \\
d<r\rightarrow p<0 \Rightarrow \text{p és interior} \\ d=r\rightarrow p=0 \Rightarrow \text{p pertany a la circumferència}
\end{cases}$$


##La paràbola

A 4t d'eso havíeu treballat les paràboles com la representació gràfica [d'una funció polinòmica de segon grau](http://proyectodescartes.org/EDAD/materiales_didacticos/EDAD_4eso_B_funciones2-JS/index.htm) del tipus $y=f(x)=ax^2+bx+c$. Vèiem que la paràbola és una funció amb simetria parell i que té un vèrtex amb abcissa $(x=-\frac{b}{2a})$.

La paràbola també es pot entendre però com el **lloc geomètric** dels punts del pla que equidisten d'un punt $F$ anomenat **focus** i d'una recta $r$ anomenada **directriu**.

<iframe scrolling="no" src="https://www.geogebra.org/material/iframe/id/2657653/width/986/height/933/border/888888/rc/false/ai/false/sdz/true/smb/false/stb/false/stbh/true/ld/false/sri/true/at/auto" width="800px" height="500px" style="border:0px;"> </iframe>

Si mirem al dibuix hi podem veure els elements següents:

1. **Eix de la paràbola**: és la recta perpendicular a la directriu que passa pel focus. En el cas específic del dibuix és l'eix $x$.
2. **Vèrtex de la paràbola**: és el punt d'intersecció de la paràbola amb el seu eix. En aquest cas és el punt $(0,0)$.
3. **Paràmetre**: és la distància del focus $F$ a la directriu $r$. L'anomenem **$p$**.

###Equació reduïda de la paràbola

Fixem-nos ara en una paràbola com la del dibuix que té el seu eix situat sobre l'eix de les abscisses i el vèrtex a l'origen de coordenades. Com que els punts de la paràbola, i el vèrtex en particular, compleixen la propietat que equidisten del focus i de la directriu, podem afirmar que les coordenades del focus són $F(\frac{p}{2},0)$ i l'equació de la recta directriu és $r:x=-\frac{p}{2}$.

Si $P(x,y)$ és un punt qualsevol de la paràbola es compleix que: $d(P,r)=d(P,F)$:


$$
\left.\begin{aligned}
d(P,r)&=\frac{|x+\frac{p}{2}|}{\sqrt{0^2+1}}\\
d(P,F)&=|\vec{FP}|=\sqrt{(x-\frac{p}{2})^2+y^2}
\end{aligned}
\right\}
\Rightarrow |x+\frac{p}{2}|=\sqrt{(x-\frac{p}{2})^2+y^2} \Rightarrow x^2+px+\frac{p^2}{4}=x^2-px+\frac{p^2}{4}+y^2
$$

Si simplifiquem tenim **l'equació reduïda de la paràbola**:

>$$y^2=2px$$

En cas que l'eix estigui situat sobre **l'eix d'ordenades**, el focus seria **$F(0,\frac{p}{s})$** i l'equació de la recta directriu seria **$r:y=-\frac{p}{2}$**. L'equació reduïda de la paràbola seria llavors:

>$$x^2=2py$$

###Equació de la paràbola d'eix paral.lel a l'eix d'abscisses o d'ordenades

<iframe scrolling="no" src="https://www.geogebra.org/material/iframe/id/2657815/width/1600/height/951/border/888888/rc/false/ai/false/sdz/true/smb/false/stb/false/stbh/true/ld/false/sri/true/at/auto" width="800px" height="500px" style="border:0px;"> </iframe>

Considerem ara que l'eix de la paràbola és paral.lel a l'eix d'abscisses. El vèrtex ha passat de ser el punt $(0,0)$ al punt $(x_0,y_0)$. Si comparem la nova paràbola amb l'anterior, amb eix l'eix de les abscisses i vèrtex el punt $(0,0)$ veiem que els punts $P(x,y)$ de la nova paràbola seran els de la paràbola anterior $P^\prime(x^\prime, y^\prime)$ però amb una translació $x_0$ en $x$ i $y_0$ en $y$:

$$
\left.\begin{aligned}
x&=x^\prime+x_0\\
y&=y^\prime+y_0\\
\end{aligned}
\right\}
$$

Per tant, si l'equació de la paràbola "vella" era $y^{\prime 2}=2px^\prime$ si fem el canvi anterior obtenim:

>$$(y-y_0)^2=2p(x-x_0)$$

que és l'**equació d'una paràbola amb l'eix paral.lel a l'eix d'abscisses i amb vèrtex el punt $(x_0,y_0)$**. Si intercanviem $x$ i $y$ obtenim l'equació d'una paràbola amb eix paral.lel a l'eix d'ordenades:

>$$(x-x_0)=2p(y-y_0)$$

Si desenvolupem les dues expressions anteriors obtenim **l'equació general de la paràbola**:

\begin{align}
(y-y_0)^2&=2p(x-x_0)\\
y^2+y_0^2-2yy_0&=2px-2px_0\\
-2px&=-y^2+2y_0y-y_0^2-2px_0\\
2px&=y^2-2y_0y+y_0^2+2px_0\\
x&=\frac{1}{2p}y^2-\frac{y_0}{p}y+\big( \frac{y_0^2}{2p}+x_0 \big)
\end{align}

>$$x&=ay^2+by+c$$

que és l'equació general d'una paràbola amb l'eix paral.lel a l'eix d'abscisses i on

\begin{align}
a&=\frac{1}{2p}\\
b&=-\frac{y_0}{p}\\
c&=\frac{y_0^2}{2p}+x_0
\end{align}

El mateix podem fer amb una paràbola amb eix paral.lel a l'eix d'ordenades:

>$$y=ax^2+bx+c$$


##L'el.lipse

##L'hipèrbola
