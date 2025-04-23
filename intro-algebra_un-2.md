# 2. Relaciones y combinatoria
Cuando formulamos una expresión que vincula o liga dos objetos entre si, en realidad estamos planteando una relación (no necesariamente matemática), es decir que una relación, es un vínculo entre dos objetos. Por ejemplo, 
en una escuela cada estudiante está asignado a un curso.
a cada país del mundo le corresponde al menos una capital. 

En matemáticas, una relación trata de la correspondencia que existe entre dos conjuntos que forman pares ordenados. 

Por ejemplo, supongamos que queremos ordenar los planetas del sistema solar de menor a mayor distancia respecto al sol, estaremos relacionando los conjuntos

$A = \{Tierra, Mercurio, Marte, Saturno Venus, Júpiter, Plutón, Urano, Neptuno\}$

$B = \{1, 2, 3, 4, 5, 6, 7, 8, 9\}$

y la relación que establecemos será:

* $Tierra \to 3$
* $Mercurio \to 1$
* $Marte \to 4$
* $Saturno \to 6$
* $Venus \to 2$
* $Júpiter \to 5$
* $Plutón \to9$
* $Urano \to 7$
* $Neptuno \to 8$

Los pares ordenados provocados por esta relación serán:

$(Tierra, 3), (Mercurio, 1), (Marte, 4), (Saturno, 6), (Venus, 2), (Júpiter, 5), (Plutón, 9), (Urano, 7), (Neptuno, 8)$

En esta unidad, estudiaremos estas relaciones matemáticas y algunas propiedades de las mismas que dan lugar a algunos tipos de relaciones particulares.

## 2.1 Producto cartesiano
Un par ordenado es una pareja de objetos en la cual importa el orden de los mismos, formalmente, dados dos elementos cualesquiera $a$ y $b$, $(a, b)$ es el par ordenado con primera coordenada a y segunda coordenada b.

Dos pares ordenados $(a, b)$ y $(a', b')$ serán iguales cuando sus primeras coordenadas son iguales y sus segundas coordenadas también lo son, es decir que:

$(a, b) = (a', b') \iff (a = a' ∧ b = b')$

Si $A$ y $B$ son dos conjuntos cualesquiera, podemos definir un conjunto llamado conjunto producto o producto cartesiano entre ellos. Este conjunto está formado por todos los pares ordenados que tengan como primera coordenada a un elemento de $A$ y como segunda coordenada a un elemento de $B$. formalmente, esto lo escribiremos como:

$A × B = \{(a, b): a ∈ A ∧ b ∈ B\}$

Veamos un ejemplo acerca de esto, para ello, tomemos $A = \{1, 2, 3, 4\}$ y $B = \{a, b, c\}$ y escribamos todos los pares ordenados posibles: 

Notemos que al elemento $1$ del conjunto $A$ lo podemos asociar con cualquier elemento del conjunto $B$, por lo tanto, los pares ordenados que tienen como primera coordenada al elemento $1$ serán:
$(1, a), (1, b), (1, c)$.


De la misma manera que anteriormente, al elemento $2$ de $A$ podemos asociarlo con cualquier elemento del conjunto $B$, por lo tanto los pares ordenados que tienen como primer coordenada al elemento $2$ serán: 
$(2, a), (2, b), (2, c)$.

Siguiendo de esta forma, los pares ordenados que tienen como primera coordenada al elemento $3$ serán: $(3, a), (3, b), (3, c)$.

Finalmente, los pares ordenados que tiene como primera coordenada al elemento $4$ serán: $(4, a), (4, b), (4, c)$.

## 2.2 Relaciones
Para poder definir el concepto de relación el concepto de producto cartesiano toma especial importancia, ya que dados dos conjuntos $A$ y $B$ dos conjuntos no vacíos, una relación de $A$ en $B$ es un subconjunto del producto cartesiano de $A \times B$. 

Por ejemplo, si tomamos el producto cartesiano del ejemplo anterior

$A \times B = \{(1, a), (1, b), (1, c), (2, a), (2, b), (2, c), (3, a), (3, b), (3, c), (4, a), (4, b), (4, c)\}$

el conjunto $R = \{(1, c), (2, a), (3, a), (4, b)\}$ es una relación de $A$ en $B$. 

Si el par $(a, b)$ pertenece a la relación $R$ vamos a decir que **$a$ está $R$-relacionado con $b$** y a veces lo denotaremos como $R(a,b)$. Si el par $(a, b)$ NO pertenece a la relación se dice que **$a$ no está $R$-relacionado con $b$** y lo escribiremos como $\neg R(a,b)$. 

Sea $R:A \to B; R \subseteq A \times B$

$A$ se denomina conjunto de partida

$B$ se denomina conjunto de llegada

$Dom(R) = \{x ∈ A : \exists y ∈ B: (x, y) ∈ R\}$

$Img(R) = \{y ∈ B: \exists x ∈ A : (x, y) ∈ R\}$

Ejemplo: Sean $A = \{1, 2, 3\}$ y $B = \{0, 1\}$

$R:A \to B; R = \{(1, 0), (1, 1), (3, 0)\}$

$Dom(R) = \{1, 3\} \neq A$

$Img(R) = \{0, 1\}$

Además de los conjuntos vistos hasta el momento, podemos definir la relación inversa $R^ \{-1\} $ como aquella relación derivada de la original en la cual el orden de los elementos es intercambiado. Es decir que si la relación $R$ se define en el producto cartesiano $A \times B$, su relación inversa se define en el sentido contrario, considerando como conjunto de partida $B$ y como conjunto de llegada $A$, por lo cual, la relación inversa es un subconjunto de $B \times A$. Formalmente, esto es 

$R^ \{-1\} = \{(y, x): (x, y)∈R\}$

Por ejemplo, sean $A = \{x: x$ *es un ser humano*$\}$, $B = \{y: y$ *es un gato*$\}$ y la relación $R$ *"$x$ es dueño de $y$"*, la relación inversa será *"$y$ es mascota de $x$"*.

## 2.3 Propiedades de las relaciones
Sea $∼$ una relación en un conjunto $A$, esto es, una relación de $A$ en $A$, el conjunto de partida y el conjunto de llegada de $∼$ son el mismo conjunto $A$.

La relación $∼$ se dice **reflexiva** si para todo $x ∈ A$ se verifica que

$x ∼ x$

La relación $∼$ se dice **simétrica** si para todo $x ∈ A$ y para todo $y ∈ A$ se verifica que

$x ∼ y \implies y ∼ x$

La relación $∼$ se dice **antisimétrica** si para todo $x ∈ A$ y para todo $y ∈ A$ se verifica que

$(x ∼ y ∧ y ∼ x) \implies x = y$

La relación $∼$ se dice **transitiva** si para todo $x ∈ A$, para todo $y ∈ A$ y para todo $z ∈ A$ se verifica que

$(x ∼ y ∧ y ∼ z) \implies x ∼ z$

## 2.4 Relaciones de orden y de equivalencia

Dijimos anteriormente que dependiendo de las propiedades que cumpliera una relación podríamos clasificarlas. En este sentido, existen dos grandes grupos de relaciones en los que haremos hincapié: las relaciones de orden y las relaciones de equivalencia. 

**Llamaremos RELACIÓN DE ORDEN a una relación que es reflexiva, transitiva y antisimétrica.**

Por ejemplo, sea $A = \{1,2,3\}$, definamos la relación $R = \{(1,1),(1,2),(1,3),(2,2),(2,3),(3,3)\}$. La relación es reflexiva ya que dado cualquier elemento $a$ de $A$, el par $(a,a)$ se encuentra en la relación. Además, notemos que la relación es antisimétrica ya que dado un par $(a,b)$ donde $a \neq b$, el par $(b,a)$ no se encuentra en la relación. Finalmente, la relación es transitiva pues: 

$(1,1)∊R, (1,2)∊R \implies (1,2)∊R$

$(1,1)∊R, (1,3)∊R \implies (1,3)∊R$

$(1,2)∊R, (2,2)∊R \implies (1,2)∊R

$(1,2)∊R, (2,3)∊R \implies (1,3)∊R$

$(1,3)∊R, (3,3)∊R \implies (1,3)∊R$

$(2,2)∊R, (2,3)∊R \implies (2,3)∊R$

$(2,3)∊R, (3,3)∊R \implies (2,3)∊R$

Por lo tanto podemos concluir que la relación $R$ *es una relación de orden*.

**Diremos que una relación que cumple las propiedades simétrica, reflexiva y transitiva es una RELACIÓN DE EQUIVALENCIA.**

Por ejemplo, la relación $R = \{(1,1),(2,2),(3,3),(3,4),(4,3),(4,4)\}$ definida sobre el conjunto $A = \{1,2,3,4\}$ es reflexiva, simétrica y transitiva (se deja como ejercicio justificarlo). Por ende la relación $R$ es una *relación de equivalencia*. 

Veamos ahora como una relación de equivalencia particiona el conjunto sobre el cual está definida. Sea $A$ el conjunto sobre el cual definimos una relación de equivalencia $R$. Para esto, tomemos un elemento a del conjunto $A$, la clase de equivalencia de $a$ (a la cual simbolizamos $[a]$) está formada por todos los elementos de $A$ que están relacionados con el elemento $a$, en símbolos esto es: 

$[a]= \{b∊A: R(a,b)\}$

Volviendo al ejemplo anterior, las clases de equivalencia que podemos encontrar son: 

$[1]= \{1\}$ *el 1 solo se relaciona con el 1*

$[2]= \{2\}$ *el 2 solo se relaciona con el 2*

$[3]= \{3,4\}$ *el par (3,4) y el par (4,3) nos dicen que el 3 se relaciona con el 4*

$[4]= \{3,4\}$ *el par $(3,4)$ y el par $(4,3)$ nos dicen que el 3 se relaciona con el 4*

Dadas dos clases de equivalencia cualesquiera, solo tenemos dos posibilidades, o son la misma clase (por ejemplo $[3]=[4]$) o no tienen elementos en común (por ejemplo $[1]$ y $[4]$ no tienen elementos en común).

A cada elemento de una clase de equivalencia lo llamamos **representante** de dicha clase. Dada una relación de equivalencia $R$ en un conjunto $A$, vamos a denominar **conjunto cociente de $A$ determinado por $R$** al conjunto formado por todas las clases de equivalencia $A/R$, es decir que 

$A/R= \{[a]:a∈A\}$

## 2.5 Combinatoria

La combinatoria es una rama de las matemáticas que estudia las agrupaciones u ordenaciones de un determinado número de elementos, es decir que las técnicas de conteo son métodos matemáticos que permiten saber de cuántas formas distintas podemos seleccionar una cierta cantidad de objetos de un conjunto más grande.

Problemas donde es necesario emplear técnicas de conteo se presentan frecuentemente en la vida real, por lo tanto conocer acerca de estas nos permitirá calcular cual es el número de posibilidades de que un evento suceda sin tener que realizar una lista de todos los posibles casos. 

### Principios básicos de conteo

En lo que respecta a las técnicas básicas de conteo hay dos principios que consideramos de importancia revisar: el **principio de la adición** y el **principio de la multiplicación**. Repasemos estos con unos ejemplos.

Felipe desea tener una mascota y desde hace meses pide autorización a su madre para ser dueño de una. Después de evaluar la situación, su madre llega a la conclusión de que el niño es capaz de hacerse cargo de las obligaciones que representa tener un mascota. Es por esto que para el cumpleaños de su hijo, decide llevarlo a un refugio de animales para adoptar una mascota. 

En el refugio hay varios animales esperando ser adoptados y prometiendo dar mucho amor, Felipe quiere llevarse a todos a casa pero su madre, teniendo en cuenta las dimensiones edilicias de su hogar pone como condición que solo puede llevar una. Si en el refugio hay cuatro perros, 3 gatos y 2 hamsters, ¿de cuántas maneras podría Felipe elegir un animal?

Para resolver esto, primero observemos que Felipe puede adoptar solo un perro o un gato o un hamster. En segundo lugar, debemos tener en cuenta que si tenemos tres conjuntos, el conjunto de los perros, el conjunto de los gatos y el conjunto de los hamsters, los mismos no comparten elementos es decir que, por ejemplo, un animal no puede ser gato y perro simultáneamente. En tercer lugar tengamos en cuenta que: 

* El conjunto de los perros cuenta con $4$ animales.

* El conjunto de los gatos cuenta con $3$ animales.

* El conjunto de los hamsters cuenta con $2$ animales.

Por lo tanto las opciones que tiene Felipe para adoptar una mascota son $4 + 3 + 2 = 9$.

Notemos entonces que **para contar los elementos de dos o más conjuntos disjuntos (que no comparten elementos) basta con sumar la cardinalidad (el número de elementos de cada conjunto) de cada uno de ellos**.  

Lo que acabamos de enunciar es el **PRINCIPIO DE LA SUMA**. Formalmente, el mismo dice que si un suceso $A$ puede ocurrir de $n$ maneras diferentes y otro suceso $B$ puede ocurrir de $m$ maneras diferentes, entonces el suceso $A$ o $B$ puede ocurrir de $m+n$ maneras.

Pensemos ahora que vamos al resto-bar *“El Conteo”* a comprar un sándwich. En este comercio podemos elegir llevar un sándwich o de pollo o de carne, y además podemos elegir agregarle palta o huevo o tomate, además de los aderezos: podemos agregarle mayonesa o mostaza o kétchup. ¿De cuántas formas podemos armar nuestro sándwich?

Para calcular de cuántas formas podemos armar nuestro sándwich podemos pensarlo como una cadena de eventos, donde primero sucede la elección de la carne, luego la elección de los extras y finalmente la elección de los aderezos. También notemos que: 

* El conjunto de las carnes, que tiene $2$ elementos

* El conjunto de los extras que tiene $3$ elementos (tomate, palta y huevo)

* El conjunto de los aderezos, que también tiene $3$ elementos. 

Además, notemos que pedir alguna de las opciones de una de las categorías no restringe las elecciones que podemos tomar en las siguientes. Por ejemplo, si elijo carne puedo ponerle huevo, palta o tomate, una vez que elijo entre estas opciones puedo elegir ponerle mayonesa, mostaza o ketchup.

Resulta necesario encontrar una forma de contarlos sin enlistar los elementos o diagramar la situación. Para ello, la elección de la carne puede ocurrir de dos maneras, la decisión de los extras puede ocurrir de tres maneras y la selección de los aderezos también puede realizarse de tres maneras. Es decir,

$C = 2 \cdot 3 \cdot 3$

Aquí hemos aplicado el **PRINCIPIO MULTIPLICATIVO**. Este principio formalmente dice que si un suceso $A$ puede ocurrir de $m$ maneras e independientemente un segundo suceso $B$ puede ocurrir de $n$ maneras entonces el número de maneras en que ambos $A$ y $B$ pueden ocurrir es $m \cdot n$. 

### Permutaciones y combinaciones

Como dijimos al principio, la combinatoria se encarga de estudiar las agrupaciones u ordenaciones de un determinado número de elementos, existen varias formas de realizar estas agrupaciones teniendo en cuenta:

* Si se repiten o no los elementos.
* Si se usan todos o solo algunos de ellos.
* Si importa o no el orden. 

Si el orden *no es importante* estaremos hablando de una **combinación**, en cambio si *el orden sí importa*, estaremos en presencia de una **permutación**.

Más adelante veremos algunas fórmulas de conteo que nos permitirán calcular el número de combinaciones y permutaciones de manera sencilla, sin embargo, para poder entender estas fórmulas necesitamos introducir el concepto de factorial de un número $n$, al que denotamos como $n!$. El factorial de un número entero positivo se define como *el producto de todos los números naturales anteriores o iguales a él*, es decir

$n!=n\cdot(n-1)\cdot(n-2)\cdot\:...\:\cdot1$

y por definición, $0!=1$. 

Ej.: $4! = 4 \cdot 3 \cdot 2 \cdot 1$

#### Fórmulas de conteo

* **Permutaciones** *(importa el orden)*

    Una permutación es una colección de elementos para los que se ha impuesto un ordenamiento.
    
    * **Permutaciones sin repetición**: El número de formas de organizar $r$ objetos de un conjunto de $n$ objetos, en orden pero sin repetición es
    
        $P(n,r)=n\cdot(n-1)\cdot(n-2)\cdot\:...\:\cdot(n-r+1)=\frac{n!}{(n-r)!}$
    
    * Permutaciones con repetición: El número de formas de organizar $r$ objetos en orden elegidos de un conjunto de $n$ objetos si los objetos pueden repetirse es
        
        $n_1 \cdot n_2 \cdot n_3 \cdot\:...\:\cdot n_r = n^{r}$

* **Combinaciones** *(no importa el orden)*

    En una combinación no nos importa el orden de los elementos sino que nos importa cuales elementos son elegidos.
    
    * **Combinaciones sin repetición**: El número de formas de elegir un subconjunto de $r$ objetos de un conjunto de $n$ objetos sin repetición donde $0 \leq r \leq n$ (también llamado **número combinatorio**) es

        $C(n,r)=\begin{pmatrix}n \\ r\end{pmatrix}=\frac{n!}{(n-r)!\cdot r!}$

    * **Combinaciones con repetición**: El número de subconjuntos de $r$ elementos de un conjunto de $n$ elementos distintos con repetición permitida es

        $C((n+r-1),r)=\frac{n+r-1!}{(n-1)!\cdot r!}$

### Binomio de Newton

El **Binomio de Newton** o **Teorema del Binomio**, es una fórmula que permite calcular de forma sencilla las potencias de un binomio $(a+b)^n$. La fórmula del binomio de Newton viene dada por la siguiente expresión:

$(a+b)^{n}=\begin{pmatrix}n \\ 0\end{pmatrix}a^{n}b^{0}+\begin{pmatrix}n \\ 1\end{pmatrix}a^{n-1}b^{1}+\begin{pmatrix}n \\ 2\end{pmatrix}a^{n-2}b^{2}+\:...\:+\begin{pmatrix}n \\ n\end{pmatrix}a^{n-n=0}b^{n}$