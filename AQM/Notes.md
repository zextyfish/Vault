Chapter 01
#### Perturbation Theory
- Analyses spectral properties of system described by a Hamiltonian ${}\hat{\mathcal{H}_{0}}{}$ (unperturbed) under the influence of an additional force or potential (perturbation(${}V{}$)).
- The solution to eigenvalue problem defined by ${}\hat{\mathcal{H}_{0}}{}$ is known ${}\textit{i}.\textit{e}.{}$ it's discrete (harmonic Oscillator) or continuous (finite potential well) spectrum.
- To which extent the physical properties encoded in eigenvalues/eigenstates of ${}\hat{\mathcal{H}_{0}}{}$ are robust under the influence of ${}V{}$.
$$
\hat{\mathcal{H}}=\hat{\mathcal{H}_{0}}+V \hspace{3cm} \text{or} \hspace{3cm} \hat{\mathcal{H}}=\hat{\mathcal{H}_{0}}+\lambda V \label{eq:12}[1.2]
$$
${}\hat{\mathcal{H}_{0}}{}$: Unperturbed System
${}V{}$: Perturbation
${}\lambda{}$: Parameter defining Strength of Perturbation
Remark: Perturbation theory not only relevant for Quantum Mechanics but also for Advanced Classical Mechanics (Canonical Perturbation Theory).
##### 1.1 Time-Independent Perturbation Theory
Given the known system Hamiltonian(${}\hat{\mathcal{H}_{0}}{}$), with
$$
\hat{\mathcal{H}_{0}}\ket{E_{j}^{0}}=E_{j}^0\ket{E_{j}^0} \hspace{3cm} j=1,2\cdots % \label{eq:unperturbedhamiltonian}
\tag{2}
$$
Now perturb the system by a (weak, in some sense) perturbation ${}V{}$, with strength parameterized by a scalar ${}\lambda{}$. To get the new hamiltonian
$$
\hat{\mathcal{H}}=\hat{\mathcal{H}_{0}}+\lambda V
\tag{3}
$$
For ${}\lambda{}$ sufficiently small, we make perturbative ansatz for eigenvalues and eigenvectors.
$$
\begin{align}
\begin{split}
\ket{E(\lambda)} = \ket{E_{a}^0} + \lambda \ket{1} + \lambda^2\ket{2} + \cdots 
\\
E(\lambda)=E_{a}^0+ \lambda \epsilon_{1} + \lambda^2\epsilon_{2} + \cdots
\end{split}
\end{align}
\tag{4}
$$
Here, the label ${}_{a}{}$ identifies the state we are interested in from within the set ${}\{E_{j}^0\}{}$ from ${}\eqref{eq:unperturbedhamiltonian}{}$

# Lecture 03
Wed 28 Oct
### Non-Degenerate Perturbation Theory
${}E(\lambda)\to E_{a}^0{}$
${}\ket{E(\lambda)}\to \ket{E_{a}^a}, \text{for } \lambda \to 0{}$
This ensures smoothness
$$
\ket{1} = \sum_{i \neq a}\frac{\bra{E_{i}^0} V|\ket{E_{a}^0} }{E_{a}^0-E_{i}^0}\ket{E_{i}^0}
\label{TransitionMatrix}[1.12]
$$

${}\bra{E_{i}^0}V\ket{E_{a}^0}{}$: Transition Matrix element from ${}\hat{\mathcal{H}_{0}}{}$ to perturbative system
To derive ${}V{}$-derived( Perturbation-induced) shifts of eigenvalues we insert
# Lecture 04
### 1.1.1 Degenerate Perturbation Theory
EIgenspace of ${}E_{A}^0{}$ with dimension larger than one.
Need to determine
$$
\lim_{ \lambda \to 0 }\ket{E(\lambda)=\ket{E_{a}^0}}\label{eq:21}[1.21]
$$
___
$$
\hat{\mathcal{H}_{0}}\ket{E_{a}^0 m} =E_{a}^0\ket{E_{a}^0 m} \qquad  \forall \quad  m =1,\ldots,N \label{eq:22}
$$
Here, ${}N{}$ is dimensions of degenerate eigenspace
Define ${}\hat{Q}{}$ (Orthogonal to ${}\hat{P}{}$) as projector upon degenerate subspace
$$
\hat{Q}=\sum_{i=1}^{N}\ket{E_{a}^0 m} \bra{E_{a}^0 m} \label{eq:23}
$$
$$
\begin{aligned}
\hat{Q} \ket{E_{a}^0} &=\ket{E_{a}^0} \\ \hat{Q}(H-E_{a}^0)&=0 \label{eq:24}
\end{aligned}
$$
$$
\begin{aligned}
\hat{Q}(H-E_{a}^0)&=\hat{Q}\sum E_{j}^0\ket {E_{j}^0} \bra{E_{j}^0} - \hat{Q}E_{a}^0 \\ \\
 &= \sum_{i=1}^N \ket{E_{a}^0 m} \bra{E_{a}^0 m} \sum_{j}E_{j}^0 \ket{E_{j} }\bra{E_{j}} -QE_{a}^0 \\
 &=\sum^N \ket{E_{a}^0 m} E_{a}^0 \bra{E_{a}^0 m} -QE_{a}^0 \\
 &=0   
\end{aligned}
$$
To distill out decomposition of ${}\ket{E_{a}^0}{}$ (from ${}\eqref{eq:21}$) into the ${}\ket{E_{a}^0 m}{}$, at first order ${}\lambda{}$, project on the first order contribution (see page 10 in manuscript) on degenerate subspace.
$$
\begin{aligned}
\lambda^1:\qquad  \lambda \epsilon_{1}\ket{E_{a}^0} &=\lambda H_{0}\ket{1} +\lambda V \ket{E_{a}^0} -\lambda E_{a}^0 \ket{1}  \\
 0&=(H_{0}-E_{a}^0)\ket{1} +(V-\epsilon)\ket{E_{a}^0}
\end{aligned}
$$
${}\hat{Q}{}$ from left:
$$
\begin{aligned}
\hat{Q}(\hat{\mathcal{H}_{0}}-E_{a}^0)\ket{1} + \hat{Q}(V-\epsilon_{1})\ket{E_{a}^0} &=0 \\
\hat{Q}((V-\epsilon_{1})\ket{E_{a}^0})&=0 \\
\hat{Q}(V-\epsilon_{1})\hat{Q}\ket{E_{a}^0} &=0 
\end{aligned}
$$
Filter out ${}\ket{E_{a}^0 m}{}$ components:
$$
\bra{E_{a}^0 m} \hat{Q}(V-\epsilon_{1})\hat{Q}\ket{E_{a}^0} =0 \qquad , \ \forall\quad m=1,\ldots,N
$$
Here ${}\epsilon_{1}{}$ still to be determined. Plugging in ${}\hat{Q}{}$:
$$
\bra{E_{a}^0 m} \sum_{N}\ket{E_{a}^0 n} \bra{E_{a}^0 n}(V-\epsilon_{1})\sum_{l}\ket{E_{a}^0 l} \braket{ E_{a}^0 l\vert E_{a}^0 } = 0     
$$
In shortcut notation:
$$
V_{ml}^Q \coloneqq \braket{E_{a}^0 m \vert V \vert E_{a}^0 l    } \label{eq:25} 
$$
Then above equation becomes:
$$
\begin{aligned}
\sum_{l=1}^N(V_{ml}^Q-\delta_{ml}\varepsilon_{1})\braket {E_{a}^0l\vert E_{a}^0}&=0\qquad ,\forall \quad m=1,\ldots,N  \\
\text{or,} \qquad (V_{ml}^Q-\varepsilon_{1} \mathbb{1}) \begin{pmatrix}
\braket{ E_{a}^0 \mathbb{1}\vert E_{a}^0  } \\
\vdots \\
\braket{ E_{a}^0 N | E_{a}^0 } 
\end{pmatrix}&=0\label{eq:26}
\end{aligned}
$$
${}\eqref{eq:26}$ has non-trivial solutions if the 
$$
{}\det(V^Q-\varepsilon_{1}\mathbb{1}){}=0\label{eq:27}
$$
vanishes ${}i.e.{}$ for ${}V^Q{}$ diagonal, with eigenvalues ${}\varepsilon_{1}{}$ as
###### First order Correction to ${}E_{a}^0{}$
If there are ${}N{}$ distinct eigenvalues,${}\qquad \varepsilon_{1}^m\qquad m=1,\ldots,N{}$ 
the degeneracy of ${}E_{a}^0{}$ is fully lifted by the perturbation
If there are less than ${}N{}$ distinct eigenvalues; proceed to next higher orders.
The eigenvector associated with ${}\varepsilon_{1}{}$ (provided eigenvalue is distinct) give the sought after expansion of ${}E_{a}^0{}$.
##### 1.1.2 Hellmann-Feynman Theorem
- Useful statement on perturbation induced shift of eigenvalues of the ${}\hat{\mathcal{H}}{}$ (from ${}\eqref{eq:12}{}$, with hold irrespective of strength ${}\lambda{}$ of perturbation, and also helps to build intuition of what ${}V{}$ does to eigenstates of ${}\hat{\mathcal{H}_{0}}{}$.
Let ${}\hat{\mathcal{H}}{}$ be time independent (autonomous) parametrized by real (scalar) ${}\lambda$
$i.e.$  $\hat{\mathcal{H}}=\hat{\mathcal{H}}(\lambda){}$  with associated parameterized eigenvalues and eigenvectors determined by

