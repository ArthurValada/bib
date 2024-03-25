## Definição
Um *Espaço vetorial* é qualquer **conjunto** de elementos com certas propriedades citadas abaixo, associado a um conjunto auxiliar chamado conjunto dos *escalares*, que atende as propriedades de *corpo* (tomemos como exemplo: $\mathbb R$ ou $\mathbb C$). Os elementos de um espaço vetorial são os vetores.
- Pode se definir uma operação de *soma vetorial*, com as propriedades:
	1. Comutatividade de soma;
	2. Associatividade de soma;
	3. Existência de elemento neutro aditivo dentro do espaço;
	4. Existência de inverso aditivo;
- Pode se definir uma operação de *multiplicação por escalar* com o vetor, com as propriedades:
	5. Associatividade de multiplicação;
	6. Existência de elemento neutro multiplicativo dentro do espaço;
	7. Distributividade da soma com a multiplicação;
	8. Distributividade da multiplicação com a soma;

As mesmas propriedades, os *axiomas* destas operações, podem ser expressas na seguinte forma, tomando $E$ como um espaço vetorial; $\vec u, \vec v, \vec w \in E$ três vetores quaisquer; $\vec 0 \in E$ o vetor nulo da adição; e $\alpha, \beta$ dois elementos quaisquer do corpo dos escalares:
1. $\vec u + \vec v = \vec v + \vec u$
2. $\vec u + (\vec v + \vec w) = (\vec u + \vec v) + \vec w$
3. $\vec 0 + \vec u = \vec u$
4. $\forall \vec u \in E, \exists (- \vec u) \in E \; t.q. \; \vec u + (- \vec u) = \vec 0$
5. $\alpha(\beta \vec u) = (\alpha \beta) \vec u$
6. $1 \vec u = \vec u$
7. $(\alpha + \beta)\vec u = \alpha \vec u + \beta \vec u$
8. $\alpha(\vec u + \vec v) = \alpha \vec u + \alpha \vec u$

> Note que $1$ é o elemento neutro da multiplicação quando o corpo dos escalares é $\mathbb R$, mas pode ser definido como outro número em contextos bastante específicos.

> Note também que, ao definirmos a soma de vetores $\vec u + \vec v = \vec w$, fica implícito que $\vec w \in E$ e que, caso não atenda a esta definição, a soma não fica definida adequadamente e $E$ não é um espaço vetorial. O mesmo vale para a definição de multiplicação $\alpha \vec u = \vec v$.

Veja que na álgebra linear, um vetor pode ser muitas coisas para além do que é definido na geometria analítica. Abaixo temos os exemplo mais importantes.
## Exemplo 1
No caso mais trivial, como os axiomas de espaço vetorial são um subconjunto dos teoremas de corpo (exceto que um espaço vetorial não precisa ter uma operação de multiplicação definida do próprio conjunto), então todo corpo é também um espaço vetorial, como no caso de $\mathbb R$ e $\mathbb C$.
## Exemplo 2
$\mathbb R ^2$ e $\mathbb R ^3$ também são espaços vetoriais, com os axiomas bem definidos e mostrados em [[Vetores no R² e R³]]. Na verdade, é fácil demonstrar que $\mathbb R^n$ é um espaço vetorial, se definirmos os vetores como n-tuplas ordenadas de forma 
$$\vec u, \vec v \in \mathbb R^n \; t.q. \; \vec u = (u_1, ..., u_n),\, \vec v = (v_1, ..., v_n)$$
e as operações
$$\vec u + \vec v = (u_1 + v_1, ..., u_n + v_n)$$
e, 
$$\forall \alpha \in \mathbb R,\, \alpha \vec u = (\alpha u_1, ..., \alpha u_n)$$
então decorre das propriedades de $\mathbb R$ aplicadas aos componentes dos n-tuplas, que $\mathbb R ^n$ é um espaço vetorial. De forma similar se demonstra para $\mathbb R^ \infty$. Veja que aqui não estamos provando formalmente o afirmado para fins de compreensão. A prova formal ficará a cargo do leitor.

## Exemplo 3
Séries e polinômios também podem ser representados por n-tuplas ordenadas, por exemplo:
$$P_3(x) = p_0 + p_1 x + p_2x^2 + p_3x^3 \in \mathcal P_3$$
pode ser escrito como
$$\vec p = (p_0, p_1, p_2, p_3) \in \mathcal P_3$$
Além disso, polinômios tem suas somas e multiplicação por escalares bem definidas. Ambos estes fatores permitem concluir com facilidade que $\mathcal P_3, \mathcal P_n$ e $\mathcal P_\infty$ são também espaços vetoriais.

## Exemplo 4
Para quaisquer funções $f, g, h: X \to \mathbb R$ denotado como $\mathcal F(X; \mathbb R)$, ou seja, qualquer função que tenha como contradomínio o corpo dos reais, podemos definir:
$$(f + g)(x) = f(x) + g(x)$$
e
$$(\alpha f)(x) = \alpha f(x)$$
Note que devido ao contradomínio das funções, temos que $f(x), \,g(x), \,h(x) \in \mathbb R$, assim, podemos usar as propriedades dos reais para encontrar as propriedades do conjunto que estamos estudando. Por exemplo, para provar a associatividade da soma,
$$(f + g)(x) + h(x) = f(x) + (g + h)(x)$$
basta saber que todos os termos da equação acima são reais e usar a própria definição da soma dada acima. Com efeito, é imediato que $\mathcal F (X; \mathbb R)$ é um espaço vetorial.
> Note que $\mathcal F (X; \mathbb R)$ ser um espaço vetorial não implica diretamente em $\mathcal P_n$ ser um espaço vetorial, apesar de a demostração ser similar.

## Exemplo 5
As matrizes tem soma, subtração e multiplicação por escalar bem definidas, assim, é fácil provar que elas formam um espaço vetorial. Lembre-se da notação $M_{n \times m} = \{ m_{ij} \}$, que permite operar para cada elemento da matriz e facilitar no processo de demonstração dos axiomas.

## Exemplo 6
O conjunto $\mathbb R^{2+} = \{(a, b) \; \forall a, b \in \mathbb R^+\}$, ou seja, o conjunto de todos os vetores que apontam da esquerda para a direita, não é um espaço vetorial, pois tomando $\vec u = (a, b) \in \mathbb R^{2+}$, implica que $- 1\vec u = (- 1a, - 1b) \notin \mathbb R^{2+} \therefore \mathbb R^{2+}$ não atende ao axioma **4** e assim não é espaço vetorial.

No entanto, é possível definir as operações de modo a tornar este conjunto um espaço vetorial.

$\mathbb R^2 - \{\vec 0\}$ não é um espaço vetorial devido ao axioma **3**.