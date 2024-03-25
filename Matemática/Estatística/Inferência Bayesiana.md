O teorema de Bayes na probabilística é bastante simples e útil. Ele permite inverter probabilidades no [[Probabilidade básica#Diagrama de árvore|diagrama de árvore]] de modo a responder perguntas como:

Se sabemos a probabilidade de $A$ e de $B$, e sabemos a probabilidade de $B$ dado que $A$ aconteceu $P(B|A)$, como podemos inverter a relação para descobrir a probabilidade de $A$ dado que $B$ aconteceu $P(A|B)$? Basta usar o teorema de Bayes:
$$P(A|B)=\frac{P(B|A)P(A)}{P(B)}$$
No entanto, se aplicarmos conceitos de inferência por [[Verossimilhança]], este teorema passa a ser muito importante. Se definirmos o evento $A$ como os parâmetros de uma distribuição, $\theta$ e o evento $B$ como novos dados observados, $d$, temos
$$P(\theta|d)=\frac{P(d|\theta)P(\theta)}{P(d)}$$
Do lado esquerdo temos $P(\theta|d)$, que é chamado de *posterior*, que é a estimativa de $\theta$ atualizada de acordo com os dados $d$.

Do lado direito, podemos estimar $P(d|\theta)=\mathcal L(\theta)$. $P(\theta)$ é chamado de probabilidade *prior* ou *a priori*, que é uma estimativa da probabilidade do parâmetro $\theta$ antes de se analisar os dados.  Por fim, $P(d)$ é chamada de *evidência* ou *verossimilhança marginal* e serve para normalizar a *posterior*.

> O teorema de Bayes é usado para atualizar os conhecimentos obtidos *a priori* sobre um parâmetro, com base em nova *evidência* e sua *verossimilhança*, para um conhecimento *posterior*.

A diferença entre a verossimilhança e a posterior podem ser observadas neste *exemplo:* Queremos saber o parâmetro sexo biológico ($\theta$) de um indivíduo macho ($M$) ou fêmea ($F$) e para isso conduzimos um teste de gravidez, que pode ter como resultado os dados $d=G$ ou $d=\bar G$. Digamos que o resultado resultado foi $S$.

A verossimilhança $\mathcal L(\theta=F)=P(d=S|\theta=F)=0,03$, pois a probabilidade de estar grávido sabendo que é fêmea é de 3%. No entanto, queremos saber a probabilidade de ser fêmea, posterior ao dado de que o indivíduo está grávido: $P(\theta=F|d=S)=1$, pois por definição, apenas fêmeas ficam grávidas.
## Considerações sobre os priors
Pela forma que a teoria Bayesiana é estruturada, é possível incorporar dados conhecidos a priori de modo a ir atualizando o conhecimento sobre dado parâmetro, ao contrário da inferência frequentista, que não permite considerar probabilidades além dos dados em si.

A forma de incorporar valores na probabilidade posterior é por meio da escolha adequada de priors. Existe muita discussão sobre a escolha de priors, principalmente porque a escolha deles pode enviesar resultados imediatos. No entanto, com medições o suficiente, é mostrado que os posteriores convergem independente da escolha dos priors iniciais.

Os priors iniciais podem ser escolhidos para agregar informações teóricas e práticas sobre os dados, como por exemplo o fato de que dados como o temperatura e massa são sempre positivos. Para incorporar este tipo de informação construímos um prior plano:
$$P(\theta)=
\begin{cases}
1/(\theta_{max}-\theta_{min}),&\theta_{min}\le\theta\le\theta_{max}\\
0, &\theta_{min}\not\le\theta\not\le\theta_{max}
\end{cases}$$
Aplicando este prior temos
$$P(\theta|d)\propto P(d|\theta)=\mathcal L(\theta)\implies P(\theta|d)=
\begin{cases}
\frac{\mathcal L(\theta)}{(\theta_{max}-\theta_{min})},&\theta_{min}\le\theta\le\theta_{max}\\
0, &\theta_{min}\not\le\theta\not\le\theta_{max}
\end{cases}$$
De modo que a distribuição fica com o mesmo formato.

O uso de priors uniformes pode causar concentrações dos dados ao redor de um valor $\sqrt{D/3}$, onde $D$ é a dimensionalidade dos dados. Em geral, para maiores dimensões se observa uma concentração maior.

É sempre importante fazer uma análise sensível da escolha de priors e pesquisar na literatura sempre que novos problemas aparecerem, de modo a não reinventar a roda.

Alguns exemplos de tipos de priors são:
- Priors de referência: escolhidos para ter máxima entropia, de forma que a contribuição dos dados para o posterior seja maximizada. Para uma distribuição Gaussiana, o prior adequado para $\mu$ é plano em $\mu$ e para $\sigma$ o prior deve ser plano em $\log \sigma$;
- Priors de ignorância: em 1812 Laplace criou o princípio de que se nada se sabe sobre a distribuição, o prior deve ser escolhido de modo a dar probabilidades iguais em todos os parâmetros. Em casos simples, estes priors podem ser escolhidos usando de simetrias;
- Priors conjugados: são priors que fazem com que a família de distribuições da verossimilhança seja similar a do posterior. Uma distribuição gaussiana é auto-conjugado, ou seja, com uma verossimilhança e um prior gaussianos, sempre se obtém um prior gaussiano;

