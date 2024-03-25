## Combinação linear
*Combinação linear* é a operação de somar $n$ vetores de um dado conjunto, antes multiplicando cada um por coeficientes, de modo a gerar um novo vetor.
$$\vec v = \alpha_1 \vec u_1 + ... +\alpha_n \vec u_n$$
Onde $\alpha _i$ pertencem ao corpo dos escalares e são os coeficientes da combinação linear; $\vec u_i$ são os vetores a se combinar e $\vec v$ é o vetor resultante. Outra forma de escrever a operação é: dado um espaço $E$ e um conjunto de vetores $\vec e_i \in X \subset E$, com $n$ vetores, o vetor $\vec v \in E$ é resultado da combinação linear dos vetores em $X$ se
$$\vec v = \sum_{i=0}^n a_i \vec e_i$$
> Veja que $X$ não precisa ser um subespaço vetorial, apenas um subconjunto de $E$.

A combinação linear de vetores é uma operação que decorre diretamente das operações definidas dentro de um [[Espaços vetoriais|espaço vetorial]].

## Dependência linear
Se um vetor $\vec v$ pode ser obtido pela combinação linear dos vetores $\vec u, \, \vec w$ diz-se que $\vec v$ é *Linearmente Dependente* ($L.D.$) de $\vec u$ e $\vec w$. Caso $\vec v$ não possa ser obtido pela combinação linear desses dois vetores, ele é *Linearmente Independente* ($L.I.$) desses dois vetores.

O mesmo conceito pode ser aplicado para conjuntos de vetores, mas para conjuntos, ao invés de checar se cada vetor pode ser escrito em termos dos demais, basta checar a seguinte condição:
$$\vec 0 = \sum_{i=0}^n \alpha_i \vec e_i, \,se\; \forall \alpha_i \neq 0$$
Ou seja, se a **única** forma de combinar os vetores para obter o vetor nulo é tornado os coeficientes $0$, então o conjunto é $L.I.$

Essa condição pode ser reescrita como um [[Sistemas lineares|sistema linear homogêneo]].
### Exemplo 1
Dado um conjunto $X = \{\vec u, \vec v, \vec w\} \subset E$, e $\alpha, \beta, \gamma \in \mathbb R^*$, sabendo que os elementos de $X$ não são nulos, e ainda assim é possível escrever
$$\vec 0 = \alpha \vec u + \beta \vec v + \gamma \vec w$$
Então $X$ é $L.D.$
