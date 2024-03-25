Uma equação linear é uma equação na forma
$$\sum a_i x_i= b$$
Onde $a_1,\dots, a_n, x_1, \dots x_n, b \in \mathbb R$. Aqui definimos $a_i$ como coeficientes e $x_i$ como incógnitas. Tomando $m$ equações com $n$ incógnitas como verdadeiras, temos um sistema $n \times m$ que pode ser escrito na forma
$$\begin{cases}
a_{11} x_{1} + \dots + a_{1n} x_{n} = b_1 \\
a_{21} x_{1} + \dots + a_{2n} x_{n} = b_2 \\
\dots \\
a_{m1} x_{1} + \dots + a_{mn} x_{n} = b_m \\
\end{cases}$$
O sistema de equações pode ser escrito como o produto da matriz de coeficientes $A_{n \times m} = \{a_{ij}\}$ pelo vetor de incógnitas $\vec x = (x_1, \dots, x_n)$ resultando no vetor de coeficientes $\vec b = (b_1, \dots, \vec b_n) \; t.q.\; A \vec x = \vec b$, ou seja:
$$
\begin{bmatrix}
a_{11} & \dots & a_{1n}\\
\vdots & \dots & \vdots\\
a_{m1} & \dots & a_{mn}\\
\end{bmatrix}
\begin{bmatrix}
x_1 \\ \vdots \\ x_n
\end{bmatrix}
=
\begin{bmatrix}
b_1 \\ \vdots \\ b_n
\end{bmatrix}
$$
O sistema pode ser resolvido pelo escalonamento da matrix expandida $(A|\vec b)$
$$
\left[
\begin{array}{(ccc|c)}
a_{11} & \dots & a_{n1} & b_1 \\
\vdots & \dots & \vdots & \vdots\\
a_{m1} & \dots & a_{mn} & b_m \\
\end{array}
\right] \tag 1
$$
Em que as linhas são equações e as colunas são as incógnitas, com os valores $a_{ij}$ sendo os coeficientes da incógnita $x_j$ na equação $i$.

Um sistema de equações lineares é dito *homogêneo* se $\vec b = \vec 0$.

## Soluções de sistemas lineares
Uma *solução* de um sistema linear é o conjunto de variáveis $x_i$ que atende a todas as equações simultaneamente.

Uma solução pode ser entendida como um ponto contido na intersecção entre todos os [[Variedades afim e hiperplanos|hiperplanos]] no sistema de equações.

Um sistema linear pode ter as seguintes propriedades quanto suas soluções:
- *Inconsistente*: não existe nenhum conjunto de variáveis que obedeça todas as equações simultaneamente (os hiperplanos são *paralelos*);
- *Consistente* com um **único** conjunto solução (os planos se interceptam em apenas um ponto);
- *Consistente* com **infinitas** soluções (os planos se interceptam em outra subvariedade afim que pode ser parametrizada);

![[Pasted image 20231031113703.png]]

**Exemplo de sistema inconsistente:**
$$
\left[
\begin{array}{(ccc|c)}
1 & 0 & 0 & a \\
0 & 1 & 0 & b\\
0 & 0 & 0 & c \\
\end{array}
\right]
$$
Se um dado $c \ne 0$, a última equação $c$ é impossível.

> Quando um sistema possui infinitas soluções, pelo menos uma das variáveis é *livre*, podendo ser parametrizada, sendo as demais *fixas* ou *dependentes*.

Se um sistema possui $n$ variáveis livres, o conjunto solução forma um hiperplano de dimensão $dim(H) = n$. Variáveis dependentes vão apenas mudar a inclinação do hiperplano.

Considerando uma matriz expandida da expressão $(1)$, após o escalonamento de Gauss - Jordan, podemos ver as soluções possíveis.

### Soluções para sistema homogêneo
- Um sistema **homogêneo** sempre tem **pelo menos uma solução *trivial*** $(0, \dots, 0)$, não podendo ser inconsistente;
**Exemplo:**
$$
\left[
\begin{array}{(ccc|c)}
1 & 0 & 0 & 0 \\
0 & 1 & 0 & 0\\
0 & 0 & 1 & 0 \\
\end{array}
\right]
$$
A única solução possível é $x_1 = x_2 = x_3 = 0$.

- Se uma linha $i$ possui apenas um número não nulo na coluna $j$, então $x_j = 0$;
**Exemplo:**
$$
\left[
\begin{array}{(ccc|c)}
0 & b & 0 & 0 \\
0 & 0 & a & 0\\
0 & 0 & 0 & 0 \\
\end{array}
\right]
$$
$x_2 = x_3 = 0$, são variáveis fixas e $x_1$ é uma variável livre, que pode ser parametrizada, por exemplo com o parâmetro $x_1 = t,\, t \in \mathbb R$, gerando infinitas soluções (contidas numa reta paralela ao eixo $x_1$).

- Se uma linha $i$ possui dois números não nulos, temos pelo menos uma variável dependente;
**Exemplo:**
$$\left[
\begin{array}{(ccc|c)}
a & b & 0 & 0 \\
0 & 0 & c & 0 \\
0 & 0 & 0 & 0
\end{array}
\right]$$
$x_3 = 0$ é uma variável livre,  e $a x_1 = -b x_2$, de modo que uma das duas é livre e a outra é dependente. O conjunto solução resultante é um plano na forma
$$h = \{(t, -\frac{a}{b}t, s) \; t.q.\; t,s \in \mathbb R\}$$

### Soluções para sistemas gerais
- Se uma linha possui apenas $0$, então ela não dá nenhuma informação e pode ser descartada (sabemos que $0x_i = 0$);
- Se um sistema tem $n$ variáveis e $m$ equações, tal que $n>m$, ele possui no mínimo $n-m$ variáveis livres.
**Exemplo:** O sistema
$$
\left[
\begin{array}{(ccc|c)}
1 & 0 & 0 & a \\
0 & 0 & 0 & 0\\
0 & 0 & 1 & b \\
\end{array}
\right]
$$
Tem as mesmas soluções que
$$
\left[
\begin{array}{(ccc|c)}
1 & 0 & 0 & a \\
0 & 0 & 1 & b\\
\end{array}
\right]
$$
Este sistema possui $m = 2$ equações (relevantes) e $n = 3$ variáveis, de modo que 

- Se uma linha $i$ da matriz da esquerda tiver apenas um $1$ na coluna $j$, então $x_j = b_i$;
**Exemplo:**
$$
\left[
\begin{array}{(ccc|c)}
0 & 1 & 0 & a \\
0 & 0 & 1 & b\\
0 & 0 & 0 & 0 \\
\end{array}
\right]
$$
$x_2 = a, \, x_3 = b$ e $x_3$ é uma variável livre.

- Se uma linha tem pelo menos um número a direita do pivô, uma das variáveis é dependente;
**Exemplo:**
$$
\left[
\begin{array}{(ccc|c)}
1 & d & 0 & a \\
0 & 0 & 1 & b\\
0 & 0 & 0 & 0 \\
\end{array}
\right]
$$
$x_3 = b$ é uma variável fixa e $x_1 + d x_2 = a$. Assim uma das variáveis é fixa e a outra dependente, assim o conjunto solução forma uma reta.

- Uma consequência óbvias do escalonamento: uma variável dependente só pode depender de uma variável livre, não de uma fixa;
- Se o sistema não tem variáveis livres, seu determinante é não nulo;
- Se as linhas são [[Combinação e dependência linear|linearmente independentes]], então a matriz tem uma solução **única** e vice-versa; 
