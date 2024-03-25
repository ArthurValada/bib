*Vetores* são grandezas com módulo, direção e sentido.

## Notações
1. Setas:
	- Módulo é o comprimento;
	- Direção é a inclinação;
	- Sentido é dado pela ponta da seta;
2. Dupla de pontos: $\vec v = \vec{AB}$; Ver [[Pontos e coordenadas]].
3. Par ordenado, de forma semelhante a um ponto: $\vec v = (v_x, v_y)$ ou $\vec v = \langle v_x, v_y\rangle$, onde $v_x$ e $v_y$ são componentes de $\vec v$;
4. Notação com soma de vetores da base canônica será explicadas mais adiante;

No caso da notação *2*, o sentido vai ser dado de $A$ para $B$, a  direção vai ser o alinhamento entre os dois pontos e o módulo vai ser a distância $|AB|$ entre eles.

Dessa forma, para a notação *3*, tomamos o primeiro ponto como sendo a origem $O(0,0)$ e o ultimo ponto definimos como $P(v_x, v_y)$, assim, seu módulo pode ser definido como $|\vec v| = |\vec{OP}| = |OP|$.

## Operações de vetores
### Módulo, comprimento ou norma
Como já definimos antes, a *norma* de um vetor $\vec v = (a, b, c)$ é:
$$|\vec v| = \sqrt{a^2 + b^2 + c^2}$$
### Soma
A soma de vetores é dada coordenada por coordenada. Para vetores $\vec v = (v_x, v_y, v_z)$ e $\vec u = (u_x, u_y, u_z)$, temos que:
$$\vec v + \vec u = (v_x + u_x, v_y + u_y, v_z + v_z)$$

#### Propriedades
- Comutatividade: $\vec a + \vec b = \vec b + \vec a$
- Associatividade: $\vec a + (\vec b + \vec c) = (\vec a + \vec b) + \vec c$
- Elemento nulo: $\vec a + 0 = \vec a$. Formalmente usa-se $\vec 0$.
- Inverso aditivo (subtração): $\vec a + (-\vec a) = 0$
> Note que na **maiorias dos casos** $|\vec v| + |\vec u| \ne |\vec v + \vec u|$, exceto quando $\vec v$ e $\vec u$ são paralelos.

### Multiplicação por escalar
Dado um escalar $k \in \mathbb R$ e um vetor $\vec v = (a,b,c)$, definimos o produto de $k$ por $\vec v$ como sendo:
$$k \vec v = (ka, kb, kc)$$
#### Propriedades
- Comutatividade: $k\vec a = \vec a k$
- Associatividade: $(k l)\vec a = k (l\vec a)$
- Associatividade de norma: $|k \vec a| = |k||\vec a|$
- Distributividades: $(k + l)\vec a = k \vec a + l \vec a$ e $k(\vec a + \vec b) = k \vec a + k \vec b$
- Elemento neutro: $1 \vec a = \vec a$
- Elemento nulo: $0 \vec a = 0$. Formalmente diríamos que $0 \vec a = \vec 0$.

As propriedades podem ser verificadas facilmente por meio de algebra, usando a definição das propriedades. Para facilitar as operações algébricas, podemos utilizar os chamados *vetores da base canônica*.

#### Vetores unitários e da base canônica
Um vetor unitário ou *versor* é um vetor de comprimento $1$, que pode ser muito útil para representar direções sem que o módulo seja relevante. Denota-se um versor paralelo a $\vec v$ como $\hat v$ tal que $\hat v = \frac{\vec v}{|\vec v|}$.

Os vetores da base canônica são:
$$\hat i = (1,0,0); \hat j = (0,1,0); \hat k = (0,0,1)$$
Veja que eles são vetores unitários paralelos aos eixos $x, y$ e $z$, respectivamente, dessa forma, podemos denotar qualquer vetor como uma soma destes 3 vetores.
**Exemplo**:
$$(-3, -4, 2) = -3 \hat i -4 \hat k +2 \hat j$$
Você pode verificar isto fazendo a soma dos vetores unitários.

Para um sistema de duas dimensões, temos a base canônica como: $\hat i = (1,0); \hat j = (0,1)$.

### Produtos entre vetores
- [[Produto escalar]];
- [[Produto cruzado]];