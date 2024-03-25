O produto vetorial ou produto cruzado por sua vez possui um [[Vetores no R² e R³|vetor]] como resultado. Esse vetor vai ser sempre perpendicular aos dois multiplicadores, dessa forma, vai ser sempre externo ao plano que os dois multiplicadores pertencem, portanto, esta operação existe apenas em $\mathbb R^3$ (sequer em dimensões superiores).

Tendo os vetores $\vec v = (v_x, v_y, v_z)$ e $\vec u = (u_x, u_y, u_z)$, temos que:
$$\vec v \times \vec u = (v_y u_z - v_z u_y, v_x u_z - v_z u_x, v_x u_y -v_y u_x)$$
## Mnemônicos
Trata-se de uma expressão grande, então usamos de alguns mnemônicos para lembrar.

Uma das formas de lembrar é considerando a ordem de eixos direta como $x, y, z, x, y, z, x, y, z, ...$ e a inversa, o seu contrário, assim, para cada componente do vetor resultante:
- O termo positivo vai ser o produto dos componentes dos multiplicadores nos eixos em ordem direta
- O termo negativo vai ser o produto dos vetores em ordem inversa;
- Exclui-se os componentes do mesmo eixo do componente resultante, então no componente do vetor resultante $y$, vamos multiplicar $xz - zx$, ignorando o $y$;
- Coloca-se sempre os componentes na ordem dos vetores do produto (tomando a notação acima, sempre $v_n u_n$, nunca $u_n v_n$)

Uma forma mais simples de memorizar é usando um processo parecido ao determinante de uma matriz $3 \times 3$, o que não vai ser explicado aqui. Entretanto, nossa "matriz" tem uma peculiaridade: a primeira linha possui o primeiro vetor; a segunda, o segundo vetor; e a terceira, os vetores de base canônica $\hat i, \hat j, \hat k$ (o que via contra às definições formais de matriz). Assim, temos:
$$
\vec v \times \vec u =
\begin{vmatrix}
v_x & v_y & v_z \\
u_x & u_y & u_z \\
\hat i & \hat j & \hat k
\end{vmatrix}
= v_x u_y \hat k + v_y u_z \hat i + v_z u_x \hat j - v_x u_z \hat j - v_y u_x \hat k - v_z u_y \hat i
$$
$$
= \hat k (v_x u_y - v_y u_z) + \hat i (v_y u_z - v_z u_y) + \hat j (v_z u_x - v_x u_z)
= (v_y u_z - v_z u_y, v_x u_z - v_z u_x, v_x u_y -v_y u_x)
$$
## Características e interpretação
Geometricamente, o módulo do produto cruzado pode ser determinado pelo ângulo entre os vetores:
$$|\vec v \times \vec u| = |\vec v||\vec u| sen \theta$$
Vê-se que o produto cruzado se comporta de uma forma oposta ao [[Produto escalar]]: quanto mais perpendiculares os vetores, maior o vetor resultante.

Ressalta-se que $\vec v \times \vec u$ é ortogonal a $\vec v$ e a $\vec u$. Com essas características, principalmente usando do teorema acima, podemos visualizar o módulo do produto cruzado como a área de um paralelogramo definido entre os vetores $\vec v$ e $\vec u$.

Esta característica geométrica nos permite calcular várias construções geométricas a partir de pontos. Por exemplo, com três vértices de um triângulo, podemos gerar dois vetores e pelo produto vetorial, calcular a área do triângulo (equivalente a metade da área do paralelogramo que citamos).

## Propriedades
- Anticomutatividade: $\vec a \times \vec b = - \vec b \times \vec a$
- Associatividade com escalar: $(k\vec a) \times \vec b = k (\vec a \times \vec b) = \vec a \times (k \vec b)$
- Associatividade de produto misto: $\vec a \cdot (\vec b \times \vec c) = (\vec a \times \vec b) \cdot \vec c$
- Distributividade:
	- $\vec a \times (\vec b + \vec c) = \vec a \times \vec b + \vec a \times \vec c$
	- $(\vec a + \vec b) \times \vec c = \vec a \times \vec c + \vec b \times \vec c$
- Associatividade de produto triplo: $\vec a \times (\vec b \times \vec c) = (\vec a \cdot \vec c) \vec b - (\vec a \cdot \vec b)\vec c$

A ultima propriedade não é tão relevante no dia a dia.

## Produtos mistos
O produto $\vec a \cdot (\vec b \times \vec c)$ é chamado de *produto misto* ou *produto triplo* e tem propriedades particularmente interessantes. A primeira é que é verdade o determinante abaixo:
$$\vec a \cdot (\vec b \times \vec c) =
\begin{vmatrix}
a_x & a_y & a_z \\
b_x & b_y & b_z \\
c_x & c_y & c_z
\end{vmatrix}
$$
O que pode agilizar certos cálculos. A segunda propriedade interessante é o significado geométrico da operação: o produto misto pode ser entendido como o volume de um paralelogramo delimitado pelos vetores do produto, como melhor demonstrado na imagem abaixo. Obviamente convém tirar o módulo do produto misto, já que não existem volumes negativos.
![[Pasted image 20230818183252.png|300]]

É um bom momento para fazermos alguns exercícios de pensamento: Por que as operações abaixo não são definidas?
- a) $\vec a \cdot \vec b \cdot \vec c$
- b) $\vec a \times (\vec b \cdot \vec c)$
- a) $\vec a \times \vec b \cdot c$
