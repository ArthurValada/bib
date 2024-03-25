O produto escalar é o produto de dois [[Vetores no R² e R³|vetores]] com o resultando como um escalar. Definimos o produto escalar como a soma do produto de cada coordenada, ou seja, para $\vec u = (u_x, u_y)$ e $\vec v = (v_x, v_y)$, temos:
$$\vec u \cdot \vec v = u_x v_x + u_y v_y$$
Geometricamente, colocando a origem dos vetores no mesmo ponto, podemos construir um triângulo e, pela lei dos cossenos, é possível deduzir o teorema:
$$\vec a \cdot \vec b = |\vec a||\vec b| cos \theta$$

Por ser uma das primeiras operações "novas" apresentadas ao aluno de ensino superior, é interessante analisar seu comportamento, que pode ser melhor compreendido pela expressão geométrica acima. Dela, fica claro que o produto escalar:
- É proporcional ao módulo dos dois vetores, quanto maiores forem, maior o produto;
- Aumenta quão mais os vetores são alinhados, quão menor é o ângulo entre eles, tendo seu maior valor quando são paralelos ($cos 0 = 1$) e menor módulo quando são perpendiculares ($cos\frac{\pi}{2} = 0$).
> Entende-se o produto escalar entende-se uma medida de alinhamento dos vetores, de quão são similares.
## Propriedades
- Comutatividade: $\vec a \cdot \vec b = \vec b \cdot \vec a$
- Associatividade com escalar: $(k\vec a) \cdot \vec b = k(\vec a \cdot \vec b) = \vec a \cdot (k\vec b)$
- Distributividade: $\vec a \cdot (\vec b + \vec c) = \vec a \cdot \vec b + \vec a \cdot \vec c$ 
- Elemento nulo: $0 \cdot \vec a = 0$. Formalmente: $\hat 0 \cdot \vec a = 0$
- Quadrado: $\vec a \cdot \vec a = |\vec a|^2$

## Componentes e projeções
Aqui definimos a operação *projeção* ou *vetor projeção*, $proj_{\vec a}(\vec b)$ (lê-se: projeção de b em a) como a construção geométrica da figura abaixo.

É um conceito difícil de explicar verbalmente, mas que pode ser entendido como a sombra de $\vec b$ sobre $\vec a$, como se $\vec a$ fosse um plano e fosse projetada uma luz completamente perpendicular a esse plano, daí, essa sombra é o vetor projeção.

Outra forma de entender é como a parte de $\vec b$ na direção de $\vec a$, excluindo a parte perpendicular.

![](Pasted%20image%2020230816200853.png)

Outra operação que definimos é a *projeção escalar*, que prefiro chamar de *componente*, $comp_{\vec a}(\vec b)$ (lê-se: componente de b na direção de a), que nada mais é que a norma do vetor projeção: $comp_{\vec a}(\vec b) = |proj_{\vec a}(\vec b)|$.

Quando queremos projetar um vetor em uma dada direção, basta multiplicar o vetor pelo versor da direção. Isso pode ser visto de forma mais intuitiva com os vetores da base canônica: $\vec v \cdot \hat i = v_x$ e $\vec v \cdot \hat j = v_y$. Veja que $v_x$ é o componente de $\vec v$ na direção de $\hat i$ e o mesmo vale para $v_y$ e $\hat j$. Sabendo disso, fica fácil de lembrar que a fórmula para componente de um vetor é:
$$comp_{\vec a}(\vec b) = \hat a \cdot \vec b$$
Ou seja:
$$comp_{\vec a}(\vec b) = \frac{\vec a}{|\vec a|} \cdot \vec b$$
Para achar a fórmula da projeção, basta usar o fato de que o componente é o módulo da projeção. Como a projeção é um vetor, precisamos "adicionar" uma direção ao componente e por definição a direção é a direção de $\vec a$, que é $\hat a$:
$$
|proj_{\vec a}(\vec b)| = comp_{\vec a}(\vec b)
\implies proj_{\vec a}(\vec b) = comp_{\vec a}(\vec b) \hat a
$$
Lembre-se de que esta é uma multiplicação de um vetor ($\hat a$) por um escalar ($comp_{\vec a}(\vec b)$). Expandindo:
$$
\implies proj_{\vec a}(\vec b) = \left(\frac{\vec a}{|\vec a|} \cdot \vec b \right)\frac{\vec a}{|\vec a|}
$$
Reorganizando, temos:
$$
\implies proj_{\vec a}(\vec b) = \vec a \cdot \vec b \frac{\vec a}{|\vec a|^2}
$$

## Produto misto
Ver [[Produto cruzado#Produtos mistos|produto misto]].