## O céu noturno é escuro
É provado que se o universo tivesse tamanho infinito, idade infinita, homogêneo e euclidiano, o céu teria luminosidade infinita, pelo paradoxo de Olbers. A solução encontrada para o paradoxo é que nosso universo e as estrelas tem idade finita (baseado no que mostraremos abaixo), assim, as estrelas mais distantes ainda não tiveram tempo de iluminar a terra.
## Em largas escalas o universo é isotrópico e homogêneo
Em pequenas escalas o universo é bastante inomogêneo e anisotrópico, i.e. existem várias diferenças de massa para diversas escalas, de  $3m$, para $3AU$ até $3Mpc$. Na escala de $3 Mpc$, as galáxias são inomogeneidades e é possível determinar uma direção relevante: de Andrômeda (M31) para a Via Láctea, assim também é anisotrópico nessa escala.

Mas para escalas de de $100Mpc$, as estruturas são em média similares: não se formão super mega aglomerados de galáxias, os superaglomerados são as maiores estruturas que se observa. Isotropia e homogeneidade do universo são o que definimos como *princípio cosmológico*.

> É possível ser inomogêneo e isotrópico em um único ponto e é possível ser anisotrópico e homogêneo. Já isotropia em **todos** os pontos implica em homogeneidade.

## Galáxias possuem redshift proporcional a suas distâncias
Sendo $\lambda_{ex}, \lambda_{ob}$ respectivamente o comprimento de onda experimental e o comprimento de onda observado, o valo do redshift $z$ de um dado objeto é
$$z \equiv \frac{\lambda_{ob} - \lambda_{ex}}{\lambda{ex}}$$
Quando $z$ é negativo, podemos chamar de blueshift.

A *lei de Hubble* diz que o redshift de uma galáxia distante é proporcional a sua distância $r$:
$$z = \frac{H_0}{c} r \tag{2.1}$$
Onde $H_0$ é a constante experimental chamada *constante de Hubble*. Assumindo que o redshift é uma consequência do efeito Doppler, $z = v/c$, encontramos a velocidade de afastamento radial das galáxias como sendo
$$v = H_0 r \tag{2.2}$$
Dados recentes aproximam o valor da constante de Hubble a
$$H_0 = 70 \pm 3 km\,s^{-1}\,Mpc^{-1}$$
O afastamento das galáxias é também homogêneo e isotrópico, ou seja, todas as distâncias entre todas as galáxias obedecem essa mesma lei.

A constante de Hubble pode ser parametrizada na forma
$$H_0 = 100 km\,s^{-1}\,Mpc^{-1} \times h$$
Onde $h$ é um parâmetro mais preciso da constante de Hubble. Isto permite que possa-se fazer modelos com diferentes valores específicos da constante, mantendo uma mesma ordem de grandeza. A colaboração do telescópio espacial Planck nos dá valores de $h = 0,68 \pm 0,5$ e a colaboração SH0ES resultou em valores de $h = 0,73 \pm 1$.

Considerando apenas a lei de Hubble como fator de afastamento das galáxias (desprezando a gravidade e outros efeitos), podemos descobrir o tempo $t_0$ em que as galáxias estavam com uma distância $r=0$ entre si:
$$t_0 = \frac{r}{v} = \frac{r}{H_0 r} = H_0^{-1}$$
Para o valor que conhecemos da constante de Hubble, $t_0 = H_0^{-1} = 14 \pm 1,4 Gyr$ (giga anos), o que é aproximadamente a idade das estrelas mais velhas que conhecemos.

## O universo tem diferentes tipos de partículas
As partículas fundamentais são:
![[Pasted image 20230918171916.png|450]]
Os quarks formam bárions:
![[Pasted image 20230918172225.png]]

**Neutrons** livres (fora de um átomo) são instáveis e decaem em protons em $\tau_n = 890 s$, enquanto que os prótons tem meia vida maior que a idade atual do universo. O decaimento de neutrons em **prótons**, chamado de decaimento beta, emite **neutrinos**.

Cerca de $3/4$ da matéria no universo é hidrogênio e os $1/4$ restantes são em sua maioria hélio. Todos os outros materiais são apenas traços.

**Neutrinos** vem nos mesmos sabores que os leptons e não tem uma massa conhecida. Os seus sabores também oscilam.

**Fótons** não tem massa e são caracterizados por sua frequência $f = c/\lambda$ ou por sua energia $E = hf$. Fótons interagem com quase todas as outras partículas, podendo separar elétrons de átomos (fotoionização) e os mais energéticos podem quebrar átomos (fotodissociação).

Gás ionizado é bastante opaco aos fótons, pois os elétrons livres interagem bastante com os fótons.

Fótons podem ser facilmente produzidos por radiação de corpo negro. A densidade de energia emitida por radiação de corpo negro nas frequências entre $f$ e $f + df$ é
$$\epsilon (f) df = \frac{8\pi h}{c^3} \frac{f^3 df}{exp(hf/kT)-1}$$
Com seu pico por temperatura de
$$f_{max}\approx 2,82k T/h \tag{3.1}$$
e energia total
$$\int_0^\infty \epsilon(f)df = \epsilon_\gamma = \alpha T^4 \tag{3.2}$$
onde
$$\alpha = \frac{\pi^2 k^4}{15 \bar h^3 c^3} = 7,56 \times10^{-16} J m^{-3} K^{-4}$$
**Matéria escura** é qualquer matéria que seja muito difícil de se ver.
## O universo é cheio de radiação cósmica de fundo
A Radiação Cósmica de Fundo (CMB) é um "ruído" de radiação isotrópico que possui um espectro de corpo negro de $T_0 = 2,725 \pm 0,001 K$. O que  nos dá uma densidade de energia de $\epsilon_\gamma = 4,17 \times 10^{-14} J\,m^{-3}=0,260MeVm^{-3}$.

A cada centímetro cúbico do espaço se têm 411 fótons do CMB.

O CMB formou-se no universo primitivo, quando as temperaturas eram muito altas ($T >> 10^4K$) para elétrons constituírem átomos. Com altas temperaturas, foi emitida muita radiação de corpo negro, que formou o CMB. Com a expansão do universo, ele se resfriou, os elétrons formaram átomos, permitindo que os fótons os permeiem livres.

O que levou ao resfriamento de $\sim 10^4K$ para $2,725K$ foi a subsequente expansão do universo, já que o aumento no volume dele implica na diminuição de sua pressão (pela primeira lei da termodinâmica), mas a pressão de um gás de fótons é proporcional a sua energia, então o aumento no volume leva a diminuição da pressão e assim a diminuição da energia dos fótons.