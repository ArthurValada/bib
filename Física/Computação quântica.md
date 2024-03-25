## Algoritmos quânticos
### Algoritmo de Deutsch
Dado $B = \{1,0\}$
O algoritmo diferencia funções $f: B \to B$ entre constante ou balanceada, complexidade $O(N)$
### Algoritmo de Deutsch - Jozsa
Diferencia entre $f: B^n \to B$ com uma operação. Também $O(1)$, equivalente clássico $O(N)$
### Peter Shor
Fatoração de números.

## Complexidade
- Pior caso: $O(f(N))$
- Caso médio: $\Theta (f(N))$
- Melhor caso: $\Omega (f(N))$

P: Polynomial ($<O(N^n)$)
NP: Non deterministic Polynomial (pode se conferir se a resposta está correta em tempo polinomial)
NP completo: matematicamente similar

## Computação quântica
### Qubit, vetores de estado
Vetor (ver [[Vetores no R² e R³]]) de estado num espaço de Hilbert de duas dimensões, **sempre de módulo 1**.

$\left|\frac{i}{\sqrt{2}}\right|^2 = \left(\frac{i}{\sqrt{2}}\right)^* \left(\frac{i}{\sqrt{2}}\right)$

Operações sobre qubits podem ser representadas por matrizes unitárias: $AA^\dagger = I$, $A^\dagger = (A^T)^*$ ou com a notação de Dirac

### Notação de Dirac
Estado:
$|\Psi \rangle = \begin{psmallmatrix}a\\ b\end{psmallmatrix}$
Estados puros:
$|0\rangle = \begin{psmallmatrix}1\\0\end{psmallmatrix}$
$|1\rangle = \begin{psmallmatrix}0\\1\end{psmallmatrix}$
Um vetor de estado é uma composição linear (soma de vetores) das bases (estados puros), com módulo 1.

Outros estados são superposições dos estados puros.

Conjugados: $|\Psi \rangle = \langle \Psi|^*$

### Portas quânticas
Not ou $X:\begin{pmatrix}a\\b\end{pmatrix} \to \begin{pmatrix}b\\a\end{pmatrix}$, matriz de transformação: $\begin{bmatrix}0&1\\1&0\end{bmatrix}$

$Z:\begin{pmatrix}a\\b\end{pmatrix} \to \begin{pmatrix}a\\-b\end{pmatrix}$, matriz de transformação: $\begin{bmatrix}1&0\\0&-1\end{bmatrix}$
H (Hadamard):
$|0\rangle \to \frac{|0\rangle + |1\rangle}{\sqrt{2}}$
$|1\rangle \to \frac{|0\rangle - |1\rangle}{\sqrt{2}}$
$H = \frac{1}{\sqrt{2}} \begin{bmatrix}1&1\\1&-1\end{bmatrix}$
$S = \begin{bmatrix}1&0\\0&i\end{bmatrix}$

### Medições
Uma medida de sistema colapsa superposição num estado específico e põe a leitura num bit clássico.

### Bases e estados
Estado de spins de um átomo em uma direção específica (x, y, z), baseado no experimento de Stem-Gerlach:

![[Pasted image 20230619081741.png|500]]
Expõem os átomos à um campo magnético não uniforme (esperado em azul, obtido em vermelho)

x representa velocidade e não é trivial de medir.

$|0 \rangle$ e $|1 \rangle$ são estados na base z (cima e baixo, respectivamente).

### Mudança de bases para o eixo z
#### Base x
$|+ \rangle = \frac{|0 \rangle + |1 \rangle}{\sqrt{2}}$ (0 na base x)
$|- \rangle = \frac{|0 \rangle - |1 \rangle}{\sqrt{2}}$ (1 na base x)
#### Base y
$|R \rangle = \frac{|0 \rangle + i|1 \rangle}{\sqrt{2}}$ (0 na base y)
$|L \rangle = \frac{|0 \rangle - i|1 \rangle}{\sqrt{2}}$ (1 na base y)

#### Realizando medições
Em sistemas quânticos, medições só são feitas em z. Se usa transformações para realizar medições em outros eixos:

Medição em x de $|\Psi \rangle$: $|0 \rangle \langle +| + |1 \rangle \langle - | \Psi \rangle$ (representação de Haddamard)
Usa-se Haddamard e realiza-se a medição: -H-M-

Medição em y de $|\Psi \rangle$: -Z-S-H-M-

### Múltiplos Qubits
Notação: $|\Psi \rangle \otimes |\Phi \rangle = |\Psi \Phi \rangle$, um estado produto, composição de um sistema $\Psi$ e um sistema $\Phi$ ($\otimes$ simboliza produto tensorial).
Exemplos:
$|0 \rangle \otimes |0 \rangle = \begin{psmallmatrix}1\\0\\0\\0 \end{psmallmatrix} = |00 \rangle$
$|0 \rangle \otimes |1 \rangle = \begin{psmallmatrix}1 \begin{bsmallmatrix}0\\1\end{bsmallmatrix}\\0\begin{bsmallmatrix}0\\1\end{bsmallmatrix} \end{psmallmatrix} = \begin{psmallmatrix}0\\1\\0\\0\end{psmallmatrix} = |01 \rangle$
Ordem de associação de sistemas quânticos: $q_1 \otimes q_0 = |q_1 q_0 \rangle$
Distributiva:
$$\frac{|0\rangle + |1\rangle}{\sqrt{2}} \otimes |1 \rangle = \frac{|0\rangle \otimes |1 \rangle + |1\rangle \otimes |1 \rangle}{\sqrt{2}} = \frac{|01\rangle + |11\rangle}{\sqrt{2}}$$
Para analisar circuitos de múltiplos qubits faz se o mapeamento para cada qubit, usando-se da notação de Dirac.

---

Emaranhamento ou estados de Bell: estado produto que não pode ser obtido por um produto tensorial.  Ver tabela. Este estado pode ser desfeito.

Porta não controlada: `cx`
Porta não duplamente controlada (Toffoli): `ccx` = $q_2 = q_0 \, AND \, q_1$

**Teorema da não clonagem:** não se clona estados não conhecidos.
$\nexists U: U |\phi \psi \rangle = |\psi \psi \rangle$
