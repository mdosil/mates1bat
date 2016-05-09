#Tema 11: Funció exponencial i logarítmica

En aquest tema estudiarem les característiques bàsiques de les funcions exponencials i logarítmiques, la seva representació gràfica i algunes de les seves particularitats.

##La funció exponencial

Les funcions exponencials són totes aquelles expressades per potències on l'incògnita és un nombre real i la base un nombre real positiu.

###Definició

Donat un nombre $a$ positiu ($a>0$) anomenem funció exponencial de base $a$ i la representem per $E_a$ a l'aplicació següent:

\begin{align}
E_a:& \mathbb{R} \rightarrow \mathbb{R}^+ \\
&x \rightarrow y=a^x\\
&2 \rightarrow a^2\\
&3 \rightarrow a^3\\
-&1 \rightarrow a^{-1}=\frac{1}{a}\\
&0 \rightarrow a^0=1\\
&\sqrt{5} \rightarrow a^{\sqrt{5}}\\
&.\\
&.\\
&.\\
\end{align}

###Representació gràfica

D'entrada podem distingir 2 casos, el cas en que $a>1$ i el cas en que $0<a<1$. Observa amb atenció el gràfic de sota. Varia el valor de $a$ i estudia què passa amb cadascun dels casos.

<iframe scrolling="no" src="https://www.geogebra.org/material/iframe/id/GY44rnNn/width/600/height/787/border/888888/rc/false/ai/false/sdz/true/smb/false/stb/false/stbh/true/ld/false/sri/true/at/auto" width="600px" height="787px" style="border:0px;"> </iframe>


**Exemple 1**

Representa gràficament la funció $f(x)=2^x$ i la funció $g(x)=(\frac{1}{2})^x$ sobre els mateixos eixos de coordenades. Explica què passa.

<iframe scrolling="no" src="https://www.geogebra.org/material/iframe/id/wzbXYbuv/width/600/height/787/border/888888/rc/false/ai/false/sdz/true/smb/false/stb/false/stbh/true/ld/false/sri/true/at/auto" width="600px" height="787px" style="border:0px;"> </iframe>

Veiem que **Les dues funcions són simètriques respecte els eixos de coordenades**. Ambdues passen pel punt $(0,1)$, ja que qualsevol nombre elevat a zero és $1$. $f(x)=2^x$ és sempre creixent i té una **assímptota horitzontal** cap a $-\infty$ en $y=0$ i $g(x)=(\frac{1}{2})^x$ és sempre decreixent i té una **assímptota horitzontal** cap a $+\infty$ en $y=0$.

###Propietats

####Propietats generals
1. És contínua en $\mathbb{R}$
2. El domini són tots els reals i el recorregut són tots els nombres reals positius: $D_f=\mathbb{R}, R_f=\mathbb{R}^+$
3. $a^x>0$
4. $a^x \cdot a^y=a^{x+y}$
5. $\frac{a^x}{a^y}=a^{x-y}$
6. $(a^x)^y=a^{x\cdot y}$
7. $(a\cdot b)^x=a^x\cdot b^x$
8. $\big(\frac{a}{b} \big)^x=\frac{a^x}{b^x}$
9. $a^0=1$
10. $a^{-x}=\frac{1}{a^x}$
11. $a^{\frac{m}{n}}=\sqrt[n]{a^m}$


####Propietats particulars

1. Si $a>1$ la funció és **creixent** en $\mathbb{R}$
2. Si $0<a<1$ la funció és **decreixent** en $\mathbb{R}$
3. $$\mbox{Si } a>1 \rightarrow \begin{cases} \lim_{x\to + \infty} a^x=+\infty \\
     \lim_{x\to - \infty} a^x=0
    \end{cases}
    $$
4. $$\mbox{Si } 0<a<1 \rightarrow \begin{cases} \lim_{x\to + \infty} a^x=0 \\
   \lim_{x\to - \infty} a^x=+\infty
  \end{cases}
  $$
5. La funció exponencial té en l'eix de les $x$ una assímptota horitzontal
##La funció logarítmica

###Definició

###Representació gràfica

###Propietats
