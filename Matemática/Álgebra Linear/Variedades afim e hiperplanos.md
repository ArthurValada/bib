O subconjunto $V \subset E$, onde $E$ é um [[Espaços vetoriais|espaço]], é uma *variedade afim* se e somente se, $\forall \vec x, \vec y \in V,$
$$r = \{(1-t) \vec x + t \vec y \;t.q.\; t \in \mathbb R\} \subset V$$
O que pode ser simplificado com o vetor diretor $\vec v = \vec y - \vec x$, de modo que $r$ é a reta $r = \{\vec x + t \vec v \;t.q.\; t \in \mathbb R \}$.

Todo espaço vetorial é por definição, variedade afim, no entanto, variedades afim não precisam ter o vetor nulo. Assim, sempre podemos obter um único subespaço $F \subset E$ *transladando* uma variedade $V$ de modo que
$$V = \vec x + F = \{\vec x + \vec v \; t.q.\; \vec v \in F\}$$
Onde $V$ é obtido pela translação de $F$ por $x$ e que $F$ é *paralelo* a $V$ e vice-versa.

Uma *subvariedade afim* é um subconjunto de uma variedade afim que mantem suas propriedades enquanto variedade afim

## Hiperplanos
Um *hiperplano* $H$ é o conjunto de todos os vetores $\vec x = (x_1, \dots, x_n) \in \mathbb R^n$ tais que
$$a_1 x_1 + \dots + a_n x_n = b$$
Onde $a_1, \dots, a_n, b \in \mathbb R$. Um sistema de $m$ [[Sistemas lineares|equações lineares]] com $n$ incógnitas é a interseção de $m$ hiperplanos, que também é um hiperplano.

O caso especial em que $b = 0$, de modo que a equação linear se chame de homogênea, é onde o ponto $(0, \dots, 0) \in H$.
