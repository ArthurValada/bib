Estas formas de apresentar os dados são essenciais para a leitura rápida de resultados em qualquer artigo e devem exprimir as partes importantes do seu artigo.

## Tabela
![[Pasted image 20230917112654.png|400]]
Características:
- Laterias abertas;
- Elaboração ou dados autoriais;
- Dados compilados;
- Nome: "Tabela n - O que? Onde? Quando?";

## Tabela de contingência
Usada para  correlacionar diferentes tipos de dados. Por exemplo, se temos uma variável $x$ e uma $y$, podemos apresentar a correlação entre elas com a seguinte estrutura:

|Variáveis| x |$\neg$x| Total|
|---|---|---|---|
| y |   |   |   |
|$\neg$ y|   |   |   |
|Total| |   |   |

Veja que a estrutura correta deveria ter laterais abertas, ao contrário da estrutura apresentada, que é de quadro.

## Quadro
O quadro deve apresentar dados não tratados e analisados e deve ter bordas fechadas:

|Caso|Valor|
|---|---|
| 1 |xxx|
| 2 |xxx|
| 3 |xxx|

**Todas as outras formas de apresentar os dados devem ter laterais abertas**

## Rol
Apenas uma lista de dados de uma única variável, com os dados apresentados de forma ordenada.

## Distribuição de  frequência
É um dado básico para fazer um histograma. Vai relacionar uma classe (um intervalo de [[Conceitos fundamentais#Tipos de variáveis|variáveis]] numéricas ou categoria) a sua frequência absoluta de ocorrência.

No caso de variáveis numéricas, a melhor forma de determinar os intervalos de frequências é calcular o número de intervalos $k = 1 + 3,22 \; log \; n$, onde $n$ é o número de dados da amostra. Tendo o número de intervalos e a amplitude da amostra $A$, a amplitude dos intervalos é $h = \frac{A}{k}$.

## Histograma
Trata-se de um gráfico de barras verticais com o eixo $y$ representando a frequência das classes e o eixo $x$ é dividido nas classes definidas na distribuição de frequência.

## Dispersão
Cada ocorrência com seus dados $(x,y)$ é plotada num plano cartesiano, permitindo visualizar a relação entre $x$ e $y$.

## Box plot
Resumo de 5 números, valor mínimo, máximo e os 3 [[Medidas de tendência central#Mediana e quartis|quartis]].
![[Pasted image 20230917123733.png|300]]
Os valores mínimo e máximo são menores que os dos conjunto de dados, para podermos determinar extremos, assim, o limite inferior e superior de extremos são:
$$LI = x_{Q_1} - 1,5 AI$$
$$LS = x_{Q_3} + 1,5 AI$$
