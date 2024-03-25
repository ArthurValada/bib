A [[Dinâmica cosmológica#Equação de Friedmann|equação de Friedmann]] pode ser reescrita em termos dos componentes dos parâmetros de densidade, usando a equação de estado de cada componente do universo, que pode ser simplificada, gerando a fórmula de diluição de energia
$$\epsilon_w(a) = \epsilon_{w0}a^{-3(1+w)} \tag 1$$
Assim, a equação de Friedmann, dividida por $H_0$ toma a forma
$$\frac{H^2}{H^2_0}=\frac{8\pi G}{3c^2}\frac{\epsilon}{H^2_0}=\frac{\sum\epsilon_{w0}a^{-3(1+w)}}{\epsilon_{c0}}$$
Substituindo os parâmetros das equações de estado de cada componente:
$$\frac{H^2}{H_0^2} = \Omega_{r0} a^{-4} + \Omega_{m0} a^{-3} + \Omega_{k0} a^{-2} + \Omega_{\Lambda 0} \tag 2$$
Onde $\Omega_{i0}$ são os parâmetros de densidade, respectivamente, da radiação (componentes com $w=\frac{1}{3}$); da matéria, bariônica ou não ($w=0$); da curvatura, que falaremos adiante e; $\Omega_{k0} = 1 - \Omega_0$ é o parâmetro de densidade de curvatura atual e
$$\Omega_{k0} = - \frac{k c^2}{R_0^2 H_0^2}$$
Ou seja, para uma curvatura esférica, $k=1, \Omega_{k0} < 0$, para uma curvatura hiperbólica, $k=-1, \Omega_{k0} > 0$ e para um universo plano, $k=0, \Omega_{k0} = 0$. Outros componentes podem facilmente serem adicionados, com base em sua equação de estado.

Em suma, a equação de diluição de energia $(1)$ nos permite descobrir como cada componente do universo contribuía com sua expansão, para um determinado fator de escala $a$.

Na  equação $(2)$, sabemos, primeiramente que $H^2 = (\dot a/ a)^2$ vai ser sempre positivo, e que os demais fatores são constantes. Podemos criar diversos modelos de universos com diferentes contribuições de cada um dos componentes e assim ver como eles evoluem.

## Universos de único componente
Tomando apenas um dos parâmetros de densidade como não nulo, obtemos resultados relativamente similares:
- Para um universo com apenas radiação, o universo cresce infinitamente. A idade do universo é metade do tempo de Hubble ($t_0=\frac{1}{2H_0}$) e a sua taxa de crescimento é $a(t)=\left(\frac{t}{t_0}\right)^{1/2}$
- Para um universo plano com apenas matéria, $t_0 = \frac{2}{3H_0}$ e $a(t) = \left(\frac{t}{t_0}\right)^{2/3}$  (conhecido como universo de Einstein-de-Sitter)
- Para um universo apenas com a constante cosmológica, o universo possui um eterno crescimento exponencial sem começo nem fim, na forma $a(t)=e^{H_0(t-t_0)}$
- Para um universo vazio, com curvatura, temos claro, 2 opções: um universo vazio, que não cresce nem diminui ou um universo hiperbólico na forma $a(t) = t/t_0$. Universos vazios de curvatura positiva não existem;

Vale lembrar que estes modelos se aplicam com certa margem de erro para universos em que os outros parâmetros de densidade são desprezíveis. Costumamos falar de universos dominados por matéria por exemplo. Estes modelos simplificados podem servir como um bom modelo para certas épocas do universo

## Modelos de múltiplos componentes e o modelo padrão
Em modelos com múltiplos componentes, há períodos de dominância de componentes específicos, o que, consequentemente, implica em parâmetros de Hubble diferentes na evolução do universo. Em geral, podem haver universos que:
- Crescem eternamente, quando todos os parâmetros são positivos ou nulos (Big Chill);
- Começam diminuindo, depois tornam a crescer (Big Bounce). Estes universos são obtidos quando se tem curvatura negativa e $\Lambda > 0$;
- Crescem, atingem um máximo e colapsam de forma temporalmente simétrica (Big Crunch). Eles são obtidos especificamente para $\Lambda < 0$, pois, depois de todos os parâmetros se diluírem, lambda dominará e levará a um colapso exponencial, ou universos sem $\Lambda$, mas com curvatura positiva ($\Omega_{k0}$ negativo);
- Existe um caso específico chamado universo ocioso ou universo de Lamaître, que tem uma balança específica de parâmetros que permite criar um período com $H(t) = 0$, e quão mais próximo um universo está destes parâmetros ideais, maior a estaticidade. Depois da época estática, o universo pode colapsar ou crescer exponencialmente (dependendo de $\Lambda$);
Estes modelos estão modelados em https://gist.github.com/icarob-eng/fe79e34cdafd1ecf6015bdc5d6b9b16c

O nosso universo é efetivamente plano, com um $\Omega_{r0}$ muito baixo e estamos na transição da época dominada pela matéria para a época dominada pela constante cosmológica. No começo do universo houve a fase dominada por radiação, mas ela durou apenas $3,34 \times 10^{-6} H_0^{-1} \approx 47.000 yr$. Depois disso, a maior parte dos 13 bilhões de anos do universo foram dominadas por matéria, de modo que a época mais relevante para se estudar evolução de galáxias no universo, foi a época da dominação de matéria.

Para o cálculo de distâncias com o modelo padrão, temos que no limite $z\to\infty$ a [[Métricas e curvaturas#As métricas de Minkowski e de Friedman-Lamaître-Robertson-Walker|distância própria]] tende a $3,24c/H_0$. Ou seja, existe um limite observacional de distâncias chamado *horizonte observacional*.
$$d_{hor}=3,24c/H_0=3,24d_H=3,24\times4285Mpc=13,8Gpc$$