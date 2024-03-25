Observações do espectro eletromagnético são fundamentais para a astronomia em geral, dessa forma, a fotometria se faz essencial para mensurar e comparar medidas astronômicas.

Aqui usaremos como base a equação fundamental da ondulatória: $c=\lambda f$
## Ângulo sólido
O *ângulo sólido* é um ângulo bidimensional medido na superfície de uma esfera. O ângulo sólido numa esfera unitária equivale à uma área
$$\omega r^2 = A$$
de forma similar a de que um ângulo plano equivale a um comprimento num círculo unitário ($\theta r = c$). O ângulo sólido é representado por $\omega$ e é medido em esferorradianos. A medida de ângulo sólido vai de $0$ a $4 \pi$, cobrindo toda a área da esfera unitária. 

É possível relacionar um ângulo sólido $\omega$ com dois ângulos planos (assumindo um sistema de coordenadas esféricas) com a forma
$$\Delta\omega=sen \theta\,d\theta d\phi$$
## Grandezas da fotometria
### Intensidade específica
A *intensidade específica* é a medida de energia $E$ (por radiação) que é emitida numa unidade de tempo $t$, numa unidade de área $A$ da fonte emissora, numa unidade de ângulo sólido $\omega$:
$$I_\perp=\frac{dE}{dt\,dA\,d\omega}$$
> Veja que, pela notação, $A\perp r$.

Se quisermos saber a intensidade específica em um intervalo infinitesimal de frequência $f$, podemos computar a *intensidade específica monocromática*:
$$I_{\perp f}=\frac{dE}{dt\,dA\,d\omega\,df}$$
Podemos retirar a restrição de perpendicularidade multiplicando a expressão acima pelo cosseno do ângulo entre vetor normal de $A$ e $\vec r$. A imagem abaixo esquematiza a superfície $A$ sendo observada por um ângulo $\theta$.
![[Pasted image 20231126175101.png|300]]
A intensidade específica não varia com a distância, pois a energia diminui na mesma medida que o ângulo sólido, em relação a distância.

### Fluxo e luminosidade
O fluxo luminoso é definido como a quantidade de energia que é absorvida numa área por unidade de tempo e por intervalo de frequência:
$$dF_{\perp f}=\frac{dE}{dt\,dA\,df}=I_{\perp f}\,d\omega$$
O fluxo é medido em $Wm^{-2}$. O fluxo de um objeto em todo o espectro de frequências é:
$$F=\int_0^\infty F_fdf$$
> Lembrando que $F_f=\int I_{\perp f}cos\theta\,d\omega$

Como o fluxo não depende do ângulo sólido, ele diminui com uma lei de inverso de quadrado, com a distância.

O fluxo pode ser relacionado com a energia total emitida por um corpo a uma distância $r$, por meio da *luminosidade* intrínseca $L$:
$$F(r)=\frac{L}{4\pi r^2}$$
A luminosidade é medida em Watts e é a energia emitida por um corpo em todas as direções.

### Magnitude aparente
Usamos um sistema logarítmico (chamado de sistema de Hipparchus) para se referir ao fluxo de estrelas, onde, quanto menor a magnitude $m$, maior o fluxo detectado:
$$m=-2,5logF+C$$
Onde $C$ define o ponto zero da escala de magnitude, definido como a magnitude da estrela Vega, mas outros objetos de magnitude e fluxo conhecidos podem ser usados para comparação:
$$m_2-m_1=-2,5log\frac{F_2}{F_1}$$
### Magnitude absoluta
A magnitude absoluta não depende da distância, pois fixamos o fluxo para uma distância hipotética de $10pc$, de modo que
$$M=-2,5log\,F(10pc)+C$$
Com ela, temos uma medida de comprimento logarítmica que chamamos de módulo de distância $m-M$
$$m-M=5log\,r-5$$
