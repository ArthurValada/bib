Quando se determina um valor médio amostral de forma experimental, é necessário atribuir um intervalo de confiança com um determinado nível de confiança. Um *nível de confiança* é uma porcentagem de vezes em que se espera que a medição esteja correta, também chamado de intervalo de probabilidade. Definimos o *nível de significância* como $\alpha=1-\text{nível de confiança}$.

*Exemplo:* Para um nível de confiança de 95%, se espera que o valor da média populacional esteja dentro da média amostral 95% das vezes.

## Erros com distribuição Gaussiana
Se estimarmos que os erros estejam numa [[Distribuições de probabilidade#Modelo normal ou Gaussiano|distribuição gaussiana]], podemos atribuir um valor para z que se correlacione com o nível de confiança, na forma
$$1-\alpha=P(-z\le Z\le z)$$
O valor z também é chamado de nível sigma, como mostra a tabela:

| $z$ | Nível sigma | Confiança: $P(-z\le Z\le z)$ | Significância: $\alpha$ |
| ---- | ---- | ---- | ---- |
| 1 | $1\sigma$ | 0,6827 | 0,3173 |
| 2 | $2\sigma$ | 0,9545 | 0,0455 |
| 3 | $3\sigma$ | 0,9973 | 0,0027 |
| 4 | $4\sigma$ | 0,99993 | 0,00007 |
| 5 | $5\sigma$ | 1-5,7e-7 | 5,7e-7 |
Veja que, ao contrário da tabela Z, aqui só listamos valores positivos, mas que se referem a $\pm z$. Vale lembrar que $P(-z\le Z\le z)=\text{erf}(z/\sqrt 2)$.

O nível de confiança muda o tamanho do intervalo de confiança por meio do *valor crítico* $z$. Ele pode ser calculado de 3 formas:
- Usando o intervalo de confiança, usando fórmula $P(-z\le Z\le z)=F(z)-F(-z)$;
- A partir da significância, invertendo a FDA para calcular $z_{\alpha/2}=F^{-1}(\alpha/2)$;
- É menos comum, mas também é possível utilizar a relação $\sqrt 2 \text{erf}^{-1}(1-\alpha)=z$;

Como usar a significância envolve uma consulta a menos na tabela z, e não é comum ter acesso a $\text{erf}^{-1}(p)$, $z_{\alpha/2}$ é o método mais usado.

Usando da [[Verossimilhança]] é possível determinar que para erros gaussianos, a melhor estimativa da média populacional $\mu$ é a média amostral $\bar x$. Além disso, é mostrado que o desvio padrão para estimar erros na estimativa da média têm a forma $z\sigma/\sqrt n$.

Juntando todos estes fatores temos a expressão para o intervalo de confiança:
$$\mu=\bar x\pm z_{\alpha/2}\sigma/\sqrt{n}$$
Ou
$$\mu=\bar x\pm\text{erf}^{-1}(1-\alpha)\sigma\sqrt{\frac{2}{n}}$$
## Erros com distribuição t de Student
A distribuição t é feita para considerar o fato de que a distribuição gaussiana só é acurada quando o número de amostras $n\to\infty$. Assim, ao invés de $z$, temos um valor $t_{n-1}$ que pode ser consultado na tabela t e leva em conta o número de graus de liberdade $n-1$.

É estabelecido que a imprecisão da distribuição gaussiana é considerável para $n<30$. Quando se têm menos de 30 amostras, é necessário utilizar erros com a distribuição t, que possui caldas mais largas, aumentando o intervalo de confiança.

Usando ela, é possível corrigir os intervalos de confiança gaussianos para a forma
$$\mu=\bar x\pm t_{\frac{\alpha}{2},n-1}\sigma/\sqrt{n}$$