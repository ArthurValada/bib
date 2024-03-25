Nos demais textos, foi assumido que [[Fundamentos da cosmologia#Em largas escalas o universo é isotrópico e homogêneo|em largas escalas o universo é isotrópico e homogêneo]]. No entanto, para escalas menores é possível se identificar estruturas - tipo sua casa. Como vimos, estruturas primordiais podem ser observadas na [[Radiação cósmica de fundo]].

As estruturas podem são formadas a partir de flutuações de densidade em relação a densidade média de energia do universo $\bar\epsilon(t)=\frac{1}{V}\int_V\epsilon(\vec r,t)d^3r$ ($V\ll$ maiores estruturas). As flutuações podem ser observadas a partir de uma flutuação adimensional na forma
$$\delta(\vec r,t)=\frac{\epsilon(\vec r,t)-\bar\epsilon(t)}{\bar\epsilon(t)} \tag{1.1}$$
Este valor é definido de modo que superdensidades têm $\delta>0$ e subdensidades têm $\delta<0$. No limite de um universo quasi homogêneo (como era primordialmente, pois as flutuações eram mínimas) temos $\delta\to0$. Neste limite é possível aplicar a Teoria de Perturbação Linear (LPT).

> Destaca-se que o menor valor da flutuação é o caso do vácuo: $\epsilon(\vec r,t)=0\implies\delta=-1$, de modo que $\delta$ não pode ser inferior à $-1$.

## Instabilidade gravitacional
Estatisticamente, flutuações em escalas quânticas num gás são esperadas, sem a formação de potenciais gravitacionais. No entanto, modelos inflacionários preveem que estas flutuações tenham sido amplificadas junto com o fator de escala em ordens de grandeza próximas de $e^{50}$.

A partir das flutuações de densidade numa região do espaço, duas coisas podem acontecer:
- Se a flutuação for grande o suficiente, a energia na região colapsa formando uma estrutura gravitacionalmente ligada, na qual se aplica o [[TeoremaDoVirial.pdf|Teorema do Virial]] ($\ddot I \approx 0$);
- Ou a pressão interna causa oscilações acústicas.

Para diferenciarmos os dois casos precisamos analisar o caso do colapso gravitacional de uma esfera de raio $R$ e massa
$$M=\frac{4}{3}\pi\bar\rho(1+\delta(t))R(t)^3 \tag{2.1}$$
>Assumindo $\bar\rho$ constante na escala de tempo do colapso, o que é razoável para fluidos não relativísticos.

(vale lembrar que $\rho(\vec r)=\bar\rho+\delta\bar\rho$).

A aceleração do raio $R$ da esfera é dada por
$$\ddot R=-\frac{G\Delta M}{R^2}=-\frac{G}{R^2}\left(\frac{4\pi}{3}R^3\bar\rho\delta\right)=-\frac{4}{3}\pi G\bar\rho\delta R \tag{2.2}$$
Isso implica que uma flutuação positiva causa um colapso ($\ddot R<0$) e uma flutuação negativa causa uma expansão ($\ddot R>0$).

Além disso, em um colapso, a massa é conservada $\dot M=0$, assim, invertendo $(2.1)$ temos
$$R(t)=\sqrt[3]{\frac{3M}{4\pi\bar\rho}\frac{1}{1+\delta(t)}}=R_0(1+\delta(t))^{-1/3}$$
Onde
$$R_0\equiv\sqrt[3]{\frac{3M}{4\pi\bar\rho}}$$
No limite $\delta\to0$ temos a expansão gravitacional
$$R(t)\approx R_0\sqrt[3]{1-\frac{1}{3}\delta(t)}\implies\ddot R\approx-\frac{1}{3}R_0\ddot\delta$$
Substituindo isto na  equação $(2.2)$ temos a equação diferencial:
$$\ddot\delta=4\pi G\bar\rho\delta \tag{2.3}$$
A solução geral para essa equação é
$$\delta(t)=A_1e^{t/t_d}+A_2e^{-t/t_d}\tag{2.4}$$
Onde $A_1,A_2$ são constantes de integração e $t_d$ é o tempo dinâmico de colapso, definido como
$$t_d\equiv\frac{1}{\sqrt{4\pi G\bar\rho}}=\sqrt\frac{c^2}{{4\pi G\bar\epsilon}} \tag{2.5}$$
O único fator que influencia no tempo dinâmico é a densidade.

> Veja que para uma flutuação inicialmente estática, $\dot\delta=0$, a função se comporta de forma muito similar ao cosseno hiperbólico.

Quando o colapso de uma nuvem de gás ocorre, a pressão interna impede que se colapse completamente, fazendo com que o objeto volte a expandir causando oscilações. Mas para isso acontecer a pressão deve se propagar mais rápido que o colapso. O tempo de propagação da pressão $t_p$ até um raio $R$, é determinado pela [[Dinâmica cosmológica#Equação de estado|velocidade do som]] no fluido:
$$t_p= R/c_s$$
De modo geral, para haver oscilações, precisamos que $t_p<t_d$. James Jeans foi um dos primeiros astrônomos a realizar estes cálculos, assim se definindo o *comprimento de Jeans*
$$\lambda_J=2\pi c_st_d$$
Dessa forma, regiões de superdensidade com diâmetros maiores que o comprimento de Jeans colapsam de modo a formar uma estrutura. Enquanto que regiões com diâmetros menores que o comprimento de Jeans, durante o colapso, atingem pressão interna elevada o suficiente para voltar a expandir, fazendo oscilações acústicas até atingir equilíbrio gravitacional.
## Comprimento de Jeans na cosmologia
Para uma análise cosmológica, determinamos a distânca de Hubble $cH^{-1}$ e o tempo de Hubble $H^{-1}$ no instante de [[Radiação cósmica de fundo#Scattering|desacoplamento]] $z_{dec}=1100$:
$$H(z_{dec})^{-1}=\sqrt\frac{3c^2}{8\pi G\bar\epsilon}=\sqrt\frac{3}{2}t_d$$
E
$$\frac{c}{H(z_{dec})}=0,2Mpc$$
De modo que
$$\lambda_J=2\pi\sqrt\frac{2}{3}\sqrt w\frac{c}{H}$$
Apesar de a igualdade radiação-matéria ter ocorrido bem antes do desacoplamento, a [[Radiação cósmica de fundo|razão bárion-fóton]] ainda é muito pequena para que os bárions sejam relevantes no fluido fóton-bárion, assim, a velocidade do som do fluido é de $c_s\approx\sqrt\frac{1}{3}c$, de modo que o comprimento de Jeans é
$$\lambda_{Jfb}\approx2\pi\sqrt\frac{2}{3}\sqrt \frac{1}{3}\frac{c}{H}\approx3,0\frac{c}{H}\approx0,6Mpc$$
Portanto, flutuações de densidade menores que 3 distâncias de Hubble não teriam densidade o suficiente para causar colapso gravitacional, gerando apenas oscilações acústicas. Isto muda após o desacoplamento, em que os fótons não exercem pressão sobre o fluido, de modo que a velocidade do som para os bárions se torna
$$c_{sbar}=\sqrt\frac{kT}{mc^2}c$$
Considerando a fração de hidrogênio e hélio do universo e usando a temperatura medida a partir da radiação cósmica de fundo, é possível determinar que a velocidade do som para o gás bariônico resultante foi de
$$c_{sbar}\approx1,5\times10^{-5}c\approx5km/s$$
Em comparação a velocidade do som dos fótons, temos uma razão de 
$$C=\frac{c_{sbar}}{c_{s\gamma}}=\frac{1,5\times10^{-5}}{\sqrt\frac{1}{3}}=2,6\times10^{-5}$$
Assim, podemos calcular a massa de bárions dentro de um comprimento de Jeans necessária para gerar um colapso, a Massa de Jeans
$$M_J\equiv\rho_{bar}\frac{4}{3}\pi\lambda_J^3$$
Imediatamente antes do desacoplamento, a massa de Jeans era de $M_J(antes)\approx7\times10^{18}M_\odot$, uma massa superior a de qualquer aglomerado conhecido. Após o desacoplamento, a massa de Jeans era de
$$M_J(depois)=C^3M_J(antes)\approx10^5M_\odot$$
O que é comparável a massa das menores galáxias anãs e bem menor que a massa da nossa galáxias ($\sim10^{11}M_\odot$).

Ou seja, as primeiras estruturas do tamanho que conhecemos se formaram aproximadamente no período de desacoplamento.
## Expansão do universo
A expansão do universo e o tempo dinâmico de colapso ocorreram em escalas de tempo similares, portanto, não podemos desconsiderá-la. Para isso, precisamos considerar o termo médio na equação $(2.2)$
$$\ddot R=-\frac{GM}{R^2}=-\frac{4}{3}\pi G(\bar \rho R-\delta\bar\rho R) \tag{4.1}$$
Além, disso, pela conservação de massa, temos que
$$R(t)\propto\rho^{-1/3}=\bar\rho^{-1/3}(1+\delta(t))^{-1/3}$$
Usando $\bar\rho\propto a^{-3}$
$$R(t)\propto a(1+\delta(t))^{-1/3}$$
Derivando isto duas vezes temos:
$$\frac{\ddot R}{R}=\frac{\ddot a}{a}-\ddot\delta/3-\frac{2}{3}\frac{\dot a}{a}\dot\delta \tag{4.2}$$
Dividindo ambos os lados da equação $(4.1)$ por $R$ e substituindo a equação $(4.2)$ temos
$$\frac{\ddot a}{a}-\ddot\delta/3-\frac{3}{2}H\dot\delta=-\frac{4}{3}\pi G\bar\rho+\frac{4}{3}\pi G\bar\rho\delta$$
Desta expressão, o caso de um universo perfeitamente homogêneo ($\delta=0$) gera a [[Dinâmica cosmológica#Equação da aceleração|equação da aceleração]]. Podemos subtrair este caso da equação, tendo como resultado a equação diferencial
$$\ddot\delta+2H\dot\delta=4\pi G\bar\rho\delta\tag{4.3}$$
Esta equação difere da equação $(2.3)$ pelo termo linear $2H\dot\delta$. Este termo é eliminado no caso de um universo estático com $H=0$.

Um cálculo relativístico mais avançado resulta na equação
$$\ddot\delta+2H\dot\delta=\frac{4\pi G}{c^2}\bar\epsilon_m\delta$$
É conveniente reescrever a equação em termos do parâmetro de densidade de massa $\Omega_m=\frac{\bar\epsilon_m}{\epsilon_c}=\frac{8\pi G\bar\epsilon_m}{3c^2H^2}$:
$$\ddot\delta+2H\dot\delta-\frac{3}{2}\Omega_mH^2\delta=0 \tag{4.4}$$
Podemos assumir valores para $\Omega_m$ de modo a simplificar a equação. [[Modelos cosmológicos#Universos de único componente|Dois casos de interesse]] são:
- A época em que a radiação dominava a expansão do universo ($\Omega_m<<1$), em que $H=1/(2t)$, quando a maioria das estruturas se formaram;-
- A época em que a matéria dominava o universo ($\Omega_m\approx1$), em que $H=2/(3t)$, que constituiu a maior parte da história do universo;

No primeiro caso, a equação se resume a
$$\ddot\delta+\frac{1}{t}\dot\delta\approx0$$
Que tem uma solução na forma
$$\delta(t)\approx B_1+B_2\ln t \tag{4.5}$$
Ou seja, na época da radiação, flutuações de densidade cresciam logaritmicamente.

Na época da matéria, a equação diferencial toma a forma
$$\ddot\delta+\frac{4}{3t}\dot\delta-\frac{2}{3t^2}\delta=0$$
Que tem uma solução geral na forma
$$\delta(t)\approx C_1t^{2/3}+D_2t^{-1}\tag{4.6}$$
> Lembrando que este é o modelo linear de pertubações e só se aplica para $|\delta|\ll1$. Para $\delta\sim1$, as pertubações não seguem mais este modelo e precisam ser modeladas com modelos não lineares, com soluções numéricas. 

Para largas escalas de tempo, o segundo termo se torna desprezível, de modo que o primeiro termo tem forma similar ao fator de escala para um universo dominado por matéria: $a(t)=(t/t_0)^{2/3}$. Assim, desprezando o segundo termo, temos que
$$\delta(t)\propto t^{2/3}\propto a(t)=\frac{1}{1+z}\tag{4.7}$$
Isto significa que se as perturbações só começassem a se formar no redshift de desacoplamento $z_{dec}\approx1100$, as flutuações só teriam crescido 1100 vezes.
## Espectro de potência
Uma forma eficiente de entender as propriedades estatísticas de $\delta(\vec r)$ é fazendo uma expansão de Fourier na forma
$$\delta(\vec r)=\frac{V}{(2\pi)^3}\int\delta_{\vec k}e^{-i\vec k\cdot\vec r}d^3k$$
Onde os componentes individuais de Fourier são
$$\delta_{\vec k}=\frac{1}{V}\int\delta(r)e^{-i\vec k\cdot\vec r}d^3r$$
Assim, quebramos a função $\delta(\vec r)$ em infinitas funções senoidais $\delta_{\vec k}$ com número de ondas $\vec k$ e comprimento de onda
$$\lambda=2\pi/k$$
Para todos estes valores, usamos o [[Métricas e curvaturas#As métricas de Minkowski e de Friedman-Lamaître-Robertson-Walker|sistema de coordenadas comoveis]].

Cada um dos componentes de Fourier obedece por si só a equação diferencial $(4.4)$, desde que o comprimento de onda próprio seja maior que o comprimento de Jeans   e menor que o comprimento de Hubble $\lambda_J<a(t)\lambda<c/H$. Se o comprimento de onda próprio for maior que o comprimento de Hubble, então as oscilações não estão causalmente conectadas, assim $\delta(t)\propto a(t)$.

A média quadrada dos componentes de Fourier é o *espectro de potência*:
$$P(k)=\left<|\delta_k|^2\right>$$
Para uma escala específica de oscilação $2\pi/k$, a função do espectro de potência define uma média da amplitude das flutuações. A média é uma aproximação válida das propriedades estatísticas das flutuações pois elas consistem num *campo gaussiano* (distribuição gaussiana das propriedades do campo).

As flutuações causadas pela inflação do universo têm um espectro de potência na forma de uma lei de potência
$$P(k)\propto k^{n_s} \tag{5.1}$$
O valor $n_s$ é o *índice espectral*, com $n_s=1$ correspondendo ao modelo de Harrisson-Zel'Dovich, que assume flutuações independentes de escala. Surveys da radiação cósmica de fundo implicam em um índice espectral de $n_s=0,96$.

Ou seja, imediatamente após desacoplamento, num universo apenas com matéria bariônica e radiação, se esperaria que o espectro de potência das pertubações de densidade seguisse a forma da equação $(5.1)$.

## O papel da matéria escura
A pressão do fluido fóton-bárion impede o colapso esférico causando as oscilações acústicas bariônicas, dessa forma, a matéria escura, que não tem pressão interna pode ser uma forma de iniciar o processo de formação de estruturas (*seeding*).

Se a matéria escura for quente (relativística), não se formam potenciais devido ao efeito de *free streaming*, o que impede a formação de pequenas estruturas (menores que a velocidade da luz). Um exemplo de matéria escura quente são neutrinos relativísticos.

Se a matéria escura for fria, flutuações com correlação causal podem sofrer o colapso esférico, o que aumenta a amplitude significativamente após a era da radiação (antes o crescimento era logarítmico).

Independente do modelo da matéria escura, para flutuações maiores que a distância de Hubble temos $\delta(t)\propto a(t)$. Assim, na época da radiação, para grandes escalas temos $\delta(t)\propto t^{\frac{1}{2}}$, enquanto que para pequenas escalas $\delta(t)\propto\ln t$, de modo que as maiores flutuações crescem mais rápido e as menores ficam efetivamente congeladas congeladas.

De modo geral temos:

| Escala                         | Sem DM                        | CMD                                   | HDM                               |
| ------------------------------ | ----------------------------- | ------------------------------------- | --------------------------------- |
| $\frac{2\pi}{k}<\lambda_J$     | Colapso de Jeans              | Colapso Jeans                         | Colapso de Jeans                  |
| $d_H>\frac{2\pi}{k}>\lambda_J$ | Espectro de potência de fundo | $\delta(t)\propto \ln t$ até $t_{rm}$ | Crescimento impedido até $t_{rm}$ |
| $d_H<\frac{2\pi}{k}$           | $\delta(t)\propto a(t)$       | $\delta(t)\propto a(t)$               | $\delta(t)\propto a(t)$           |
