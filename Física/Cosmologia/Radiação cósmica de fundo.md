A [[Fundamentos da cosmologia#O universo é cheio de radiação cósmica de fundo|radiação cósmica de fundo]] (CMB) é uma fonte de radiação eletromagnética quase [[Fundamentos da cosmologia#Em largas escalas o universo é isotrópico e homogêneo|isotrópica]], com um espectro de corpo negro de pico em $\uplambda=2mm$ ($2,725K$).

Partindo da densidade de energia $\epsilon_{\gamma0}=0,621MeVm^{-3}$ e da energia média de cada fóton, é possível estimar a densidade numérica de fótons como
$$n_{\gamma0}=4,11\times10^{8}m^{-3}\tag{1.1}$$
Partindo da nossa melhor estimativa do [[Medidas do parâmetro de densidade#Densidade de objetos visíveis|parâmetro densidade energética de matéria bariônica]], $\Omega_{bar0}=0,04$ e assumindo que que a contribuição dessa energia é principalmente da massa de prótons e neutrons ($E\approx939MeV$), temos uma densidade numérica de bárions de
$$n_{bar0}=0,22m^{-3}\tag{1.2}$$
Assim, a razão bárion-fóton do universo é de:
$$\eta=\frac{n_{bar0}}{n_{\gamma0}}=5\times10^{-10} \tag{1.3}$$
## Observações do CMB
O primeiro mapa abrangente de todo o CMB foi feito pela sonda espacial COBE (1989), que teve 3 importantes resultados:
1. A radiação cósmica de fundo se comporta de forma muito aproximada a um espectro de corpo negro. Tão aproximada que os sensores da COBE não detectaram desvios;
2. O mapa gerado pela COBE possuía uma distorção de dipolo no seu espectro, ou seja, uma região tinha o espectro de corpo negro desviadas para o azul e na região diametralmente oposta, se tinha um desvio para o vermelho. Esta distorção pôde ser eliminada se considerar o efeito doppler relativo ao movimento:
	- Da sonda em relação à terra,
	- Da terra em relação ao sol,
	- Do sol em relação a via láctea,
	- Da via láctea em relação ao grupo local,
	- Do grupo local em relação ao aglomerado Virgo,
	- Do aglomerado de Virgo em relação ao superaglomerado Hydra-Centauro
	Desconsiderando todas estas velocidades, o CMB se torna isotrópico;
3. Desconsiderando distorções de dipolo, as flutuações de temperatura do CMB são pequenas em amplitude. A raiz da flutuação quadrada média de temperatura medida pelo COBE foi de $1,1\times10^{-5}$ (desconsiderando regiões com ruído como as emissões da Via Láctea). Em outras palavras, a radiação do CMB varia apenas $30\mu K$, o que é muito próximo de isotropia;
Isto tudo mostra que a radiação cósmica de fundo está muito próxima de uma emissão de corpo negro isotrópica, o que suporta muito a hipótese do Big Bang.
## Formação do CMB
Houveram 3 épocas importantes durante a formação da radiação cósmica de fundo, muito próximas, mas ainda assim distintas:
1. Recombinação: é o momento em que a matéria bariônica (com núcleos já formados) deixa de ser iônica e passa a ser neutra. Como isso foi um processo gradual, o instante de recombinação é definido como o momento em que metade da quantidade de núcleos bariônicos se tornaram neutros;
2. Desacoplamento dos fótons: o momento em que a taxa de scattering (epalamento de Thomson) de fótons se torna menor que o parâmetro de Hubble (a taxa de expansão do universo), quando isso acontece os fótons param de interagir com elétrons e o universo se torna transparente;
3. Último scattering: o instante médio de emissão do CMB;
Veja que apesar de relacionados, são fenômenos diferentes.

> No universo primordial, logo após a nucleossíntese, a matéria bariónica e radiação estavam fortemente acopladas. Elétrons livres possuem uma cross-section maior, o que aumenta a taxa de scattering devido ao espalhamento de Thomson, um caso específico do efeito Compton (interação elétron-fóton). Dessa forma, fótons, elétrons e, devido a interações elétricas, núcleos, se comportam como um único fluido fóton-bárion (F-B).

Com a expansão do universo primordial, a temperatura da radiação de fundo diminui ao ponto em que a *recombinação* se intensifica (tecnicamente a primeira combinação).

A recombinação diminui a quantidade de elétrons livres, o que reduz a taxa de scattering, ao mesmo tempo que a constante de Hubble sempre está crescendo. Ambos fatores combinados, há o instante de *desacoplamento*. Com o intensificar do desacoplamento, momentos depois ocorre o *último scattering*.
### Recombinação
O instante de recombinação é definido como o instante em que a ionização parcial definida abaixo seja $X=0,5$. Aqui assumimos um universo primordial apenas com hidrogênio ionizado, pois a presença de hélio serve apenas como uma mera contaminação que mudaria pouco os valores reais.
$$X\equiv\frac{n_p}{n_p+n_H}=\frac{n_p}{n_{bar}}=\frac{n_e}{n_{bar}} \tag{3.1}$$
Recombinações individuais ocorriam a qualquer momento desde a nucleossíntese, no entanto, a maioria dos fótons possuía energia suficiente para fotoionizar qualquer átomo que formasse.

Para que isso não ocorresse, a energia da radiação de fundo precisava ser menor que a energia de ionização do hidrogênio $Q=13,6eV$, o que significa uma temperatura de recombinação de $T=60000K$.

No entanto, como a radiação cósmica de fundo segue um espectro de corpo negro, apesar da energia média ser inferior à estimada, a quantidade de fótons acima desta energia ainda seria grande o suficiente para reionizar a maior parte dos átomos. Isto porque, mesmo que fótons de alta energia sejam uma fração muito pequena da radiação de fundo, existem muitos fótons para cada bárion (lembrando: $\eta=5\times10^{-10}$).

Considerando o espectro de corpo negro em função do parâmetro de Hubble e a densidade numérica de fótons, é possível estimar que a taxa de ionização parcial. Desse modo temos alguns resultados: a temperatura de recombinação da radiação cósmica de fundo é de $3740K$, pouco acima da temperatura de fusão do Tungstênio.

A radiação de fundo atingiu esta temperatura em $z_{rec}=1370$, o que, no modelo padrão é $t_{rec}=240.000yr$. Vale lembrar que não foi um processo instantâneo: a ionização parcial foi de $X=0,9$ a $X=0,1$ em aproximadamente $70.000yr$.
### Scattering
Considerando elétrons livres com uma cross-section de Thomson de $\sigma_e=6,65\times10^{-29}m^2$, a taxa de scattering de Thomson é de
$$\Gamma=n_e\sigma_ec$$
Corrigindo para conservação de energia temos
$$\Gamma=\frac{n_e\sigma_ec}{a^3}=n_e\sigma_ec(1+z)^3$$
Podemos determinar $\Gamma(z)$ utilizando ($1.2$) e ($3.1$).
$$\Gamma(z)=n_e(z)\sigma_ec(1+z)^3=X(z)n_{bar}(1+z)^3\sigma_ec=4,4\times10^{-21}s^{-1}X(z)(z+1) \tag{3.2}$$
Além disso, neste período o universo já era dominado pela matéria, de modo que o parâmetro de Hubble pode ser obtido por um [[Modelos cosmológicos#Universos de único componente|modelo cosmológico apenas com matéria]]:
$$\frac{H^2}{H_0^2}=\frac{\Omega_{m0}}{a^3}=\Omega_{m0}(1+z)^3$$
Usando $\Omega_{m0}=0,3$:
$$H(z)=1,24\times10^{-28}s^{-1}(1+z)^{3/2}\tag{3.3}$$
Assim, o desacoplamento ocorre quando:
$$\begin{align}
\Gamma(z_{dec})&=H(z_{dec})\\
1+z_{dec}&=\frac{43}{X(z_{dec})^{2/3}}\\
z_{dec}&\approx1100
\end{align}$$
A partir da equação $(3.2)$ também é possível determinar o instante de último scattering, que é bem próximo do instante de desacoplamento. Usando o modelo padrão, o redshift $z_{dec}=z_{us}=1100$ é equivalente a $350.000yr$.

| Evento | Redshift | Temperatura (k) | Idade do universo (anos) |
| ------ | -------- | --------------- | ---------------------------- |
| Igualdade matéria-radiação       | 3570         | 9730                | 47.000                             |
| Recombinação       | 1370         | 3740                | 240.000                             |
| Desacoplamento       | 1100         | 3000                | 350.000                             |
| Último scattering       | 1100         | 3000                | 350.000                             |
## Flutuações no CMB
As primeiras medições do CMB já tinham como um dos objetivos determinar um mapa e padrões de anisotropia (daí o nome Wilkson Microwave Anisotropy Probe) em diversas escalas angulares do céu.
![[Pasted image 20240131124055.png]]
 O gráfico de correlação de anisotropia (em flutuações de temperatura) em relação à escala angular tem um pico no ângulo de aproximadamente 1°, o que sugere a existência de estruturas com diâmetro angular de 1°.

Para determinar o tamanho real destas estruturas podemos relacionar um tamanho real $\ell$ com um tamanho angular $\delta\theta$ usando a [[Medidas de parâmetros cosmológicos#Réguas padrão|distância angular]] $d_A$ até a superfície de último scattering.
$$d_A=\frac{\ell}{\delta\theta}$$
No limite para altos redshifts temos que
$$d_A\approx\frac{d_{hor}(t_0)}{z_{us}}=\frac{14.000Mpc}{1100}=13Mpc$$
Assim
$$\ell=d_A(\delta\theta)=13Mpc\left(\frac{\delta\theta}{1rad}\right)=0,22Mpc\left(\frac{\delta\theta}{1°}\right)$$
A distância de Hubble para $z=1100$, usando a eq. $(3.3)$ é  de $c/H(1100)\approx0,2Mpc$. Ou seja, flutuações de 1° no CMB equivalem à distância de Hubble: $\theta_H\approx1°$.

A origem dessas deformações pode ser explicada em [[Formação de estruturas|flutuações de densidade]] de energia. A densidade de energia pode ser modelada como um campo escalar $\epsilon(\vec r)$ onde existem variações na densidade média
$$\epsilon(\vec r)=\bar\epsilon+\delta\epsilon(\vec r) \tag{4.1}$$
Estas variações de densidade geram variações no campo potencial gravitacional, pela equação de Poisson:
$$\nabla^2(\delta\Phi)=\frac{4\pi G}{3}\delta\epsilon \tag{4.2}$$
Devido ao redshift gravitacional, as variações de potencial gravitacional no momento do desacoplamento são diretamente relacionadas à variações de temperatura no CMB. Esta relação é descrita pelo efeito Sachs-Wolfe:
$$\frac{\delta T}{T}=\frac{1}{3}\frac{\delta\Phi}{c^2} \tag{4.3}$$
Isto permite explicar flutuações de temperatura com escalas maiores que a distância de Hubble ($\theta>\theta_H\approx1°$). Elas ocorreram pela inomogeneidade da própria matéria escura. Isto porque os movimentos do fluido fóton-bárion são irrelevantes para escalas maiores que a distância de Hubble, já que o parâmetro da equação de estado do fluido está no intervalo $0<w<1/3$, de modo que a [[Dinâmica cosmológica#Equação de estado|velocidade do som (5.2)]] é menor que a velocidade da luz.

Como a flutuação aleatória da matéria escura é mais difícil de prever em comparação à outra causa das flutuações, as flutuações em escalas $\theta>\theta_H\approx1°$ possuem desvio padrão maior e são menores em amplitude.

### Baryon Acoustic Oscillation (BAO)
Para escalas $\theta<\theta_H\approx1°$ o movimento do fluido fóton-bárion começa a ser relevante. Momentos antes da recombinação, a matéria escura pode se aglomerar gravitacionalmente, pois ela não interagia com o fluido fóton-bárion.

As flutuações de matéria escura geraram potenciais gravitacionais $(4.1)$ que causaram o colapso de bolhas no fluido F-B. Ao colapsar nos centros das aglomerações de matéria escura, a densidade aumentou nestes pontos, de modo que, pela [[Dinâmica cosmológica#Equação de estado|equação de estado (5.1)]], a pressão aumentou, fazendo que as bolhas se expandissem. Vale lembrar que a matéria escura não interage com esta pressão.

Com a expansão da bolhas, a densidade e a pressão diminuíram, fazendo as bolhas colapsarem novamente. Este ciclo se repetiu várias vezes e se chama *Oscilação Acústica Bariônica* (BAO).

Assim, os diferentes multipolos observados no gráfico de isotropia acima representam diversos modos de vibração das bolhas de BAO no instante de desacoplamento. As maiores correlações no gráfico representam modos de vibração mais comuns.

O fato de o maior pico ser associado a 1° significa que as bolhas que este era o modo de vibração mais comuns das oscilações no instante de desacoplamento. Determinar o tamanho esperado dos diferentes modos de vibração é um processo um complicado. Mas em geral é esperado que a correlação mais comum seja para bolhas do tamanho da distância de Hubble (o limite de correlação causal) que, como calculamos, têm tamanho angular de aproximadamente 1°.

O fato de que o valor calculado e o mensurado serem tão próximos indica que a [[Métricas e curvaturas|curvatura]] do nosso universo é de $k=0$, uma vez que não há distorção causada por curvaturas entre o valor próprio (estimado) das bolhas e o valor angular medido.

Além disso, os diversos modos de vibração também permitem estimar a proporção entre fótons e bárions no fluido F-B, pois esta proporção pode ser estimada pela velocidade do som $c_s=\sqrt w_{FB}c$.

Variando estes parâmetros é possível encontrar modelos que melhor se ajustam nos dados experimentais de anisotropia mostrados acima. Como pode-se ver, o modelo encontrado se ajusta quase perfeitamente com os dados de anisotropia obtidos. Este modelo nos gera os parâmetros de densidade abaixo. Por completude, também inserimos o valor da constante de Hubble, determinado em [[Medidas de parâmetros cosmológicos]].

| Parâmetro           | Valor                |
| ------------------- | -------------------- |
| $\Omega_{k0}$       | $0$                  |
| $\Omega_{m0}$       | $0,3$                |
| $\Omega_{r0}$       | $8,4\times10^{-5}$   |
| $\Omega_{\Lambda0}$ | $0,7$                |
| $H_0$               | $74,0\pm1,4km/s/Mpc$ |
