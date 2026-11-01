# Lecture 01
## Brownian Motion

​$\tau_0$ : time-scale above which motion become uncorrelated

​$\text{d}N$ : Number of observation with change ${}\Delta {}$ from ${}[\Delta,\Delta+\text{d}\Delta]{}$ during ${}\tau_{0}{}$

$$
\text{d}N=Nf(\Delta)\text{d}\Delta
\tag{1}
$$
- Properties of ${}f(\Delta){}$
	- Symmetrical: ${}f(\Delta)=f(-\Delta){}$
	- Normalization: ${}\int_{-\infty}^{\infty}f(n){}$ 

# Lecture 02
## Interlude on Ergodicity
Let's say we have observable ${}B{}$.
We compute average of this observable ${}\langle B\rangle{}$ at a time ${}t{}$
$$
\langle B\rangle = \int_{\text{phase space}}B(\Gamma)f(\Gamma)\text{d}\Gamma
\tag{2}
$$
This is an ensemble average.
We look at how this evolve in time
# Lecture 03
if we want to look at internal energy of the system
$$
U = \langle \hat{\mathcal{H}} \rangle_{eq}=\int \hat{\mathcal{H}}f_{0}^{[N]}dr^Ndp^N
\tag{3}
$$
${}f_{0}^{[N]}{}$ depends on thermodynamics properties of the ensemble

If we want to look at isolated system with constant volume ${}V{}$, ${}N{}$ identical particles
$$
f_{0}^{[N]}(\vec{r}^N,\vec{p}^N) = c \delta[\hat{\mathcal{H}}-E] \hspace{3cm} \text{Microcanonical ensemble } (N,V, E \text{ fixed})
\tag{4}
$$
where, ${}c{}$ : Normalization constant

For a Canonical ensemble (${}N, V, T{}$ fixed), ${}f_{0}^{[N]}{}$ depends on Boltzmann distribution
$$
f_{0}^{[N]}(\vec{r}^N, \vec{p}^N)=\frac{1}{h^{3N}N!} \frac{e^{-\beta \hat{\mathcal{H}}}}{Q_{N}}
\tag{5}
$$
where,
${}h{}$ : Planck's constant
${}N!{}$ : Due to indistinguishable particles
${}Q_{N}{}$ : Canonical Partition function
$$
Q_{N} = \frac{1}{h^{3N}}\int e^{-\beta \hat{\mathcal{H}}} \text{d} \vec{r}^N \text{d}\vec{p}^N
\tag{6}
$$
Equilibrium energy is given by Helmhotz function (minimize free energy)
$$
\begin{align}
F&=U-TS\\
&= -k_{B}T\ln Q_{N}
\end{align}
\tag{7}
$$
In thermodynamics,
$$
U = \frac{\partial}{\partial (\frac{1}{T})}
$$
In statistical mechanics,
$$
U = \frac{1}{h^{3N}N!}\int \hat{\mathcal{H}}e^{-\beta \hat{\mathcal{H}}} \text{d}\vec{r}^N \text{d}\vec{p}^N= - \frac{\partial\ln Q}{\partial \beta }
$$
If ${}\hat{\mathcal{H}}{}$ if of form: ${}\hat{\mathcal{H}}=V_{N}(\vec{r}^N)+V_{N}(\vec{p}^N){}$ ${}i.e.{}$ there is no coupling between position and momenta.

The integral ${}\int \text{d} p^{3N}{}$ in ${}Q_{N}{}$ gives ${}\int e^{- \beta \frac{|p|^2}{2m}}\text{d}\vec{p}=\sqrt{ 2\pi mk_{B}T }{}$ , where ${}\beta=\frac{1}{k_{B}T}{}$.
De Broglie wavelength: ${}\Lambda=\sqrt{ \frac{2\pi \beta T}{m} }{}$.
Now, the partition function is
$$
Q_{N} = \frac{1}{N!} \frac{\mathcal{Z}}{\Lambda^{3N}}
$$
where, ${}\mathcal{Z}$: configuration part of partition function
$$
\mathcal{Z}_{N}= \int e^{-\beta V_{N}(\vec{r}^N)} \text{d}\vec{r}^N
$$
If we look at ideal gas ${}\to{}$ no interaction between particles (${}V_{N}{}$, potential = 0)
$$
\mathcal{Z}_{n}^{\text{id}}=\int \text{d}\vec{r}^N = V^N
$$
where, ${}V^N{}$: Volume of system(Scaled with number of particles)
Canonical Partition function:
$$
Q_{N}^{\text{id}}=\frac{1}{N!} \frac{V^N}{\Lambda^{3N}}
$$
Free energy for ideal gas:
$$
F^{\text{id}} = -k_{B}T\ln Q_{N}= -k_{B}T\ln\left( \frac{1}{N!} \frac{V^N}{\Lambda^{3N}} \right)
$$
Using Stirling formula: ${}\ln(N!)=N\ln N-N{}$ (works for large N)
Thus,
$$
F^{\text{id}} = k_{B}T(\ln(\Lambda^3\rho)-1)
$$
where, ${}\rho{}$ is the density${}\left( \frac{N}{V} \right){}$
Chemical Potential:
$$
\mu^{\text{id}}=k_{B}T\ln(\Lambda^3\rho)
$$
If we go back to system with interacting particles with ${}\hat{\mathcal{H}}=V_{N}(\vec{r}^N)+K_{N}(\vec{p}^N){}$.
We can separate
$$
Q_{N}=Q_{N}^{\text{id}} \frac{\mathcal{Z}_{N}}{V^N}\hspace{3cm}, F=F^{\text{id}}+F^{\text{excess}}
$$ 
where, ${}F^{\text{excess}}{}$ depends on interactions
$$
F^{\text{excess}}=-k_{B}T\ln\left( \frac{\mathcal{Z}_{N}}{V^N} \right)
$$
In literature, we don't talk about ${}F^{\text{id}}{}$ when we talk about free energy.
For internal energy: ${}{}$
$$
\begin{aligned}
U&=U^{\text{id}}+U^{\text{excess}}\\
&=\frac{3}{2}Nk_{B}T+\langle V_{N} \rangle _{{\text{eq}}} \\
&=\frac{3}{2}Nk_{B}T+\frac{1}{\mathcal{Z}_{N}}\int V_{N}(\vec{r}^N)e^{-\beta V_{N}}\text{d}\vec{r}^N
\end{aligned}
$$
${}\langle V_{N} \rangle_{{\text{eq}}}{}$ is in general difficult to calculate 