## Métricas de superfícies
Num plano, a distância infinitesimal $ds$ entre dois pontos pode ser representada por
$$ds^2 = dx^2 + dy^2 \tag{1.1}$$
Usando as coordenadas retangulares $(x,y)$. Mas usando as coordenadas polares $(r, \theta)$, temos
$$ds^2 = dr^2 + r^2d\theta^2 \tag{1.2}$$
Nesta equação temos a variação do componente radial $dr$ e a variação do comprimento de arco $rd\theta$, ambos ao quadrado.

Ambas as equações podem ser usadas para descrever a curvatura de uma superfície, e são chamadas de *métricas*. Um espaço plano possui curvatura nula.

Para superfícies curvas, com *curvatura positiva*, i.e. um espaço esférico com área limitada, fechado sobre si, em que é possível "circunavegar" o espaço, a distância entre dois pontos vai ser expressa como
$$ds^2 = dr^2 + R^2 sen^2(r/R) d\theta^2 \tag{1.3}$$
Nesta expressão, as distâncias radiais permanecem as mesmas, no entanto, os arcos, ao invés de serem proporcionais ao raio, vão ter um termo de escala da esfera $R sen(r/R)$. Tomando $r<\pi R$ (para a distância ficar no mesmo hemisfério), o termo de escala vai variar entre $0$ a $\pi$ como uma onda senoide, assim, os objetos a $\pi/2$ vão ter maiores valores.

Nesta equação, $r$ é a distância do ponto a um polo qualquer (origem) e $\theta$ é o ângulo entre algum meridiano qualquer. Enfatizo que $r$ é uma distância, por isso chamamos isto de coordenada polar.

Para superfícies com *curvatura negativa*, que possuem área infinita (área mais infinita do que é possível se representar no nosso espaço razoavelmente plano), a equação é bem similar, com o termo de escala usando o seno hiperbólico:
$$ds^2 = dr^2 + R^2 senh^2(r/R)d \theta \tag{1.4}$$
Por conta disso, essas superfícies as vezes são chamadas de espaços hiperbólicos, em contrapartida aos planos e esféricos. O termo de escala $R^2 senh^2(r/R)$ cresce de forma exponencial de acordo com o valor de $r$, de modo que arcos distantes vão parecer enormes.

Lembrando que curvatura é uma propriedade local. Para aplicar as métricas apresentadas para um espaço todo, precisamos assumir que ele seja [[Fundamentos da cosmologia#Em largas escalas o universo é isotrópico e homogêneo|homogêneo e isotrópico]].
## Métricas de espaços
Para espaços planos de 3 dimensões, a métrica retangular é
$$ds^2 = dx^2 + dy^2 + dz^2 \tag{2.1}$$
Aqui, podemos usar as coordenadas esféricas
$$ds^2 = dr^2 + (rd\theta)^2 + (rsen\theta d \phi)^2$$
Ou, de forma mais comum,
$$ds^2 = dr^2 + r^2(d\theta^2 + sen^2\theta d \phi^2)$$
Aqui definimos $\theta$ como o ângulo entre $r$ e o eixo $z$ e $\phi$ o ângulo no plano $xy$ partindo do eixo $x$. Por causa da projeção do arco paralelo a $\phi$ passando no ponto, o que requer uma escala, temos $rsen\theta d \phi$ ao invés do esperado $r d \phi$.

Isso fica claro se tomarmos $r$ e $\theta$ constantes, de modo que $ds^2 = (r sen \theta d \phi)^2$:  o arco projetado no eixo $xy$ não vai ter o comprimento $rd\phi$, já que a projeção vai fazer a distância ser $r sen \theta$.

As equações para espaços com curvaturas não nulas vão fazer o mesmo processo de adicionar um fator de escala $Rsen(r/R)$ ou $Rsenh(r/R)$ no $r$ constante da métrica esférica, de modo que podemos criar uma função de escala
$$
S_k(r) = \begin{cases}
Rsen(r/R), & (k=+1)\\
r, & (k=0)\\
Rsenh(r/R),& (k=-1)
\end{cases}
$$
Onde $k$ é o sinal da curvatura do espaço. A curvatura positiva, nula e negativa, dão a $k$, respectivamente os valores de $+1, 0, -1$.

Também podemos usar o ângulo sólido, ao invés de dois ângulos:
$$d\Omega^2 \equiv (d\theta^2 + sen^2\theta d \phi^2)$$
Dessa forma, podemos representar qualquer espaço de curvatura homogênea e isotrópica como
$$ds^2 = dr^2 + S_k(r)^2d\Omega^2 \tag{2.2}$$
Se definirmos $x \equiv S_k(r)$, podemos substituir $S_k(r)$ por uma única expressão:
$$ds^2 = \frac{dx^2}{1-kx^2/R^2} + x^2d\Omega^2 \tag{2.3}$$ 
## As métricas de Minkowski e de Friedman-Lamaître-Robertson-Walker
Na *Teoria da Relatividade Especial*, o espaço é indissociável tempo, então ao invés de pontos num espaço, falamos de eventos no *espaço-tempo*, e usamos coordenadas $(t, r, \theta, \phi)$. A *separação* de dois eventos no espaço-tempo é dada pela *métrica de Minkowski*:
$$ds^2 = -c^2 dt^2 + dr^2 + r^2d\Omega^2 \tag{3.1}$$
Veja que ela assume um espaço-tempo plano, euclidiano, assim, não considera curvaturas no espaço-tempo, o que só ocorre na Relatividade Especial. Além disso, o tempo tem valor negativo pois partículas viajando na velocidade da luz possuem geodésias nulas, i.e., $ds=0$, o que significa que elas viajam apenas no espaço, não no tempo, de modo que
$$0 = -c^2 dt^2 + dr^2 + r^2d\Omega^2$$
E, para um caminho linear, radial, temos
$$
0 = -c^2 dt^2 + dr^2
$$
$$
c^2 dt^2 = dr^2 \implies \frac{dr}{dt} = c \tag{3.2}
$$

Alexander Friedmann, Georges Lemaître, Howard Robertson e Arthur Walker desenvolveram independentemente uma métrica que leva em conta a expansão do universo, considerando ele ainda homogêneo e isotrópico (o que não tinha muitas evidências na época, mas é mais fácil de calcular). O resultado foi a *métrica de Friedmann-Lemaître-Robertson-Walker* (métrica de FLRW), as vezes chamada de modelo padrão da cosmologia:
$$ds^2 = -c^2 dt^2 + a(t)^2[dr^2 + S_k(r)^2d\Omega^2] \tag{3.3}$$
No espaço de Robertson-Walker, a variável $t$ é o tempo cosmológico ou *tempo cósmico* e as coordenadas $(r, \theta, \phi)$ são as coordenadas *co-móveis*, que permanecem as mesmas, com a expansão do universo. Isso tudo assumindo homogeneidade e isotropia. Isto permite que descrevamos toda a geometria do universo com apenas 3 valores: $a(t), k$ e $R_0$.

Independente da expressão de $a(t)$, seu valor é normalizado para $1$ no presente, e $R_0$ é a curvatura do espaço no presente.

A distância de dois objetos em um dado espaço de tempo pode ser medida sabendo o instante de emissão $t_e$ e o de observação $t_0$ e integrando a equação da geodésia $(3.2)$ para a métrica de FLRW. Esta distância é chamada de *distância própria*:
$$c\int_{t_e}^{t_0}\frac{dt}{a(t)}=\int_0^rdr=d_p(t_0) \tag{3.4}$$

O fator de escala $a(t)$ pode se relacionar com a [[Fundamentos da cosmologia#Galáxias possuem redshift proporcional a suas distâncias|constante de Hubble]] uma vez que $(2.2)$ nos diz que $v = H_0 r$, e usando as distâncias co-móveis, temos
$$\dot a = H_0 a$$
ou
$$H_0 = \left(\frac{\dot a}{a}\right)_{t=t_0} \tag{3.5}
$$
Além disso, elas nos permitem deduzir o crescimento do espaço $a(t_e)$ que um objeto estava experienciando quando emitiu sua luz, por meio do seu redshift (considerando que a escala atual $a(t_0) = 1$):
$$1 + z = \frac{1}{a(t_e)} \tag{3.6}$$