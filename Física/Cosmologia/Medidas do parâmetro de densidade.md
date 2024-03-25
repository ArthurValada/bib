Determinando o valor do parâmetro de desaceleração $q_0=-0,55$ nos permite definir uma das variáveis da equação $(1.1)$ de [[Medidas de parâmetros cosmológicos]]
$$q_0 = \Omega_{r0}+\frac{1}{2}\Omega_{m0} - \Omega_{\Lambda0} \tag{1.1}$$
Precisamos então estimar os demais parâmetros de densidade.
## Parâmetro de densidade de radiação
O parâmetro de densidade de radiação felizmente é fácil de estimar, basta considerar que a radiação que compõem a densidade de radiação são apenas os fótons da [[Fundamentos da cosmologia#O universo é cheio de radiação cósmica de fundo|Radiação Cósmica de Fundo]]. Eles podem ter baixa energia, mas possuem uma densidade muito maior que os fótons emitidos por galáxias, de modo que os fótons emitidos após o Big Bang contribuem com cerca de 3% da energia do parâmetro de densidade.

No entanto, a densidade de energia de radiação também recebe contribuição da Radiação Cósmica de Fundo de Neutrinos (Cosmic Neutrino Background, CNB). Infelizmente, até o momento da escrita deste texto, não existem evidências de detecção de neutrinos do CNB, de modo que apenas podemos estimar sua densidade numérica a partir do CMB.

Se especula que os neutrinos do CNB são relativísticos, ou seja, sua energia é muito maior que sua massa inercial. Em algum momento na história do universo os neutrinos deixarão de ser relativísticos e sua contribuição ao parâmetro de densidade de radiação será diferente. Baseando-se nessa especulação, estimamos que, para cada sabor de neutrino:
$$\epsilon=\frac{7}{8}\left(\frac{4}{11}\right)^{4/3}\epsilon_{CMB}$$
De modo que
$$\Omega_{CNB}=0,681\Omega_CMB$$
Em conclusão:
$$\Omega_{r0}=\Omega_{CMB}+\Omega_{CNB}=8,4\times10^{-5}$$
O que a pesar de ser um valor especulativo, mais superestima do que subestima o valor desse parâmetro. I.e., se os neutrinos não forem mais relativísticos, então a densidade de radiação seria ainda menor e mais desprezível.

## Parâmetro de densidade de matéria
Assim, na equação $(1.1)$ ou mesmo na [[Modelos cosmológicos|equação de Friedmann]] $(1)$, nos resta determinar o valor de mais uma variável, para completar nosso modelo cosmológico. Como não sabemos a natureza da constante cosmológica, precisamos então medir a densidade de matéria no universo.
### Densidade de objetos visíveis
Em distâncias astronômicas, a matéria só é visível quando é luminosa, sendo a luminosidade a principal propriedade observável de um objeto astronômico. Estrelas são os principais objetos luminosos no universo, em massa. Para estimar a densidade de massa de estrelas no universo, precisamos determinar a densidade luminosa média de um grande volume do universo (uma esfera com raio de centenas de Mpcs) e estimar a razão massa-luz, o que é menos trivial, uma vez que consiste em descobrir a massa e luminosidade intrínseca de muitas estrelas, ambas medições não triviais.

Baseado nos nossos melhores dados, temos uma densidade de massa estelar de
$$\rho_{\star0}=\left<M/L_B\right>j_{\star B}=5\times10^8M_\odot Mpc^{-3}$$
Onde $j_{\star B}$ é a densidade luminosa do universo em algumas centenas de Mpc, na banda B e $L_B$, a luminosidade estelar na banda B.

Estes dados nos geram um parâmetro de densidade de
$$\Omega_{\star0}=0,0004$$
No entanto, usar a razão massa-luz nos dá um parâmetro de densidade de massa do universo muito impreciso, pois desconsidera diversos objetos escuros mas massivos, como nuvens de gás, planetas, buracos negros e estrelas menos luminosas.

Em galáxias espirais com a Via Láctea e M31, o gás representa 10% da massa total da galáxia e em galáxias irregulares esse número é ainda maior. Já em aglomerados de galáxias como o Coma, a massa de gás intergaláctico é 6 a 7 vezes maior que a massa de estrelas do aglomerado.

A massa de gás pode ser estimada por emissões de corpo negro do gás no espectro de raio x, por razões que serão explicadas a diante.

Estudos indicam que o parâmetro de densidade de matéria bariônica no universo é aproximadamente
$$\Omega_{bar0}=0,04\pm0,01$$
Que é duas ordens de grandeza maior que a densidade de estrelas. No entanto, como será mostrado adiante, a densidade de massa que observamos em galáxias e aglomerados gera um parâmetro bem maior que esse.
### Densidade de objetos não visíveis
Além da relação massa-luz, é possível utilizar de interações gravitacionais para modelar a distribuição de massa em estruturas como galáxias e aglomerados.
#### Curvas de rotação de galáxias
Para uma galáxia, a velocidade orbital das estrelas é muito pequena, de modo que podemos considerar suas órbitas circulares, de modo que a velocidade orbital é
$$v=\sqrt\frac{GM(R)}{R} \tag{3.1}$$
Onde $M(R)$ é a distribuição radial de massa de uma galáxia. Esta equação considera distribuições esfericamente simétricas de massa. As correções para um formato mais realista de massa apenas acrescentam um pequeno fator de correção.

Para mensurar a velocidade orbital de um objeto é necessário saber a velocidade de recessão $v=cz$ do corpo principal (galáxia) e subtraí-la da velocidade de recessão do objeto em si.

Tipicamente, para uma galáxia espiral, o brilho superficial de uma galáxia decai exponencialmente com a distância do centro.
$$I(R)=I(0)e^{-R/R_s}$$
Onde $R_s$ é uma constante de normalização proporcional ao tamanho da galáxia. Para a nossa galáxia, $R_s\approx4 kpc$. Assumindo que as estrelas são de uma mesma população e por isso terão uma razão $\left<M/L_B\right>$ uniforme por toda galáxia, é possível usar a distribuição de brilho superficial para estimar a distribuição radial de massa luminosa na galáxia $M_\star(R)$.

Usando parâmetros experimentais de curva de redshift de galáxias, é possível determinar a curva de rotação $v(R)$ e a partir disso modelar $M_e(R)$. O astrônomo Vesto Slipher foi o primeiro a tentar determinar a curva de rotação da galáxia M31, em 1914, determinando que $v(R)$ cresce linearmente até $R=6kpc=R_s$. Por limitações dos equipamentos, ele só conseguiu realizar medições até $3R_s$.

Com equipamentos melhores, Vera Rubin e Kent Ford conseguiram, em 1970, determinar a curva de rotação de estrelas na M31 até $4R_s$. Em 1975 Roberts e Whitehurst usaram medições de radio para determinar distâncias até $5R_s$.

Como resultado dos diversos estudos foi mostrado que a curva de rotação de uma galáxia espiral tende a se comportar da seguinte forma: crescimento linear até $R_s$ e depois disso, velocidades constantes ou com leve crescimento (como no caso de nossa galáxia).

Este padrão de curva de velocidade difere do comportamento esperado pela curva de luminosidade (decaimento exponencial). Na verdade, ele sugere a existência de grandes quantidades de massa numa distância maior que o raio visível da galáxia, servindo de âncora para as estrelas numa órbita mais rápida não escaparem da galáxia.

Para a nossa galáxia, temos que $R_s\approx4 kpc$ e o raio do halo de *matéria escura* é de $R_{halo}\approx300kpc$ (metade da distância até M31), de modo que a massa da galáxia, considerando essa matéria escura invisível, é de 10 a 40 vezes mais massa que a massa estimada para as estrelas. Se nossa galáxia é típica nesse aspecto, podemos esperar um parâmetro de densidade de até
$$\Omega_{gal0}=0,16$$
#### Distribuições de massa em aglomerados de galáxias
Em aglomerados de galáxias também existe a presença de matéria escura e gás intergaláctico. Podemos estimar a massa destes usando o [[TeoremaDoVirial.pdf|Teorema do Virial]] estático:
$$0=E_g+2K$$
Que pode ser resolvido de modo que a massa total do aglomerado é
$$M=\frac{\left<v^2\right>r_h}{\alpha G}$$
Onde $\left<v^2\right>$ é a velocidade quadrada média das galáxias e $r_h$ e $\alpha$ parâmetros relativos ao formato do aglomerado, o primeiro sendo o raio de meia massa do aglomerado, que não é trivial de se estimar. No entanto, se assumirmos uma distribuição de massa esféria e similar a distribuição de matéria visível, é possível fazer aproximações.

Também é possível estimar massas num aglomerado usando a distribuição de temperatura do gás intergaláctico. Devido a concentrações de massa, a pressão gravitacional faz com que o gás esquente (emitindo até raios-x).

Um método mais recente é usar as distorções da [[Radiação cósmica de fundo]] causadas pelo efeito Compton para fótons do CMB passando por nuvens de gás ionizado. Com isso é possível determinar distribuições numéricas e consequentemente, de massa, do gás.

Usando os métodos citados de determinação de massa de aglomerados, temos que a contribuição para o parâmetro de densidade da massa de aglomerados é
$$\Omega_{agl0}\approx0,2$$
Isto provê um limite inferior em $\Omega_{m0}$, pois não considera distribuições de matéria fora dos aglomerados.
#### Teorias de matéria escura
*Matéria escura* não é uma teoria: é um conjunto de observações (incluindo as listadas acima) que mostram discrepância entre a quantidade de massa observável e a massa não observável em diversas escalas astronômicas.

Além disso, pelo fato de essa massa extra não observer nem emitir radiação, é determinado que elas não interagem fortemente com o espectro eletromagnético. Junto a isso, pelo seu comportamento e distribuição se deduz que a matéria escura também não é colisional, pois não há mecanismos de liberação de energia de modo que esta matéria tenha suas órbitas diminuídas.

Em suma, o que for a matéria escura precisa ter as propriedades:
- Possuir massa;
- Não colidir;
- Não interagir no espectro eletromagnético;

No entanto, existem diversas teorias que tentam explicar o que compõe estas massas. Uma teoria era a presença de MACHOs: MAssive Compact Halo Objects, i.e. objetos bariônicos como buracos negros e anãs marrons (objetos não diretamente visíveis) presentes no halo galáctico poderiam compor a massa necessária para a matéria escura.

Devido a sua compacidade estes objetos não colidem (tecnicamente estrelas também não são colisionais numa escala galáctica) e não absorvem radiação de forma perceptível. Além disso, devido a baixas temperaturas, estes objetos não emitem muita radiação.

Buscas por observações de micro lentes gravitacionais consequentes da passagem de MACHOs por objetos distantes foram feitas. Estes eventos foram tão raros ao ponto de poder estimar que os MACHOs não contribuem de forma significativa para a massa da matéria escura.

A teoria (ou conjunto de teorias) mais prevalente na astrofísica atual é a de WIMPs: Weakly Interacting Massive Particles - Nota sobre o nome: WIMPs foram propostas antes dos MACHOs. Neste conjunto de teorias a matéria escura é uma partícula que forma um gás que não interaja no espectro eletromagnético nem entre si.

Nesse sentindo, existem várias propostas de WIMPs, por exemplo, neutrinos do CNB se assumirmos que eles já não são mais relativísticos. Porém, mesmo para as maiores estimativas de massa de neutrinos, usando a densidade numérica de neutrinos derivada do CMB, ainda teríamos um parâmetro de massa de $\Omega_\nu=10^{-3}$.

Em teorias de WIMPs a física de partículas se torna muito importante, com várias partículas teóricas que poderiam suprir o papel da matéria escura. Até o momento, não tivemos nenhum resultado para resolver o problema da matéria escura.
## Constante cosmológica
Não sabemos o que causa ela. Nossa melhor estimativa de $\Omega_{\Lambda0}$ parte da nossa melhor estimativa de que $\Omega_{m0}\approx0,3$ (estimada a partir do [[Radiação cósmica de fundo|CMB]]), de modo que, na equação $(1.1)$:
$$-0,55=8,4\times10^{-5}+\frac{1}{2}0,3-\Omega_{\Lambda0}\implies\Omega_{\Lambda0}=0,7$$