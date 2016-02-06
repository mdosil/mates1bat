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

###Potència d'un punt respecte d'una circumferència


##L'el.lipse

##La paràbola

##L'hipèrbola
