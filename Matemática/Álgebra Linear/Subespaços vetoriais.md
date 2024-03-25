Um *subespaço vetorial* nada mais é que um [[Espaços vetoriais|espaço vetorial]] contido dentro de outro subespaço vetorial. Em outras palavras, se $E$ e $F$ são espaços vetoriais e $F \subset E$, então diz-se que $F$  é subespaço de $E$.
## Definição
Para se preservar enquanto espaço vetorial, um dado subconjunto $F$ de $E$ precisa atender as seguintes propriedades (os demais axiomas provêm de $E$):
1. $\vec 0 \in F$
2. $\forall \vec u, \vec v \in F \implies \vec u + \vec v \in F$
3. $\forall \alpha \in \mathbb R \forall \vec u \in F \implies \alpha \vec u \in F$
> Aqui estamos assumindo que $\mathbb R$ é o conjunto de escalares de $E$.

O que isso tudo nos diz é que o vetor nulo precisa continuar no subespaço e que as somas e produtos de vetores não podem sair do subespaço.

### Exemplo 1
$\{\vec 0\} \in E$ e o próprio $E$ são subespaços triviais de $E$.

### Exemplo 2
Uma reta construída a partir de um  vetor não nulo $\vec v \in E$, da forma $F = \{\alpha \vec v \; t.q. \; \alpha \in \mathbb R\}$ é um subespaço de $E$, com todos os vetores sendo produtos do vetor diretor $\vec v$.

### Exemplo 3
O conjunto $\mathcal H$ de todos os vetores $\vec v = (x_1, ..., x_n) \in \mathbb R^n$ em que
$$\alpha_1 x_1 + ... + \alpha_n x_n = 0$$
é um subespaço de $\mathbb R^n$. No caso de todos os coeficientes serem nulos, $\mathcal H = \mathbb R^n$ e no caso contrário, $\mathcal H$ define um *hiperplano* em $\mathbb R^n$ que passa pela origem.

## União de subespaços
O conjunto $F = F_1 \cup F_2$, onde $F_1, F_2 \subset E$, é formado por todas as somas $\vec v_1 + \vec v_2, \, \forall \vec v_1 \in F_1, \, \forall \vec v_2 \in F_2$. Assim, escreve-se $F = F_1  + F_2$. Quando um conjunto $X = \{\vec u\}$ possui apenas um elemento, escrevemos a soma na forma $\vec u + F$ e diz-se que $\vec u$ *translada* o conjunto $F$.

Quando $F_1 \cap F_2 = \{\vec 0\}$, a soma desses dois subespaços é chamada *soma direta* e é denotada como $F = F_1 \oplus F_2$.

### Teorema
Sejam $F_1, F_2, F$ subespaços vetoriais de $E$, então $F = F_1 \oplus F_2$, se e somente se todo elemento de $\vec u \in F$ é obtido de forma **única** pela soma $\vec u = \vec v_1 + \vec v_2\; t.q. \; \vec v_1 \in F_1, \, \vec v_2 \in F_2$.