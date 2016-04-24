#Tema 10: Límits i continuïtat de funcions

En aquest tema estudiarem en detall la continuïtat d'una funció i també què passa en els punts que aquesta és discontínua. Ho farem utilitzant el concepte de límit que ja vam començar a treballar amb les [successions](http://mdosil.cat/mates1batcientific/temes/successions/). D'altra banda, ens fixarem també què passa quan la variable es fa molt petita ($x\rightarrow -\infty$) i quan aquesta es fa molt gran ($x\rightarrow +\infty$).

##Concepte de límit d'una funció en un punt

En el tema de successions, teníem que sempre calculàvem el límit d'una successió $a_n$ quan $n\rightarrow +\infty$. I ens trobàvem amb 3 casos:

$$
lim \quad a_n=L \begin{cases} +\infty \\
-\infty \\
\mbox{ nombre real }\end{cases}
$$

En aquest tema traslladarem el concepte de límit a les funcions. Si tenim una funció $f(x)$ podem plantejar-nos 3 coses:

1. Què passa quan $x\rightarrow -\infty$
2. Què passa quan $x\rightarrow +\infty$
3. Què passa quan $x\rightarrow a$ on $a \in \mathbb{R}$

Ens fixarem aquí en el primer cas i més endavant ja pensarem què passa amb una funció en els límits infinits.

###Interpretació gràfica

A través d'un exemple molt senzill veurem què vol dir gràficament el límit d'una funció en un punt.

**Exemple 1**

Considerem la funció $y=f(x)=2x+1$. El domini d'aquesta funció són tots els nombres reals. Volem calcular quin és el límit d'aquesta funció quan $x$ s'acosta a $2$. Com que el domini d'aquesta funció són tots els nombres reals, el $2$ tindrà imatge, de fet, $f(2)=2\cdot 2+1=5$. Considerem ara un petit entorn de $2$ que l'anomenem $A$ i mirarem que passa amb les imatges d'aquest entorn. A sota podeu veure'n una representació gràfica.


<iframe scrolling="no" src="https://www.geogebra.org/material/iframe/id/tM7D6quP/width/600/height/629/border/888888/rc/false/ai/false/sdz/true/smb/false/stb/false/stbh/true/ld/false/sri/true/at/auto" width="600px" height="629px" style="border:0px;"> </iframe>

Veiem que si les $x$ estan en un entorn $A$ amb punt central $x=2$ les imatges d'aquest entorn estan en un entorn de centre $y=5$ i radi $r$, això és, en un interval $(5-r,5+r)$. Si fem aquest entorn de $x=2$ cada vegada més petit, podem veure que les imatges cada vegada s'acosten més a $5$. D'aquesta manera podem afirmar que:


$$\lim_{x\to 2} f(x)=\lim_{x\to 2} (2x+1)=5$$

Això, expressat en un altre llenguatge, és:

$$\lim_{x\to 2} f(x)=5 \Leftrightarrow \exists \text{  un entorn  } A | \text{ si } x \in A \text{ , } x \neq 2 \Rightarrow f(x) \in (5-r, 5+r)$$

###Definició de límit d'una funció en un punt

Anem a definir més rigorosament el límit d'una funció en un punt:

>$$\lim_{x\to a} f(x)=L \Leftrightarrow \forall \text{   entorn } (L-r, L+r) \text{ en l'eix y  } \exists \text{  un entorn } A \text{ d' }a \text{ en l'eix } x | \text{ si } x \in A \text{ , } x \neq a \Rightarrow f(x) \in (L-r, L+r)$$


###Límits laterals

Quan parlem del límit d'una funció en un punt, també podem considerar-ne els límits laterals, què passa amb la funció quan ens acostem al punt per l'esquerra i què passa amb la funció quan ens acostem al punt per la dreta.

PEr estudiar això fixem-nos amb la funció part entera: $y=f(x)=E(x)$, que representem a continuació.

<iframe scrolling="no" src="https://www.geogebra.org/material/iframe/id/nEMUtsN9/width/520/height/751/border/888888/rc/false/ai/false/sdz/true/smb/false/stb/false/stbh/true/ld/false/sri/true/at/auto" width="520px" height="751px" style="border:0px;"> </iframe>

Si estudiem què passa quan ens acostem a $x=1$ per l'esquerra (valors més petits que $1$) i per la dreta (valors més grans que $1$) veiem que obtenim dos resultats diferents:

\begin{align}
\lim_{x\to 1^+}&=1 \\
\lim_{x\to 1^-}&=0
\end{align}

Quan els límits laterals **no coincideixen**, diem que $\lim_{x\to 1} E(x)=  \nexists$. Per tant:

>$$\text{Si } \lim_{x\to a-} f(x)=\lim_{x\to a-} f(x)=L \Rightarrow \lim_{x\to a} f(x)=L$$

en cas contrari (els límits laterals no coincideixen) el límit **no existeix**.

###Límits d'una funció a l'infinit



##Continuïtat d'una funció en un punt

##Discontinuïtats
