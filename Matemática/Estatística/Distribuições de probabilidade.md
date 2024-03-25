Primeiramente tratamos das probabilidades discretas e depois aplicamos a continuação.

## Probabilidades discretas

O [[Probabilidade básica|espaço amostral]] pode ser mapeado numas **variável aleatória discreta (VAD)**: função que pega valores do espaço amostral e retorna um valor discreto (pode ser racional, desde que em passos discretos). Neste teto representamos VAs como $X$.

Já uma **função de densidade de probabilidade (FDP)** mapeia valores de uma VA para distribuições de probabilidade. A notação em geral é: a probabilidade do resultado do experimento ser $X=x$ é de $P(X=x)$. Dessa forma, pelos [[Probabilidade básica#Axiomas de Kolmogorov|axiomas de Kolmogorov]], $\sum_{i=0}^n P(X=x_i) = 1$

> Nota: este valor não é nulo, uma vez que probabilidades discretas não são valores infinitamente precisos como nas probabilidades contínuas.

Podemos somar várias densidades de probabilidade para obter uma **função de densidade acumulada (FDA)**. Uma FDA consiste no cálculo de todos os resultados possíveis tais que o valor de um dado resultado é $X\le x_i$ e denota-se $P(X \le x_i) = \sum_{j=0}^i P(X=x_j)$.

Com base nisso, o valor esperado de vários experimentos tende a um valor específico chamado **valor esperado**
$$E = \sum x_i P(X=x_i)$$

Além disso, de modo geral a **variância** $\sigma^2$ e o **desvio padrão** $\sigma$ são:
$$\sigma^2 = \sum(x_i-E)^2P(X=x_i),\;\sigma = \sqrt{\sigma^2} = \sqrt{\sum (x_i-E)^2P(X=x_i)}$$
Com base no mostrado, são determinados dois modelos estatísticos para facilitar o cálculo de certos problemas. Ambos assumem um experimento nos moldes do **ensaio de Bernoulli**, ou seja, são testes binários, ou há sucesso ou falha e queremos calcular a taxa de sucesso de $n$ experimentos independentes (amostras), com probabilidade constante $p$.

Em geral queremos descobrir qual a probabilidade de termos $x$ sucessos encontrando a FDP $P(X=x)$, ou, até $x$ sucessos, com a FDA $P(X\le x)$.

### Modelo binomial
$$P(X=x)=\tbinom{n}{x}p^x(1-p)^x=\frac{n!}{x!(n-x)!}p^x(1-p)^{n-x}$$
$$E=np,\;\sigma^2=np(1-p),\;\sigma=\sqrt{\sigma^2}=\sqrt{np(1-p)}$$
### Modelo hipergeométrico
Neste modelo temos dados de uma população $N$, na qual existe uma quantidade $A$ de sucessos, com base em conhecimentos posteriores e queremos saber qual a taxa de sucesso em $n$ experimentos específicos sem reposição.
$$P(X=x)=\frac{\tbinom{A}{x}\tbinom{N-A}{n-x}}{\tbinom{N}{n}}$$
$$E=\frac{nA}{N},\;\sigma=\sqrt{\frac{nA(N-A)}{N^2}}\sqrt{\frac{N-n}{N-1}}$$
### Modelo de Poissan
Diferente dos demais modelos, este descreve a probabilidade de encontrar um certo número de eventos independentes num intervalo fixo (de tempo ou espaço). Os eventos possuem uma taxa constante $\lambda$ de acontecimentos por unidade (de tempo ou espaço).

*Exemplo:* podemos descrever uma densidade de galáxias por esferoradiano de $\lambda = 1galáixa/sr$ ou uma quantidade de emissões de um objeto celeste como $\lambda=8fótons/s$.

A probabilidade de $x$ eventos acontecerem num intervalo $y$ (de tempo ou espaço) é
$$P(X=x)=\frac{(\lambda y)^x}{x!}e^{-\lambda y}$$
Veja que esta é uma função discreta em relação ao número de eventos $x$ e não uma função do intervalo $y$.

*Exemplo:* um detector de partículas mede prótons emitidos a uma taxa de $\lambda=4,5/s$. Qual a probabilidade de detectar 6 prótons num intervalo de 2 segundos?
$$P(X=6)=\frac{(4,5/s\times2s)^6}{6!}e^{4,5/s\times2s}=0,09$$
## Probabilidades contínuas
Os conceitos são similares a probabilidades discretas, porém aqui trabalhamos com **variáveis aleatórias contínuas (VAC)**. Assim, o terceiro axioma de Kolmogorov se escreve na forma $\int_{-\infty}^{+\infty}P(x)dx = 1$.

Como pelo axioma citado, a probabilidade de $P(X=x)$ é infinitesimal, tratamos apenas de probabilidades em intervalos específicos. Em um caso geral, se quisermos saber a chance de um experimento gerar resultados no intervalo $a\le X\le b$, dada a FDP $f(x)=P(X=x)$, escrevemos $P(a\le x\le b) =\int_a^b f(t) dt$.

A FDA seria usada se quisermos calcular a chance de $X\le x$ a FDA seria $F(x) = P(X\le x)=\int_{-\infty}^xf(t)dt$. Apesar de usarmos intervalos de infinitos, a função pode ser nula na maior parte do intervalo, assumindo valores não nulos apenas num trecho conhecido.

Além disso, pelo teorema fundamental do cálculo, $P(X>a)=1-F(a)$ e $P(a\le X\le b)=\int_a^bf(t)dt=F(b)-F(a)$

Baseado nisso, temos: $E = \int_{-\infty}^{\infty}xf(x)dx$ e $\sigma^2 = E(x^2) - [E]^2=\int_{-\infty}^{\infty}x^2f(x)dx-(\int_{-\infty}^{\infty}xf(x)dx)^2$

### Modelo uniforme
Todos os casos são equiprováveis, o que implica em FDP constante:
$$\begin{cases}
f(x) = \frac{1}{b-a}, && se\;a\le x \le x\\
f(x) = 0, && se\;a\ge x\le b
\end{cases}$$
$$E=\frac{a+b}{2},\,\sigma=\sqrt{\frac{(b-a)^2}{12}}$$
### Modelo normal ou Gaussiano
Distribuição mais comum na natureza de fenômenos estatísticos.
$$f(x)=\frac{\exp(-\frac12\left(\frac{x-\mu}{\sigma}\right)^2)}{\sqrt{2\pi}\sigma}$$
A integral desta FDP é impossível de se resolver analiticamente, portanto é feita uma padronização na forma
$$z=\frac{x-\mu}{\sigma}$$
Onde $\mu$ é a média populacional, $\sigma$ é o desvio padrão populacional e $z$ é a padronização ou [[Medidas de variação#Score Z|Score Z]] de um valor $x$. De modo que os valores de
$$F(z)=P(Z\le z)=\int_{-\infty}^z\frac{\exp(-t^2/2)}{\sqrt{2\pi}}dt$$
Podem ser obtidos na chamada Tabela Z, com valores comuns transcritos abaixo. Veja que $z$ está padronizado em unidades de desvio padrão

| $z=k\sigma$ | $P(Z\le z)$ |
| ---- | ---- |
| -4 | 0,00004 |
| -3 | 0,0013 |
| -2 | 0,0228 |
| -1 | 0,1587 |
| 0 | 0,5 |
| 1 | 0,8413 |
| 2 | 0,9772 |
| 3 | 0,9987 |
| 4 | 0,99997 |
*Exemplo:* se quisermos calcular, numa distribuição $X(100,20)\sim\mathcal N(\mu,\sigma)$ a probabilidade $P(X\le140)$, primeiro precisamos padronizar o limite:
$$z=\frac{x-\mu}{\sigma}=\frac{140-100}{20}=2$$
Pela tabela, $P(Z\le2)=0,9772$, portanto, $P(X\le140)=0,9772$.

*Exemplo:* Na mesma distribuição, se quisermos calcular a probabilidade de ter um resultado entre até 3 desvios padrões da média, queremos calcular $P(\mu-\sigma\times3\le X \le\mu+\sigma\times3)$. Esta expressão pode ser reescrita como
$$P(-3\le \frac{X-\mu}{\sigma}\le3)=P(-3\le Z\le3)$$
Pelo fato de que se trata de uma integração, pelo teorema fundamental do cálculo,
$$P(-3\le Z\le3)=F(3)-F(-3)$$
Como já padronizamos os valores, basta substituir usando a tabela Z:
$$P(-3\le Z\le3)=0,9987-0,0013=0,9974$$

De modo geral, a FDA é definida como
$$F(x)=P(X\le x)=\int_{-\infty}^x\frac{\exp(-\frac12\left(\frac{t-\mu}{\sigma}\right)^2)}{\sqrt{2\pi}\sigma}dt$$
No entanto, se define a chamada função de erro na forma
$$\text{erf}(x)=\int_{-x}^{x}\frac{\exp(-t^2)}{\sqrt{\pi}}dt=P(-\sqrt2x\sigma\le X-\mu\le \sqrt2x\sigma)=P(-\sqrt 2x \le Z\le\sqrt 2x)$$
Esta função tem seus valores tabelados e amplamente disponíveis, de modo que:
$$F(x)=\frac{1}{2}\left(1-\text{erf}\left(\frac{x}{\sqrt 2}\right)\right)$$

### Modelo Log-normal
As distribuições Log-normais são similares às normais, mas com uma cauda mais longa à direita, de modo que a mediana e a média são diferentes. Elas são úteis para modelar fenômenos biológicos, por exemplo, em que se há mais indivíduos acima da média que abaixo, mas os indivíduos que estão acima da média tem medidas bem maiores que num modelo normal.

A FDP possui uma distribuição na forma
$$f(x)=f_N(\ln x)/x=\frac{\exp(-\frac12\left(\frac{\ln x-\mu}{\sigma}\right)^2)}{x\sqrt{2\pi}\sigma}$$
Onde $f_N$ é uma FDP de distribuição normal. De modo similar, a FDA é
$$F(x)=F_N\left(\frac{\ln x-\mu}{\sigma}\right)=\frac{1}{2}\left(1-\text{erf}\left(\frac{\ln x-\mu}{\sqrt 2\sigma}\right)\right)$$
