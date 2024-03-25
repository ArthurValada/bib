Sabemos que se o universo tiver curvatura positiva, o raio de curvatura não pode ser significativamente menor que a distância de Hubble ($c/H_0\approx4285Mpc$), senão, a luz de objetos próximos daria voltas no universo e notaríamos sua periodicidade.

## Derivação da equação de Friedmann
As equações de Friedmann partem de um princípio newtoniano (e euclidiano) de energia, para servir de base para princípios relativísticos. Tomando uma esfera homogênea de massa constante $M_s$, com densidade e raio relacionados na forma
$$M_s = \frac{4 \pi}{3} \rho(t) R_s(t)^3 \tag{1.1}$$
Supondo que a esfera cresça de modo
$$R_s(t) = a(t) r_s \tag{1.2}$$
Onde $r_s$ é o [[Métricas e curvaturas#As métricas de Minkowski e de Friedman-Lamaître-Robertson-Walker|raio co-móvel]] do universo e $a(t)$ o fator de escala.

Desse modo, para um objeto na superfície da esfera, temos a relação newtoniana de energia para um objeto de teste na distância $R_s$, como
$$E_{tot} = E_c - E_{pg}$$
Ou seja,
$$U = \frac{1}{2}\left(\frac{dR_s}{dt} \right)^2 - \frac{GM_s}{R_s(t)}$$
Fazendo as substituições $(1.1)$ para o termo da energia cinética e $(1.2)$ para o termo da energia potencial gravitacional:
$$\frac{1}{2} r^2_s \dot a^2 = \frac{4 \pi}{3} G \rho (t) a(t)^2 + U$$
Dividindo ambos os lados $r^2_s a(t)^2/2$, temos
$$\left( \frac{\dot a}{a} \right)^2 = \frac{8 \pi G}{3} \rho (t) + \frac{2U}{r^2_s} \frac{1}{a(t)^2} \tag{1.3}$$
Que é a forma newtoniana da equação de Friedmann.

## Equação de Friedmann
Ela pode ser expressa como:

$\text{Termo de expansão}^2 = \text{termo gravitacional} + \text{coeficientes do espaço} \times \frac{1}{\text{termo de escala}^2}$

Partindo de princípios relativísticos e não se limitando a uma esfera finita, a verdadeira equação de Friedman é:
$$\left( \frac{\dot a}{a} \right)^2 = \frac{8 \pi G}{3 c^2} \epsilon (t) - \frac{kc^2}{R_0^2} \frac{1}{a(t)^2} \tag{2.1}$$
Que permite descrever da [[Métricas e curvaturas#Métricas de espaços|curvatura do universo]] (descrita por $k$ e $R_0$) e depende da densidade de energia $\epsilon (t)$, já que partículas sem massa como fótons ainda possuem momento linear $p$ e energia da forma
$$E_{rel} = pc = hf$$
De modo geral, a energia total de um corpo é dada pela relação massa-energia
$$E^2 = m^2c^4 + p^2 c^2$$
Onde o momento linear é dado pelo movimento *peculiar* de cada partícula (que difere das tendências cosmológicas). Considerando um movimento não relativístico ($v << c$),
$$E \approx mc^2 (1 + v^2/c^2) \approx mc^2 + \frac{1}{2} m v^2$$
Veja que a equação de Friedmann permite relacionar a expansão do universo $a(t)$, sua curvatura e a energia.

A outra mudança feita é que o termo que chamamos de  "coeficientes do espaço" pode ser substituído como:
$$\frac{2U}{r^2_s} = - \frac{kc^2}{R^2_0} \tag{2.2}$$
Para finalizar, a [[Fundamentos da cosmologia#Galáxias possuem redshift proporcional a suas distâncias|constante de Hubble]] pode ser calculada para um dado $t$, de modo que generalizamos-a como *parâmetro de Hubble*,
$$v(t) = H(t) d(t).$$
Em termos do fator de escala:
$$\frac{\dot a}{a} = H(t)$$
De modo que a equação de Friedman fica
$$H(t)^2 = \frac{8 \pi G}{3 c^2} \epsilon (t) - \frac{kc^2}{R_0^2} \frac{1}{a(t)^2}. \tag{2.3}$$
No momento atual $t_0$
$$H_0^2 = \frac{8 \pi G}{3 c^2} \epsilon_0 - \frac{kc^2}{R_0^2}$$
Além disso, podemos achar uma densidade crítica tal que $k=0$:
$$\begin{split}
H(t)^2 &= \frac{8 \pi G}{3 c^2} \epsilon_c (t)
\\\epsilon_c(t) &\equiv \frac{3 c^2}{8 \pi G}H(t)^2
\end{split}
\tag{2.4}
$$
De modo que podemos fazer um desvio da densidade crítica, chamado de *parâmetro de densidade*
$$\Omega (t) \equiv \frac{\epsilon(t)}{\epsilon_c(t)}=\frac{8\pi G}{3c^2}\frac{\epsilon(t)}{H(t)^2},$$
com o qual podemos reescrever a equação de Friedmann na forma
$$\begin{split}
H(t)^2 &= \frac{8 \pi G}{3 c^2} \epsilon (t) - \frac{kc^2}{R_0^2a(t)^2}\\
1&=\frac{8\pi G}{3c^2}\frac{\epsilon(t)}{H(t)^2}-\frac{kc^2}{R_0^2a(t)^2H(t)^2}\\
1&=\Omega(t)-\frac{kc^2}{R_0^2a(t)^2H(t)^2}
\end{split}$$
$$1 - \Omega(t) = - \frac{k c^2}{R_0^2 a(t)^2 H(t)^2}. \tag{2.5}$$
Valores modernos nos dão $1 - \Omega \approx 10^{-3}$. Analisando a equação, vê-se que o sinal do lado direito da equação não muda com o avanço do universo, ou seja, o sinal da curvatura não muda na história do universo.

## Equação dos fluidos
Assumindo que o universo é adiabático:
$$\dot E + P \dot V = 0. \tag{3.1}$$
Sabemos que para um volume qualquer, em relação ao raio co-móvel é
$$V(t) = \frac{4 \pi}{3} (r_s a(t))^3$$
O que nos leva a
$$\dot V
= \frac{4 \pi}{3} r^3_s (3a^2 \dot a)
= V \left( 3\frac{\dot a}{a} \right). \tag {3.2}
$$
Além disso, $E = V \epsilon$, então a variação de volume é
$$\dot E
= V \dot \epsilon + \dot V \epsilon
= V \left(\dot \epsilon + 3 \frac{\dot a}{a} \epsilon \right) \tag{3.3}$$
Unindo $(3.1), (3.2)$ e $(3.3)$:
$$V \left(\dot \epsilon + 3 \frac{\dot a}{a} \epsilon \right) + P V \left( 3\frac{\dot a}{a} \right) = 0$$
ou seja,
$$\dot \epsilon + 3 \frac{\dot a}{a} (\epsilon + P) = 0 \tag{3.4}$$
Que é a chamada *equação dos fluidos*.

## Equação da aceleração
A equação de Friedmann $(2.1)$ multiplicada por $a^2$ é
$$\dot a^2
= \frac{8 \pi G}{3 c^2} \epsilon a^2 - \frac{kc^2}{R_0^2} \tag{4.1}$$
Derivando, temos:
$$\begin{split}
2 \dot a \ddot a^2
&= \frac{8 \pi G}{3 c^2} (\dot \epsilon a^2 + 2 \epsilon a \dot a)
\\ \frac{\ddot a}{a} &= \frac{4 \pi G}{3 c^2}(\dot \epsilon \frac{a}{\dot a} + 2 \epsilon)
\end{split}$$
E, usando a equação dos fluidos $(3.4)$
$$\begin{split}
\frac{\ddot a}{a} &= \frac{4 \pi G}{3 c^2}(-3(\epsilon + P) + 2 \epsilon)
\\ \frac{\ddot a}{a} &= -\frac{4 \pi G}{3 c^2}(\epsilon + 3P)
\end{split}
\tag{4.2}
$$
Que é chamada de *equação da aceleração*.
## Equação de estado
No momento temos duas equações independentes $(2.1)$ e $(3.4)$ (já que $(4.2)$ é derivada destas) e três variáveis: $a(t), \,\epsilon(t)$ e $P(t)$. Precisamos de alguma equação independente que relacione dois destes fatores, para que possamos deduzi-los. Para isso surge a equação de estado, na forma $P = P(\epsilon)$, que em geral tem a forma
$$P = w \epsilon \tag{5.1}$$
Para gases não relativísticos,
$$w \approx \frac{\langle v^2 \rangle}{3 c^2} \ll 1$$
Onde $\langle v^2 \rangle$ é a velocidade média quadrada das partículas do gás. Mesmo para plasmas, este valor é muito pequeno.

Para gases relativísticos, temos
$$P_{rel} = \frac{1}{3} \epsilon_{rel}$$
Seja para fótons ou para partículas de velocidade quase relativísticas.

O parâmetro $w$ também permite definir a velocidade do som de um fluído:
$$c_s=\sqrt w c\tag{5.2}$$
> $w$ negativo significa oscilações acústicas não estáveis;

Podemos substituir $(5.1)$ em $(4.2)$ para algumas análises:
$$\frac{\ddot a}{a} = -\frac{4 \pi G}{3 c^2}\epsilon (1 + 3 w)$$
Os componentes com $w < -\frac{1}{3}$ nos dão uma aceleração negativa, o que implica num universo cíclico. Os componentes $w = -1$, na equação dos fluidos $(3.4)$ geram $\dot \epsilon = 0$, que são componentes de [[Constante cosmológica]].