Estudo de incertezas dentro de um conjunto de possíveis eventos, o **espaço amostral**. Um **evento** é um resultado específico num conjunto de todos os eventos (o espaço amostral). Um evento pode ser **simples** ou **combinado**, de modo que um evento dependa do outro.

## Revisão de conjuntos
- A intersecção de conjuntos $A \cap B$ é o conjunto de elementos (eventos) que estão em $A$ e em $B$ simultaneamente;
- A união de conjuntos $A \cup B$ é a soma (*sem repetição*) dos elementos dos dois conjuntos. Cada elemento em $A \cup B$ está em um ou outro, simultaneamente ou não;
- O conjunto complementar $A^c$ ou $\bar A$ é o conjunto de todos os elementos do espaço amostral que não estão em $A$.
- Tamanho de um conjunto é expresso na forma $n(A)$

## Revisão de contagem
As duas principais formas de combinar eventos são **permutação** e **combinação**, onde
$\text{permutação} \subset \text{combinação}$

A permutação diferencia ordem ($\{a, b\} \ne \{b, a\}$), enquanto a combinação não.

O número de permutações possíveis é dado pelo princípio multiplicativo.

As combinações de um conjunto de $n$ elementos tomados em subconjuntos de tamanho $k$ tem valor de
$$\tbinom{n}{k} = \frac{n!}{k!(n-k)!}$$

## Diagrama de árvore
O diagrama de árvore é usado para visualizar a interação de dois conjuntos de eventos e seus complementares.

Na imagem temos o diagrama de árvore para a probabilidade de dois eventos.
![[Pasted image 20231016203534.png|300]]

## Probabilidade simples
$$P(A) = \frac{n(A)}{n(S)}$$
### Axiomas de Kolmogorov
As probabilidades são construídas para atender os seguintes axiomas:
1. $0 \le P \le 1$
2. $A \cap B = \emptyset \implies P(A \cup B) = P(A) + P(B)$ 
3. $P(A) = 1 \implies A$ é um evento certo de se ocorrer;
#### Teoremas
1. Eventos mutualmente excludentes: $P(A \cap B) = 0$ 
2. $A \subseteq B \implies P(A) \le P(B)$
3. $P(A^c) = 1 - P(A)$
4. $P(A \cup B) = P(A) + P(B) - P(A \cap B)$
