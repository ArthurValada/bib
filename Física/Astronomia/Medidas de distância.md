Medir distâncias é importante para diversas áreas da astronomia, principalmente a [[Medidas de parâmetros cosmológicos|cosmologia]], no entanto, não se trata de uma tarefa fácil, requerendo diferentes técnicas para diferentes objetos a diferentes distâncias. Todas estas técnicas precisam ser calibradas com base em dados mais sólidos, servindo de base para novas técnicas, assim, estrutura-se a chamada "escada de distâncias". 
## Medições diretas
![[Pasted image 20240105154415.png]]
Os objetos astronômicos mais próximos da terra podem ter suas distâncias medidas de forma direta, por radar ou usando paralaxe.
### Radar
As medidas de radar são tecnicamente simples: basta emitir uma onda de rádio na direção que o planeta vai estar baseando-se numa estimativa de sua velocidade e medir o tempo $\Delta t$ que leva para a reflexão dessa onda ser absorvida de volta à terra. Baseando-se nisso, a distância $r$ do objeto é
$$d=\frac{c\Delta t}{2}$$
Telescópios de rádio como o Arecibo são muito usados para essas medições. Atualmente são mais empregados para medir a distância de asteróides a distâncias menores que $10AU$. Para distâncias maiores a reflexão fica muito fraca para ser detectada. 
### Paralaxe
Usando as medidas de Radar é possível determinar com precisão a órbita da terra, e a partir disso podemos usar o paralaxe para determinar distâncias de objetos fora do sistema solar. O paralaxe é calculado a partir do ângulo em que um objeto é visto a partir de dois locais distintos. Quanto mais longes estes dois locais estão, menor a resolução angular necessária para determinar a distância $d_\pi$ do objeto.
$$d_\pi=\left(\frac{b}{1AU}\right)\left(\frac{1"}{\theta}\right)1pc$$
A medida de paralaxe nos institui uma unidade conveniente, o *parsec*, ou seja, paralaxe para 1 segundo de arco, como a fórmula deixa claro. $b$ é a distância entre os dois pontos de medição, a qual queremos maximizar, então usamos a órbita da terra $b=2AU$, de modo que as medidas de paralaxe devem ser feitas de 6 em 6 meses.

Este método é limitado pela resolução angular de nossos telescópios. Um dos primeiros grandes catálogos (surveys) de distâncias astronômicas foi feito pelo satélite Hipparcos, com uma resolução angular de $0,001"$ (milissegundo de arco), e mapeou a distância de 10 mil objetos.  Pondo a resolução angular na fórmula, podemos ver que a distância máxima que Hipparcos pode medir foi de
$$
d_\pi=\left(\frac{2AU}{1AU}\right)\left(\frac{1"}{0,001"}\right)1pc=2kpc
$$
O survey mais preciso de estrelas até o momento foi o do satélite Gaia, que mapeou 1,7 bilhões de estrelas com uma resolução de $0,000001"$ (microssegundo de arco), o que teoricamente permite medições de objetos com distâncias de até $2Mpc$. No entanto, apesar da capacidade de resolver paralaxes tão pequenos, o que limita este método é a capacidade de resolver objetos específicos, a distâncias tão grandes.

Para referência, a Grande Nuvem de Magalhães está a $\approx 50 kpc$ e Andrômeda a $\approx 0,8 Mpc$.
## Velas padrão
Para escalas maiores que $1Mpc$ se torna impossível utilizar astrometria e paralaxe para determinar distâncias, de modo que outros métodos precisam ser utilizados. Os principais métodos de medição de distâncias astronômicas se baseiam em [[Fotometria]], i.e., partindo da luminosidade de um objeto, basta medir o fluxo aparente para determinar a distância até o objeto.

No entanto, saber a luminosidade de um objeto não é uma tarefa trivial e existem vários trabalhos estatísticos que classificam os objetos  de acordo com suas propriedades de modo a *padronizar* sua luminosidade em relação a algum outro parâmetro mensurável. Daí surge o termo *velas padrão*.

![[Pasted image 20240105155017.png]]
A imagem acima mostra diversos métodos de calibragem de velas padrão, por exemplo:
1. Cefeidas em aglomerados de estrelas tem suas distâncias calibradas por paralaxe espectroscópico (BW);
2. Estas cefeidas são usadas para calibrar cefeidas do grupo local (LMC) e outras identificadas pelo Telescópio Espacial Hubble (HST);
3. Estas são usadas para calibrar distâncias de Supernovas do tipo Ia e também a confirmar distâncias de galáxias para usar a relação de Faber-Jackson, a relação de Tully-Fischer e a relação Sigma-D;
4. Sabendo a distância das galáxias é possível calibrar a [[Fundamentos da cosmologia#Galáxias possuem redshift proporcional a suas distâncias|lei de Hubble]] para descobrir galáxias muito distantes. 
### Paralaxe espectroscópico
Este método - nada relacionado a paralaxe - envolve fazer um diagrama de Hertzsprung-Russel (HR) de uma população de estrelas a se analisar (geralmente de um mesmo aglomerado) e estimar a distância dessa população de modo a aproximar a sequência principal da população à sequência esperada para uma população típica de estrelas (considerando metalicidade e etc).

Para as distâncias que este método é aplicável (de 1 a 1000 kpc, como mostra o diagrama), usa-se o efeito Bappu-Wilson (BW) para identificar linhas espectrais e descobrir o redshift das estrelas. Sabendo o redshift basta estimar a distância da população, o que implica em mudar a estimativa da curva de magnitude absoluta para a sequência principal.

Este método é limitado pela capacidade de resolver estrelas individuais, para criar o diagrama de HR da população.
### Estrelas variáveis
Algumas estrelas são intrinsecamente instáveis, de modo a colapsar e reexpandir periodicamente. Sabendo disso, foi descoberto que é possível relacionar linearmente o período das oscilações e a luminosidade delas, ou seja, é possível padronizar estrelas variáveis para descobrir suas luminosidades e respectivamente suas distâncias.

Tecnicamente existem dois principais grupos de estrelas variáveis: as Cefeidas (como as estrelas variáveis são conhecidas) e as RR Lyrae.
### Supernovas do tipo Ia
Supernovas do tipo Ia (SN Ia) são supernovas que decorrem como resultado da interação de um sistema binário com uma anã branca e outra estrela (seja uma gigante ou mesmo uma anã branca menor).

Devido a sua densidade, a anã branca rouba massa da estrela maior, no entanto, anãs brancas,  que usualmente são inativas, ao atingir uma certa massa crítica, se reacendem causando uma reação em cadeia que gera a supernova. Essa massa é conhecida como massa de Chandrasekhar e equivale a $1,44$ massas solares (as anãs brancas tem de $0,17$ a $1,44$ massas solares).

Pelo fato de as energias envolvidas na reação em cadeia serem bem características, a curva de luminosidade em relação ao tempo das SN Ia são padronizáveis tornando-as uma das principais velas padrão.

Supernovas desse tipo emitem energia capaz de ofuscar uma galáxia inteira, tornando este um dos melhores métodos de determinação de distâncias, limitados apenas pela frequência que estas SNs ocorrem.
### Padronização de propriedades de galáxias
É possível inferir a luminosidade de galáxias usando padrões estatísticos de suas propriedades mensuráveis, como formato e curva de rotação. Para galáxias elípticas se usa a relação de Faber-Jackson, que diz que a luminosidade absoluta de uma galáxia se relaciona a velocidade média de suas estrelas na forma
$$L \propto V^4$$
Esta mesma relação foi identificada para galáxias espirais por Tully-Fischer. A velocidade média das estrelas de uma galáxia pode ser calculada a partir de mapas de redshift da galáxia.

A relação Simga-D relaciona o diâmetro angular $D$ de uma galáxia espiral a sua dispersão de velocidades $\sigma$. $D$ é mais precisamente o diâmetro angular da galáxia até um limite específico de luminosidade superficial absoluta, de modo que serve de base para calcular a luminosidade absoluta da galáxia. Os dois valores são relacionados na forma
$$log(D)=1,333log(\sigma)+C$$
Onde $C$ é uma constante que depende da distância ao aglomerado da galáxia.