#Tema 13: Derivades

##Derivada d'una funció en un punt



### Definició de derivada d'una funció en un punt

Donada una funció real $f$ i un punt d'abcissa $x=a$, $a \in \mathbb{R}$, on $a \in D_f$, considerem el límit següent:

$$\lim_{h\to 0} \frac{f(a+h)-f(a)}{h}$$

si aquest límit existeix s'anomena **derivada de la funció $f$ en $x=a$, $f^{\prime} (a)$**:

$$f^{\prime}(a)=\lim_{h\to 0} \frac{f(a+h)-f(a)}{h}$$

Aquesta expressió es pot escriure d'una altra manera si adoptem el canvi de variable següent:

\begin{align}
a+h&=x \rightarrow \begin{cases} h=x-a \\
     \mbox{si } h \rightarrow 0 \Rightarrow x \rightarrow a
    \end{cases}\\
f^{\prime}(a)&=\lim_{x\to a} \frac{f(x)-f(a)}{x-a}
\end{align}

**Exemple 1**

Donada $f(x)=7x-3$ calculeu $f^{\prime}(a) \forall a \in \mathbb{R}$.

$$f^{\prime}(a)=\lim_{x\to a} \frac{f(x)-f(a)}{x-a}=\lim_{x\to a} \frac{7x-3-(7a-3)}{x-a}=\lim_{x\to a} \frac{7(x-a)}{x-a}=7$$

**Exemple 2**

Esbrineu si existeix la derivada en els punts $x=0$, $x=2$ i $x=-2$ de la funció a trossos:

$$f(x)= \begin{cases} 2x+1 \mbox{ si } x \le 0 \\
     x-1 \mbox{ si } x > 0
    \end{cases}$$

Per calcular la derivada en aquests punts, el que haurem de fer és calcular els límits anteriors per $x\to 0$, $x\to 2$ i $x \to -2$.

$$f^{\prime}(0)=\lim_{x\to 0} \frac{f(x)-f(0)}{x-0}=?\Rightarrow\begin{cases} \lim_{x\to 0^{+}} \frac{f(x)-f(0)}{x-0}= \lim_{x\to 0^{+}} \frac{x-1-1}{x}=\lim_{x\to 0^{+}} \frac{x-2}{x}=\frac{-2}{0}=-\infty\\
     \lim_{x\to 0^{-}} \frac{f(x)-f(0)}{x-0}=\lim_{x\to 0^{-}} \frac{2x}{x}=2
    \end{cases}$$

Veiem que els límits laterals no coincideixen. Per tant, el límit no es pot calcular, o sigui que **$f^{\prime}(0)=\nexists$**

$$f^{\prime}(2)=\lim_{x\to 2} \frac{f(x)-f(2)}{x-2}=\lim_{x\to 2} \frac{x-1-1}{x-2}=\lim_{x\to 2} \frac{x-2}{x-2}=1$$

$$f^{\prime}(-2)=\lim_{x\to -2} \frac{f(x)-f(-2)}{x+2}=\lim_{x\to -2} \frac{2x+4}{x+2}=\lim_{x\to -2} \frac{2(x+2)}{x+2}=2$$





###Interpretació geomètrica de la derivada

Anem a veure si amb un dibuix entenem què és això de la derivada. Fixeu-vos amb el gràfic següent:

<iframe scrolling="no" src="https://www.geogebra.org/material/iframe/id/bd7R3xbq/width/814/height/700/border/888888/rc/false/ai/false/sdz/true/smb/false/stb/false/stbh/true/ld/false/sri/true/at/auto" width="814px" height="700px" style="border:0px;"> </iframe>

Fixem-nos amb el gràfic de la funció f. Considerem dos punts, un punt $A$ de coordenades $(a, f(a))$ i un altre punt $B$ de coordenades $(x, f(x))$. Amb el punt lliscant podeu anar movent el punt $B$. Tracem una secant des del punt $A$ al punt $B$. Considerem el triangle dibuixat a la figura. El catet inferior té longitud $\Delta x=x-a$ i el catet superior $\Delta y=f(x)-f(a)$. El **pendent de la recta secant** és el quocient entre aquests dos valors i també coincideix amb **la tangent de l'angle $\alpha$**:

$$m=tan \alpha= \frac{\Delta y}{\Delta x}=\frac{f(x)-f(a)}{x-a}$$

Si ens fixem aquesta fórmula és molt semblant a la de la definició de la derivada d'una funció en el punt $a$, $f^{\prime}(a)$. La diferència està en el **límit**.

Si ara anem acostant cada vegada més el punt $B$ al punt $A$, veiem que aquesta recta secant, en **el límit** que $A=B$ es converteix en una **recta tangent en $x=a$**, i per tant:

>La derivada en $x=a$ de $f(x)$, $f^\prime(a)$, és **el pendent de la recta tangent a la gràfica de la funció en el punt $x=a$**  i es calcula a partir del límit: $f^{\prime}(a)=\lim_{x\to a} \frac{f(x)-f(a)}{x-a}$  

###Definició de recta tangent a una corba en un punt

Vist això, anomenem recta tangent a una corba en el punt $x=a$, a aquella recta que compleix:

1. Conté el punt $(a,f(a))$
2. Té per pendent $m=f^{\prime}(a)$

D'aquí podem expressar l'equació de la recta tangent a una funció en el punt $x=a$ de la manera:

$$y-f(a)=f^{\prime}(a)(x-a)$$

**Exemple 3**

Trobeu l'equació de la recta tangent a la funció $f(x)=3x^2-5x+2$ en el punt d'abcissa $x=1$.

El punt $A$ en aquest cas és el punt $(1,f(1))=(1,0)$

Anem a calcular la derivada de la funció $f$ en $x=1$:



$$m=f^{\prime}(1)=\lim_{x\to 1} \frac{f(x)-f(1)}{x-1}=\frac{3x^2-5x+2-0}{x-1}=1$$

Per tant, l'equació de la recta tangent a $f(x)$ en $x=1$ és:

$$y-0=1(x-1)\Rightarrow y=x-1$$


###Relació entre la derivada i la continuïtat d'una funció en un punt

##La funció derivada

###Definició de funció derivada

###Derivació o càlcul de Derivades

####Regla 1

####Regla 2
