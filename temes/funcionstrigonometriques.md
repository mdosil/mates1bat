#Tema 12: Funcions trigonomètriques


##La funció sinus

###Definició

La funció sinus és aquella funció que a cada nombre real se li associa el valor del sinus de l'angle en **radiants**:

\begin{align}
sin:& \mathbb{R} \rightarrow \mathbb{R} \\
&x \rightarrow y=sin (x)\\
&0 \rightarrow sin(0)=0\\
&\frac{\pi}{2} \rightarrow sin(\frac{\pi}{2})=1\\
&\pi \rightarrow sin(\pi)=0\\
&\frac{3\pi}{2} \rightarrow sin(\frac{3\pi}{2})=-1\\
&.\\
&.\\
&.\\
\end{align}

A partir d'aquí ja podem deduir que el domini són tots els nombres reals i el recorregut és l'interval de $-1$ a $1$ ja que el sinus d'un angle està entre aquests dos valors:

\begin{align}
D_f&=\mathbb{R}\\
R_f&=[-1,1]
\end{align}

###Representació gràfica

<iframe scrolling="no" src="https://www.geogebra.org/material/iframe/id/asB5hGdD/width/830/height/700/border/888888/rc/false/ai/false/sdz/true/smb/false/stb/false/stbh/true/ld/false/sri/true/at/auto" width="830px" height="700px" style="border:0px;"> </iframe>


Veiem que la representació gràfica dóna lloc a una funció que s'anomena **corba sinusoide**. És una funció **periòdica** on $T=2\pi$. Si recordem el que vam aprendre en el [Tema 2](http://mdosil.cat/mates1batcientific/temes/trigonometria/) podrem entendre moltes coses que passen en aquesta representació:

* $sin (2\pi)=sin(\pi)=0$
* $sin (\frac{\pi}{2})=1$
* Els angles del 1r i del 2n quadrants tenen $sin>0$.
* Els angles del 2n i del 4t quadrants tenen $sin<0$.

###Propietats

1. El domini de la funció sinus són tots els nombres reals: $D_{sin(x)}=\mathbb{R}$
2. El recorregut està entre $1$ i $-1$ ja que no hi pot haver cap angle que tingui sinus inferior o superior a aquests valors:  $R_{sin(x)}=[-1,1]$
3. És una funció periòdica amb període $T=2\pi$: $sin(x)=sin(x+2k\pi) \mbox{ on } k \in \mathbb{Z}$
4. És contínua en $\mathbb{R}$
5. És creixent en els intervals $(-\frac{\pi}{2}+2k\pi,\frac{\pi}{2}+2k\pi)$, $k \in \mathbb{Z}$
6. És decreixent en els intervals $(\frac{\pi}{2}+2k\pi,\frac{3\pi}{2}+2k\pi)$, $k \in \mathbb{Z}$
7. El sinus d'angles suplementaris és el mateix: $sin(x)=sin(\pi-x)$
8. El sinus dels angles $x$ i $x+\pi$ té signe contrari: $sin(x)=-sin(\pi+x)$
9. El sinus d'angles oposats són oposats: $sin(x)=-sin(-x)$

**Exemple 1**

Representa en els mateixos eixos de coordenades les funcions $f(x)=sinx$, $g(x)=sin(3x)$, $h(x)=sin(x+\pi)$ i $j(x)=2sin(x)$. Estudia després els aspectes següents:

* La relació entre $f(x)$ i $g(x)$
* La relació entre $f(x)$ i $h(x)$
* La relació entre $j(x)$ i $f(x)$.

Si comparem $f(x)$ i $g(x)$ veiem que el nombre que multiplica la incògnita determina el període: el període s'escurça en aquest factor, o sigui, la segona funció varia 3 vegades més ràpid: en el primer cas, $T=2\pi$ i en el segon $T=\frac{2\pi}{3}$. **L'amplitud** (la distància entre els màxims i els mínims de la funció) és en ambdós casos la mateixa, o sigui, $2$, ja que el recorregut en les dues funcions és el mateix, $R_f=R_g=[-1,1]$.

<iframe scrolling="no" src="https://www.geogebra.org/material/iframe/id/FxVP85SK/width/700/height/291/border/888888/rc/false/ai/false/sdz/true/smb/false/stb/false/stbh/true/ld/false/sri/true/at/auto" width="700px" height="291px" style="border:0px;"> </iframe>

En el segon cas, veiem que ambdues funcions són *oposades*, quan $f$ aconsegueix el màxim, $h$ està en el seu mínim. Això és perquè els signes del sinus de dos angles separats $\pi$ unitats són **iguals però de signe contrari**. Aquí podem fer una observació més, el fet d'afegir un sumand a la variable $x$ vol dir que:

* En el cas de tenir $sin(x+k)$, $k \in \mathbb{R}^+$, la funció $sin(x)$ es desplaçaria $k$ unitats cap a **l'esquerra**
* En el cas de tenir $sin(x-k)$, $k \in \mathbb{R}^+$, la funció $sin(x)$ es desplaçaria $k$ unitats cap a **la dreta**

En qualsevol cas les funcions mantenen l'amplitud (el recorregut és el mateix) i el període.

<iframe scrolling="no" src="https://www.geogebra.org/material/iframe/id/JcvDYwWc/width/700/height/291/border/888888/rc/false/ai/false/sdz/true/smb/false/stb/false/stbh/true/ld/false/sri/true/at/auto" width="700px" height="291px" style="border:0px;"> </iframe>

En el tercer cas, el fet de multiplicar la funció $sin(x)$ per $2$ provoca un augment en l'amplitud de la funció: $R_f=[-1,1]$ i $R_j=[-2,2]$. Tot i això, es **conserven el període i la posició dels màxims i els mínims**.

<iframe scrolling="no" src="https://www.geogebra.org/material/iframe/id/ZeYnwwvy/width/700/height/300/border/888888/rc/false/ai/false/sdz/true/smb/false/stb/false/stbh/true/ld/false/sri/true/at/auto" width="700px" height="300px" style="border:0px;"> </iframe>



##La funció cosinus

###Definició

###Representació gràfica

###Propietats

##La funció tangent

###Definició

###Representació gràfica

###Propietats

##La funció arc sinus

##La funció arc cosinus

##La funció arc tangent
