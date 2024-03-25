## Média aritmética
$$\bar x = \frac{\sum x_i}{n}$$
A média aritmética é sensível a valores extremos.
## Média ponderada
Dado um vetor de pesos $\vec p$ e o nosso vetor de dados amostrais $\vec x$, podemos escrever a média ponderada como
$$\bar x_p = \frac{\vec p \cdot \vec x}{\sum p_i}$$
Permite dar pesos diferentes a valores de relevâncias diferentes.
## Moda
Valor de maior frequência. Quando um conjunto de dados não possui repetições, chamamos de amodal. A divisão em classes usada na [[Visualização de dados#Distribuição de frequência|distribuição de frequências]] permite que variáveis contínuas tenham moda. Uma distribuição com dois máximos relativos pode ser chamada de bimodal. O mesmo vale para multimodal. 
## Mediana e quartis
Para dados ordenados, os quartis vão ser os índices dos dados na posição de $\frac{1}{4}, \frac{2}{4}$ e $\frac{3}{4}$ do conjunto de dados. São chamados de primeiro, segundo e terceiro quartil os elementos nas posições
$$Q_1 = \frac{1}{4}(n + 1)$$
$$Q_2 = \frac{2}{4}(n + 1)$$
$$Q_3 = \frac{3}{4}(n + 1)$$
Assim, o elemento na posição $x_{Q_1}$ é maior que $25\%$ dos dados e menor que $75\%$ dos dados.

O segundo quartil $Q_2$ é conhecido como **mediana**.

Caso o valor do quartil não seja um número inteiro, deve-se arredonda-lo, exceto se for múltiplo de $\frac{1}{2}$, neste caso se tira a média do número arredondado para baixo e do arredondado para cima.

Por exemplo, se $n=9$, $Q_1 = \frac{10}{4} = 2,5$, assim, $x_{Q_1} = \frac{x_2 + x_3}{2}$.

### Formatos de distribuição
Em geral muitos conjuntos de dados se comportam como uma distribuição normal, (em formato de sino), em que a média é igual a mediana e é o ponto de simetria da distribuição. No entanto, distribuições podem ter assimetrias ("caudas"), para a esquerda ou direita.

Como a mediana não é sensível a extremos, ela tende a permanecer próxima da moda (o pico da distribuição), enquanto que a média já é "puxada" por esses extremos. Assim, se
- $\bar x \approx x_{Q_2},$ a distribuição tende a ser simétrica;
- $\bar x > x_{Q_2}$, a distribuição tem uma assimetria ("cauda") para a direita, e a concentração fica para a esquerda;
- $\bar x < x_{Q_2}$, a distribuição tem uma assimetria ("cauda") para a esquerda, e a concentração fica para a direita;

Veja nestes histogramas como a média é mais "puxada" para a direção das assimetrias.
![[Pasted image 20230917163606.png]]