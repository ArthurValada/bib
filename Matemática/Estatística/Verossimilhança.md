A *função de verossimilhança* (ou likelihood) é responsável por determinar os parâmetros que melhor ajustam a [[Distribuições de probabilidade|FDP]] de um determinado modelo aos dados amostrais.

Os parâmetros são colocados no conjunto $\theta$. Por exemplo, o parâmetro para um modelo binomial é apenas $\theta=p$, a probabilidade de um único experimento; para um modelo uniforme os parâmetros são o começo e o final do intervalo $\theta=\{a,b\}$; para um modelo Gaussiano, $\theta=\{\mu,\sigma\}$.

*Exemplo:* Para um modelo binomial, a função de verossimilhança toma a forma
$$\mathcal L(\theta)=P(X=x_i|\theta)=\tbinom{n}{x_i}\theta^{x_i}(1-\theta)^{x_i}$$
Veja que a função permite estimar a probabilidade dos parâmetros de um modelo serem próximos da realidade a partir dos dados imputados ($n,x_i$). Dados observados diferentes geram funções de verossimilhança diferentes.

De forma esquemática, se temos uma FDP com parâmetros $\{\mu,\sigma\}$, podemos facilmente determinar a probabilidade de observar um valor específico. No entanto, se temos um conjunto de valores, usamos a likelihood para determinar os parâmetros $\{\mu,\sigma\}$.

## Princípio de máxima verossimilhança
Dizemos que o modelo distribuição estatística que melhor se aproxima da realidade é o modelo cujos parâmetros maximizam a função de verossimilhança. Assim, se define o *Valor de Verossimilhança Máxima* VVM:
$$\theta_{VM}=\max_\theta\mathcal L(\theta)$$
Ele pode ser encontrado resolvendo a equação
$$\left[\frac{\partial\mathcal L}{\partial\theta}\right]_{\theta_{VM}}=0 \tag{2.1}$$
Com a restrição de que
$$\left[\frac{\partial^2\mathcal L}{\partial\theta^2}\right]_{\theta_{VM}}>0 \tag{2.2}$$
Comummente, é útil se empregar a *verossimilhança logarítmica* para simplificar estas derivadas, uma vez que logaritmo é uma função monótoma, os máximos ficam no mesmo ponto.

*Exemplo:* pra uma distribuição gaussiana com amostras $n$ independentes (ou seja $P(a\cap b)=P(a)P(b)$), a função de Likelihood é:
$$\mathcal L(\mu,\sigma)=\cap_{i=0}^nP(X=x_i|\mu,\sigma)=\prod_{i=0}^n\frac{\exp\left(-\frac{1}{2}\left(\frac{x_i-\mu}{\sigma}\right)^2\right)}{\sqrt{2\pi}\sigma} \tag{2.3}$$
Onde $x$ é o conjunto de amostras e calculamos a probabilidade total do conjunto. Esta expressão pode ser reescrita como
$$\mathcal L = L_0\exp(-\chi^2/2) \tag{2.4}$$
Onde
$$\chi^2\equiv\sum_{i=0}^n\left(\frac{x_i-\mu}{\sigma}\right)^2\tag{2.5}$$
$$L_0\equiv\left(\frac{1}{\sqrt{2\pi}\sigma}\right)^n$$
Se quisermos calcular o valor de $\mu$ que maximiza a verossimilhança, podemos utilizar a log-likelihood:
$$\left[\frac{\partial\ln\mathcal L(\mu,\sigma)}{\partial\mu}\right]_{\mu_{VM}}=0$$
Resolvendo a expressão, vemos que
$$\mu_{VM}=\frac{1}{n}\sum_{i=0}^n x_i=\bar x \tag{2.6}$$
Ou seja, o parâmetro que maximiza a verossimilhança de um modelo normal num conjunto de amostras é a média amostral.

De modo semelhante, mas com algumas adaptações práticas, temos que
$$\sigma_{VM}^2=S^2=\frac{\sum_{i=0}^n(x_i-\mu_{MV})}{n-1} \tag{2.7}$$
## Cálculo de intervalos de confiança
Podemos considerar erros marginais se fizermos uma expansão de Taylor para o termo genérico da verossimilhança logarítmica no ponto de verossimilhança máxima:
$$\ln \mathcal L(\theta)=
\ln\mathcal L(\theta_{VM})
+\left[\frac{\partial\ln\mathcal L(\theta)}{\partial\theta}\right]_{\theta_{VM}}(\theta-\theta_{VM})
+\frac{1}{2}\left[\frac{\partial^2\ln\mathcal L(\theta)}{\partial\theta^2}\right]_{\theta_{VM}}(\theta-\theta_{VM})+\dots$$
Por construção, a derivada primeira da expressão é nula, de modo que a expressão abaixo é uma aproximação razoável de variações marginais de verossimilhança.
$$\mathcal L(\theta)\approx\mathcal L(\theta_{VM})\exp\left(-\frac{1}{2}\frac{(\theta-\theta_{VM})^2}{\Sigma_\theta^2}\right) \tag{3.1}$$
Onde
$$\frac{1}{\Sigma_{VM}^2}=\left[-\frac{\partial^2\ln\mathcal L(\theta)}{\partial\theta^2}\right]_{\theta_{MV}} \tag{3.2}$$
Considerando erros Gaussianos, podemos aplicar a equação $(2.3)$ e concluir que
$$\Sigma_{VM}^2=\sigma^2/N =S^2/N$$
O que chamamos de *incerteza*.

De modo geral reportamos um valor na forma.ll
$$\mu = \mu_{VM} \pm z\Sigma_{VM}$$
Onde $z$ é o *valor crítico* associado ao [[Intervalos de confiança gaussianos|nível de confiança]] desejado, ou seja, o $z$ associado a probabilidade $P(-z\le Z\le z)$ de que $\mu$ esteja no intervalo estimado.

Baseado nisso, podemos expressar o parâmetro de média gaussiano como
$$\mu=\bar x\pm z\sigma/\sqrt n$$

De modo geral, para estimar a Máxima Verossimilhança, basta:
1. Identificar a função de likelihood, partindo do modelo que mais se relaciona ao processo estudado e identificar os parâmetros de interesse $\theta$;
2. Estimar a verossimilhança máxima maximizando a função $\mathcal L$;
3. Calcular a incerteza associada nos parâmetros $\theta_{VM}$ computando o intervalo de confiança;
