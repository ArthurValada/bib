*Eixos coordenados* podem ser denominados por letras e representam a direção que a coordenada cresce, a direção positiva. Eixos também possuem uma *origem* $O$ onde os eixos se interceptam com o valor de $0$.

Um *ponto* é um conjunto de demarcações em cada um dos eixos que demarca um local único.

*Planos coordenados* são os planos que contém dois eixos do sistema. Por exemplo, o plano $xy$ contem os eixos $x$ e $y$, e é perpendicular a $z$.

A notação para pontos num espaço bidimensional é uma dupla (ou par) ordenada $P(a, b)$, onde $a$ e $b$ são as coordenadas $x$ e $y$ do ponto $P$. Num espaço tridimensional a notação é $P(a,b,c)$.

Como $\mathbb R$ é o conjunto de ordenadas em um único eixo,  o produto cartesiano $\mathbb R \times \mathbb R = \mathbb R^2$ vale para 2 eixos e o mesmo processo nos dá $\mathbb R^3$ para 3 eixos.

Um gráfico de uma equação que relaciona $x$ a $y$ em $\mathbb R^2$ se chama *curva* e uma equação que relaciona $x, y$ e $z$ se representa uma *superfície* em $\mathbb R^3$.

Quando uma coordenada não está contida numa equação, ela se chama *variável livre* e a superfície resultante vai ter todas as combinações possíveis de variáveis livres.

**Exemplo:** a equação $x = y$ resulta numa superfície com pontos $(a,b,c)$ com todos os valores de $c \in \mathbb{R}$ desde que $a = b$, onde $c$ é a variável livre.

## Distância entre pontos
A distância entre o ponto $P_1(x_1, y_1, z_1)$ e o ponto $P_2(x_2, y_2, z_2)$ é denotada como $|P_1P_2|$ e é dada por:
$$|P_1P_2| = \sqrt{(x_2-x_1)^2 + (y_2-y_1)^2 + (z_2-z_1)^2}$$
É como deslocar a vértice de um triângulo retângulo para $P_1$ e calcular sua hipotenusa até $P_2$.

## Equação da esfera
Uma esfera é definida como uma superfície com todos os pontos equidistantes ao centro.

Matematicamente, basta definimos que um ponto $P(x,y,z)$ pertence à superfície de uma esfera que possui centro em $C(a, b, c)$ se ele estiver precisamente a uma distância $r$ do centro, ou seja, $r = |CP|$.

Se alterarmos esta equação para inequações como $r > |CP|$, todos os pontos que pertencem à inequação estão dentro do volume da esfera.