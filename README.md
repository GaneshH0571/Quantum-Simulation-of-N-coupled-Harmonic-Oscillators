# Quantum-Simulation-of-N-coupled-Harmonic-Oscillators

A Quantum computer is a specialized computer that uses quantum bits instead of normal bits.
This makes a quantum computer a natural tool to carry out simulation of quantum system as this
problem is too difficult to solve on a classical computer. In this report, we establish two schemes
to simulate bosonic systems like the quantum harmonic oscillator on a quantum computer. We
will also be looking at an algorithm to map the exponential of a Hamiltonian, which is a linear
combination of Pauli operators to single qubit and two qubit gates. And finally, we will simulate
a system of coupled oscillators and analyze the results of the simulation by plotting expectation
values of observables such as position, momentum, and energy.

# Conclusion from Code

The simulation of bosonic systems such as the coupled quantum harmonic oscillator on a quantum
computer requires a truncation of the energy spectrum, this truncation does not decrease the accuracy
of any expectation values we choose to compute, but it just puts a restriction of the maximum possible
energy, so if our bosonic system of interest only takes takes certain finite energy values, then it can be
simulated accurately on a quantum computer. Once we have the spectrum of truncated occupation
number spectrum, we can map these eigen states and the Hamiltonian to a system of qubits, there
are various ways of doing the same. In this report we looked at two kinds of encoding schemes, one
hot and gray code. While one hot encoding is simple to understand and implement, the results make
it clear that gray code encoding is superior both in terms of time taken and depth of the resultant
circuit. And finally the simulation can be carried out by simply computing the time evolution operator
(for the case of time independent Hamiltonian) , we have also shown a way to construct the time
evolution operator as single and two qubit gates by Trotterizing it given that H is mapped onto a
linear combination of Pauli operators. Once the time evolution operator is obtained, we can compute
the states of system at any time and compute various expectation values to study the properties we
desire.
