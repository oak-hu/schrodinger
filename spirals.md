# Schrödinger Spirals

We visualise the quantum mechanics of a particle that lives on the real line \(\mathbb R\).

The _wavefunction_ \(\psi:\mathbb R\to(\mathbb R\to \mathbb C)\) maps each time \(t\) to a _state_ \(\psi(t): \mathbb R \to \mathbb C\), which in turn assigns a value in the complex plane \(\mathbb C\) for each location in \(\mathbb R\). The squared magnitude \(|\psi(t)(x)|^2\) of the value assigned to a location \(x\) represents the particle's density there, such that integrating over a region of \(\mathbb R\) and normalising gives the probability of measuring the particle in that region. The wavefunction must then, more specifically, map each time to an element of the Hilbert space \(L^2(\mathbb R, \mathbb C)\) of _square-integrable functions_ from \(\mathbb R\) to \(\mathbb C\); this Hilbert state is our _state space_.

For any state, we can draw a path (call it a "Schrödinger spiral") through the complex plane by plotting the value assigned by that state to each location in \(\mathbb R\). Typically, this path "starts" and "ends" at zero.

The Schrödinger equation governs how the value (in state space) of \(\psi\) changes over time:

\[\dot\psi(t) = i\left(\frac{\hbar(\psi(t))''}{2m} - \frac{ V \cdot \psi(t)}{\hbar}\right)\]

In effect, each state \(\psi(t)\) moves to \(\psi(t+\varepsilon)\) by rotating in the state space, at a rate which positively on the spatial concavity of the state \(\psi(t)\) divided by the mass of the particle, but negatively on the potential energy \(V:\mathbb R\to\mathbb R\) multiplied (pointwise) by the state. Thus, the wavefunction is Markovian in the sense that the history preceding a state does not affect how that state will evolve. But unlike with real-valued _diffusion_, the _preceding_ states are also fully determined by the present state! Thus, the above simulations work in reverse as well. (Note that the rotation in state space is not in general a rotation of each of its output values—these are the same if and only if the density function is constant over time.)

The first animation shows how states evolves by plotting their Schrödinger spirals \(\psi(t)([-1,1])\subset\mathbb C\). The second animation shows how the density \(|\psi(t)[(x)]|^2\) of the particle over the region \([-1,1]\subset \mathbb R\) changes over time.
