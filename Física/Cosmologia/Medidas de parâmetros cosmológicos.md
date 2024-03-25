Existem 3 formas de medir distâncias, as quais, quando comparadas com o redshift $z=\frac{\lambda_o-\lambda_e}{\lambda_e}=\frac{H_0}{c}r$, permitem determinar a constante de Hubble e, para redshifts maiores, o *parâmetro de desaceleração*, obtido matematicamente (sem nenhum modelo cosmológico) pela expansão de Taylor para o fator de escala:
$$a(t)\approx1+H_0(t-t_0)+\frac{1}{2}q_0H_0^2(t-t_0)^2$$Onde $q_0 \equiv -\left(\frac{\ddot a}{\dot a H^2_0}\right)_{t=t_0}$  é o parâmetro de desaceleração. Ele pode ser inserido na [[Dinâmica cosmológica#Equação de Friedmann|equação de Friedmann]] para resultar a expressão:
$$q_0 = \Omega_{r0}+\frac{1}{2}\Omega_{m0} - \Omega_{\Lambda0} \tag{1.1}$$
Onde $\Omega_{k0} = 0$. Baseado nisso, o [[Modelos cosmológicos#Modelos de múltiplos componentes e o modelo padrão|modelo padrão]] da cosmologia nos diz que $q_0 \approx -0,55$. Com base nisso, o universo pode ser descrito fenomenologicamente determinando apenas $H_0$ e $q_0$.

Também temos a expansão para a recíproca de $a(t)$:
$$\frac{1}{a(t)}\approx1-H_0(t-t_0)+\left(1+\frac{q_0}{2}\right)H_0^2(t-t_0)^2 \tag{1.2}$$
Isto pode ser usado para calcular a integral da equação da [[Métricas e curvaturas#As métricas de Minkowski e de Friedman-Lamaître-Robertson-Walker|distância própria (3.4)]] para encontrarmos a relação
$$d_p(t_0)\approx c(t_0-t_e)+\frac{cH_0}{2}(t_0-t_e)^2 \tag{1.3}$$
O primeiro termo seria a distância para um universo de tamanho constante ($a=1\implies d=c\Delta t$) e o segundo termo é uma correção para a expansão do universo durante o tempo em que o fóton viajou. Substituindo $z=1/a(t_e)-1$ na equação $(1.2)$, conseguimos a relação entre $z$ e $t_0-t_e$, que pode ser substituído na equação $(1.3)$, gerando a relação entre a distância e o redshift.
$$d_p(t_0)\approx\frac{c}{H_0}z\left(1-\frac{1+q_0}{2}z\right) \tag{1.4}$$
Esta equação permite determinar $H_0$ e $q_0$ sabendo a relação entre a distância e o redshift de galáxias. Determinar o redshift de um objeto é relativamente simples, requerendo apenas medir o espectro de uma galáxia e comparar as linhas de absorção observadas às linhas de absorção de elementos conhecidos.

No entanto, determinar a distância de objetos astronômicos é um processo bem mais envolvido que usa de diversas ferramentas diferentes. Os detalhes de como estas medições são feitas são discutidos em [[Medidas de distância]] e [[Fotometria]]. No presente texto vamos apenas classificar e revisar para o contexto de cosmologia as medidas em 3 tipos: medidas diretas, medidas usando réguas padrão e medidas usando velas padrão.
## Medições diretas
As [[Medidas de distância#Medições diretas|medições diretas]] de distâncias astronômicas, como radar planetário e paralaxe, valem apenas para pequenas distâncias e objetos locais que não sofrem efeitos cosmológicos relevantes.
## Velas padrão
Medidas de distância que se baseiam em [[Medidas de distância#Velas padrão|velas padrão]] no entanto, permitem mensurar distâncias muito grandes, de modo que a geometria e expansão do universo precisam ser consideradas. Artigos que calibram as velas padrão precisam especificar qual modelo cosmológico usam, em termos de constante de Hubble e parâmetros de densidade.

Dois efeitos afetam a medição de distâncias usando velas padrão e precisam se considerados na relação entre o fluxo, luminosidade e distância: distorções devido a geometria do espaço e mudanças no fluxo luminoso devido a perda de energia do redshift (pois o fluxo é uma medida de potência por área).

As distorções da geometria são descritas pela [[Métricas e curvaturas#As métricas de Minkowski e de Friedman-Lamaître-Robertson-Walker|métrica de Friedmann-Lamaître-Roberston-Walker]]. Seguindo a métrica FLRW, a *área própria* de uma esfera de raio $r$ num dado momento é
$$A_p(t_0)=4\pi S_k(r)^2$$
Já as mudanças de energia relativas ao redshift são relacionadas ao fator de escala $a(t)$. Sabendo que o fator de escala faz um comprimento de onda crescer do tempo de emissão ao tempo de observação na forma:
$$a(t_e)\lambda_0=\lambda_e\implies\lambda_0=\frac{\lambda_e}{a(t_e)}=\frac{\lambda_e}{(1+z)}$$
Usando $E=hc/\lambda$:
$$E_0=\frac{E_e}{1+z}$$
Juntando tudo temos a relação de distância, luminosidade e fluxo com correções cosmológicas,
$$f=\frac{L}{4\pi[S_k(r)(1+z)]^2}$$
Onde o termo ao quadrado é a chamada *distância de luminosidade*
$$d_L=S_k(r)(1+z) \tag{3.1}$$
Como sabemos, mesmo se nosso universo tiver curvatura, seu raio de curvatura é maior que o horizonte observável, de modo que $S_k(r)\approx d_p(t_0)$, assim, podemos substituir $(1.3)$ na $(3.1)$ para obter
$$d_L=d_p(t_0)(1+z)\approx\frac{c}{H_0}z\left(1-\frac{1+q_0}{2}z\right)(1+z)\approx \frac{c}{H_0}z\left(1+\frac{1-q_0}{2}z-\frac{1+q_0}{2}z^2\right)$$
Podemos desprezar o termo cúbico (apenas contribui com um fator de $(1+z)$) no limite $z\ll1$ de modo que a equação se torna
$$d_L\approx\frac{c}{H_0}z\left(1-\frac{1+q_0}{2}z\right) \tag{3.2}$$
Veja que no limite $z\to0,\;d_L\approx d_p(t_0) \approx\frac{c}{H_0}z$
## Réguas padrão
Apesar de não usual, é possível utilizar réguas padrão para determinar distâncias. Uma régua padrão é um objeto de  tamanho fácil de determinar, de modo que, medindo seu tamanho angular e comparando ao seu tamanho real, é possível determinar sua distância.

No sistema de coordenadas esféricas $(r,\theta,\phi)$, assumimos $r$ constante e medimos um tamanho angular $\delta \theta$ (para simplificar escolhemos um sistema em que $\delta\phi=0$), dessa forma, a distância $\ell$ entre as duas pontas da régua padrão é determinada pela métrica de Friedman-Lamître
$$\ell=ds=a(t_e)S_k(r)\delta\theta=\frac{S_k(r)\delta\theta}{1+z}$$
Baseado nisso, definimos a distância angular como sendo
$$d_A\equiv\frac{\ell}{\delta\theta}=\frac{S_k(r)}{1+z} \tag{4.1}$$
Veja que em comparação às equações $(1.4)$ e $(3.2)$, temos que
$$(1+z)d_A=d_p(t_0)=\frac{d_L}{1+z}$$
Baseado nisso
$$d_A\approx\frac{c}{H_0}z\left(1-\frac{3+q_0}{2}z\right) \tag{4.2}$$
Poucos objetos podem ser padronizados assim, sendo um dos principais exemplos as [[Radiação cósmica de fundo#Observações do CMB|Bolhas Acústicas Bariônicas]]. Apesar de serem associadas a padrões na radiação cósmica de fundo, elas também se relacionam com a distribuição atual de matéria, tendo raio próprio de $150Mpc$. Dessa forma, analisando a correlação angular de galáxias, é possível encontrar bolhas de BAO, as quais têm tamanho determinado pela cosmologia.
## Resultados experimentais
Para grandes distâncias, os métodos de velas padrão são os mais utilizados atualmente. Estes métodos são descritos pela equação $(3.2)$, transcrita abaixo.
$$d_L\approx\frac{c}{H_0}z\left(1-\frac{1+q_0}{2}z\right)$$
Como já discutimos, para $z\ll1$, $d_L\approx\frac{c}{H_0}z$, no entanto, para distâncias maiores que $z=1$, o termo quadrático produz erros na forma $\epsilon=-\frac{1+q_0}{2}z^2$, de modo que quanto maior a distância, maior o erro associado a $q_0$, podendo assim determina-lo com maior precisão. Dessa forma, o método para medir estes dois valores consiste em: medir distâncias próximas de redshift para determinar estatisticamente $H_0$ na relação linear e então medir distâncias maiores e determinar estatisticamente $q_0$.

Este é o método da escada de distâncias, usado em colaborações como a SH0ES: Supernova H0 for the Equation of State, que combinou dados de Parallax do survey da missão Gaia com dados de cefeidas e supernovas do telescópio espacial Hubble, gerando o resultado de $H_0=74,0\pm1,4km/s/Mpc$ e $q_0\approx-0,55$.

A evolução histórica das medidas valores de $H_0$ do SH0ES com os anos é mostrado na figura abaixo.

![[Pasted image 20240112182156.png|500]]