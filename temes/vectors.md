#Tema 5: Vectors en el pla

##Conceptes

###Definició

Un vector és un segment en el pla que determina una *direcció*, una *mòdul* o *magnitud* i un *sentit*. La direcció ve determinada per la recta sobre la qual es troba el vector, la magnitud és la llargada d'aquest vector i el sentit és, per entendre'ns, la punta de la fletxa del vector.

<iframe scrolling="no" src="https://www.geogebra.org/material/iframe/id/2240083/width/1600/height/933/border/888888/rc/false/ai/false/sdz/true/smb/false/stb/false/stbh/true/ld/false/sri/true/at/auto" width="600px" height="350px" style="border:0px;"> </iframe>

###Components cartesianes d'un vector

Donats dos punts $A=(a_1,a_2)$ i $B=(b_1,b_2)$ en el pla definim el vector $\vec{AB}$ com el segment que té origen en $A$ i final en $B$, tal i com hem vist a la figura anterior. Les coordenades del vector les calculem de la manera següent:

>$$\vec{AB}=(b_1-a_1,b_2-a_2)$$

El mòdul o llargada del vector,$|\vec{AB}|$,   el calculem aplicant el teorema de Pitàgores al triangle rectangle que defineix:


>$$|\vec{AB}|=\sqrt{(b_1-a_1)^2+(b_2-a_2)^2}$$

<iframe scrolling="no" src="https://www.geogebra.org/material/iframe/id/2240083/width/1600/height/933/border/888888/rc/false/ai/false/sdz/true/smb/false/stb/false/stbh/true/ld/false/sri/true/at/auto" width="600px" height="350px" style="border:0px;"> </iframe>

###Vectors equipol.lents

Dos vectors són equipol.lents si tenen la mateixa direcció, mòdul i sentit. En definitiva, si tenen les mateixes coordenades. A la pràctica, els vectors equipol.lents són paral.lels en el pla i podem passar de l'un a l'altre amb un senzill moviment de translació.

**Exemple 1**

Considera els punts en el pla $A(2,4)$, $B(13,7)$, $C(1,2)$ i $D(12,5)$. Dibuixa els vectors $\vec{AB}$ i $\vec{CD}$ i demostra que són equipol.lents.

Anem a calcular les components d'aquests vectors abans de dibuixar-los:

\begin{align}
    \vec{AB} &=(13-2,7-4)=(11,3)\\
    \vec{CD} &=(12-1,5-2)=(11,3)
\end{align}

Veiem que tenen les mateixes components.

<iframe scrolling="no" src="https://www.geogebra.org/material/iframe/id/2240299/width/1920/height/933/border/888888/rc/false/ai/false/sdz/true/smb/false/stb/false/stbh/true/ld/false/sri/true/at/auto" width="600px" height="350px" style="border:0px;"> </iframe>

>Cada conjunt de vectors equipol.lents representen un sol vector anomenat **vector lliure**.

Els vectors lliures normalment es representen amb origen el punt $O(0,0)$ i extrem les coordenades del vector.


<iframe scrolling="no" src="https://www.geogebra.org/material/iframe/id/2240397/width/1920/height/933/border/888888/rc/false/ai/false/sdz/true/smb/false/stb/false/stbh/true/ld/false/sri/true/at/auto" width="600px" height="350px" style="border:0px;"> </iframe>

<!---------------------------------------------------------->
##Operacions amb vectors

###Suma

Siguin $\vec{u}=(u_1,u_2)$ i $\vec{v}=(v_1,v_2)$, per sumar algebraicament dos vectors només cal que sumem les components dos a dos:

>$$\vec{u}+\vec{v}=(u_1+v_1,u_2+v_2)$$



 Si els sumem gràficament en el pla, aplicarem *la regla de paral.lelogram* per trobar gràficament el vector suma: es tracta de posar els dos vectors amb el mateix origen (típicament el punt $(0,0)$) i traçar rectes paral.leles als vectors. La diagonal del paral.lelogram que es forma és el vector suma.

<<iframe scrolling="no" src="https://www.geogebra.org/material/iframe/id/2233817/width/1600/height/951/border/888888/rc/false/ai/false/sdz/true/smb/false/stb/false/stbh/true/ld/false/sri/true/at/auto" width="600px" height="350px" style="border:0px;"> </iframe>

La suma de vectors té les propietats següents:

1. Associativa: $\vec{u}+\vec{v}+\vec{w}=(\vec{u}+\vec{v})+\vec{w}=\vec{u}+()\vec{v}+\vec{w})$
2. Commutativa: $\vec{u}+\vec{v}=\vec{v}+\vec{u}$
3. Element neutre: $\vec{u}+\vec{0}=\vec{u}$ on $\vec{0}=(0,0)$
4. Element oposat: $\vec{u}+(-\vec{u})=\vec{0}$

###Resta

Donats $\vec{u}=(u_1,u_2)$ i $\vec{v}=(v_1,v_2)$, per restar-los algebraicament només cal que restem les components dos a dos:

>$$\vec{u}-\vec{v}=(u_1-v_1,u_2-v_2)$$

Gràficament, el vector resta consisteix en el vector que s'obté unint l'extrem del primer vector amb el del segon vector.

<iframe scrolling="no" src="https://www.geogebra.org/material/iframe/id/2240625/width/1600/height/933/border/888888/rc/false/ai/false/sdz/true/smb/false/stb/false/stbh/true/ld/false/sri/true/at/auto" width="600px" height="350px" style="border:0px;"> </iframe>


###Producte d'un nombre real per un vector

Per multiplicar un nombre real $k$ per un vector només cal multiplicar les components per aquest nombre real:

>$$k\cdot \vec{u}=(k \cdot u_1,k \cdot u_2)$$

###Producte escalar

El producte escalar entre dos vectors és un **nombre real** i es defineix com:
      >$$\vec{u}\cdot \vec{v}=|\vec{u}|\cdot|\vec{v}|\cdot cos \alpha$$

on $|\vec{u}|$ i $|\vec{v}|$ són els mòduls dels vectors i $\alpha$ l'angle que formen entre ells.

Més endavant demostrarem que el producte escalar de dos vectors també es pot expressar com:

>$$\vec{u}\cdot \vec{v}=u_1\cdot v_1+u_2\cdot v_2$$

Ja veiem que si dos vectors són perpendiculars (o **ortogonals**) ($\alpha=90^0$) el seu producte escalar serà $0$ i si són paral.lels ($\alpha=0^0$) el seu producte escalar serà màxim i serà igual al producte dels seus mòduls.

El producte escalar té les propietats següents:

1. Commutativa: $\vec{u} \cdot \vec{v}= \vec{v} \cdot \vec{u}$
2. Associativa: $\lambda \cdot (\vec{u} \cdot \vec{v})= (\lambda \cdot \vec{u}) \cdot \vec{v}= \vec{u} \cdot (\lambda \cdot \vec{v})$
3. Distributiva respecte la suma: $\vec{u} \cdot (\vec{v}+\vec{w})=\vec{u}\cdot \vec{v}+ \vec{u} \cdot \vec{w}$


####Projecció d'un vector sobre un altre

A vegades ens pot interessar calcular la projecció d'un vector sobre un altre o el que és el mateix, donats dos vectors, buscar quina part d'un d'ells està en la mateixa direcció de l'altre. Fixeu-vos en la construcció següent:

<iframe scrolling="no" src="https://www.geogebra.org/material/iframe/id/2284605/width/1938/height/951/border/888888/rc/false/ai/false/sdz/true/smb/false/stb/false/stbh/true/ld/false/sri/true/at/auto" width="600px" height="350px" style="border:0px;"> </iframe>

Si considerem el triangle rectangle $ABD$, el cosinus de l'angle $\alpha$ es calcula segons:

$$cos \alpha=\frac{AD}{|\vec{u}|} \Rightarrow AD=cos \alpha \cdot |\vec{u}| $$

També sabem que:

$$ \vec{u} \cdot \vec{v}= |\vec{u}| \cdot |\vec{v}| \cdot cos \alpha$$

Per tant, ajuntant les dues expressions tenim que:

$$AD=\frac{\vec{u}\cdot \vec{v}}{|\vec{v}|}$$

El segment $AD$ és la projecció del vector $\vec{u}$ sobre el vector $\vec{v}$, $proj_{\vec{v}}(\vec{u})$, per tant:

>$$proj_{\vec{v}}(\vec{u})=\frac{\vec{u}\cdot \vec{v}}{|\vec{v}|}$$


<!---------------------------------------------------------->
##Combinació lineal entre vectors

Donat un vector $\vec{u}$, si el multipliquem per un nombre real $\lambda$ obtenim una **combinació lineal** d'aquest vector: $\lambda \cdot \vec{u}$. Veiem també que necessàriament el vector i la combinació lineal han de ser **paral.lels** perquè si no, no podríem expressar un com l'altre multiplicat per un nombre.


Per tant, si $\lambda$ i $\mu$ són nombres reals:

>$\lambda \cdot \vec{u}+ \mu \cdot \vec{v}$ és una combinació lineal dels vectors $\vec{u}$ i $\vec{v}$  




###Vectors linealment independents i dependents

Tenint en compte el que hem vist a dalt, diem que:

1. Dos vectors que tenen la mateixa direcció diem que són **linealment dependents** i si tenen diferent direcció són **linealment independents**.
2. Donat un conjunt de vectors, són **linealment dependents** si algun és *combinació lineal* dels altres i són **linealment independents** si cap es pot expressar com a combinació lineal dels vectors restants.

**Exemple 2**

Donats els vectors $\vec{u}=(2,5)$, $\vec{v}=(0,3)$ i $\vec{w}=(-1,1)$ són linealment dependents?

Per comprovar-ho hem de trobar dos nombres $\lambda$ i $\mu$ que compleixin: $\vec{u}=\lambda \cdot\vec{v}+\mu \cdot \vec{w}$:


$$(2,5)=\lambda (0,3)+ \mu (-1,1) \begin{cases} 2 = \lambda \cdot 0- \mu \rightarrow \mu=-2 \\ 5=\lambda \cdot 3 + \mu \rightarrow \lambda = \frac{7}{3}
\end{cases}$$

Veiem que sí que són linealment dependents, perquè podem expressar $\vec{u}$ com a combinació lineal dels altres dos:

$$\vec{u}=\frac{7}{3} \vec{v}-2\vec{w}$$


<!---------------------------------------------------------->
##Bases en el pla
###Canvis de base
###Base ortogonal i ortonormal
