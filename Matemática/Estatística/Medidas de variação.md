## Amplitude
$$A = x_{max} - x_{min}$$
A amplitude é o intervalo de valores que do conjunto de dados. É extremamente sensível a extremos.
## Amplitude interquartil
Trata-se da amplitude entre $Q_1$ e $Q_3$, o que permite ignorar os valores mais extremos do conjunto de dados.
$$AI = x_{Q_3} - x_{Q_1}$$
## Desvio da média
Sabendo a [[Medidas de tendência central#Média aritmética|média]] de um conjunto de dados, é possível saber como cada dado desvia da média
$$x'_i = x_i - \bar x$$
Como consequência temos
$$\sum x'_i = 0$$
Assim, não é possível calcular um desvio médio. O desvio permite calcular extremos, por meio do.
## Variância amostral
$$S^2 = VAR = \frac{\sum (x_i - \bar x)^2}{n-1} = \frac{\sum (x'_i)^2}{n-1}$$
Trata-se de um valor com dimensões inconvenientes e de valor exagerado, assim, só é usado para calcular o desvio padrão:
## Desvio padrão amostral
$$S = \sqrt{S^2} = \sqrt{\frac{\sum (x'_i)^2}{n-1}}$$
Não confundir com o *desvio padrão populacional*, representado por $\sigma$.
## Score Z
O score Z é uma convenção usada para saber se um dado valor é ou não extremo. O seu valor é calculado como
$$Z = \frac{x'_i}{S}$$
Com isso, se $|Z| > 3$, concluímos que o valor é um extremo. O sinal do conjunto diz se o extremo é inferior ou superior.
## Covariância
A covariância é dada por
$$Cov(X, Y) = \frac{\sum x'_i y'_i}{n-1}$$
e serve apenas para dizer se os valores variam no mesmo sentido ou não (sem dizer intensidade).
A forma mais prática de calcular a covariância de dois conjuntos de dados é construindo uma tabela do tipo:

| |$x$|$y$|$x'$|$y'$|$x'y'$|
|---|---|---|---|---|---|
|$1$|$x_1$|$y_1$|$x_1 - \bar x$|$y_1 - \bar y$|$x'_1y_1'$|
|...|...|...|...|...|...|
|$n$|$x_n$|$y_n$|$x_n - \bar x$|$y_n - \bar y$|$x'_ny_n'$|
|$\Sigma$|$\sum x_i$|$\sum y_i$|||$\sum x'_iy'_1$|

## Coeficiente de correlação de Pearson
O coeficiente de correlação de Pearson diz a intensidade da correlação de dois conjuntos de dados. Ela é construída para ter módulo máximo de $1$, de modo que
$$\rho = \frac{Cov(X,Y)}{S_xS_y}$$
Se convenciona a seguinte interpretação de seus valores:

|$\rho$|Intensidade da correlação|
|---|---|
|$[0.00, 0.19]$|Muito fraca|
|$[0.20, 0.39]$|Fraca|
|$[0.40, 0.69]$|Moderada|
|$[0.70, 0.89]$|Forte|
|$[0.90, 1.00]$|Muito forte|

No caso de valores negativos, se diz que é uma correlação negativa ou inversa ($x \propto -y$), com a mesma descrição das intensidades.