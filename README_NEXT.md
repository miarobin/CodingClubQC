# A Pair of Complicated Algorithms

Now jump back into your qiskit environment again:
```
conda activate ENV_NAME
source ./ENV_NAME/bin/activate
```
And open the second tutorial in your chosen format. Note if you're using the [IBM server](https://quantum-computing.ibm.com/), you can just upload my jupyter notebook.

Here are two algorithms which you can build & run on the IBM quantum computer:
1. The prime factorisation algorithm.
2. Quantum error correction.
Choose one to start with (order doesn't matter).

## 1. The Prime Factorisation Algorithm.
This tutorial is going to run you through Shor's factorisation algorithm. Essentially, you can use a quantum computer to speed up factorisation to polynomial time, from the best known classical algorithm which runs in super-polynomial time (i.e. time is not bounded by any polynomial).

The prime factorisation algorithm essentially boils down to the following things:/
a) Quantum Phase Estimation/
```
jupyter notebook quantum_phase_estimation.ipynb
```
b) Quantum Fourier Transform/
```
jupyter notebook quantum_fourier_transform.ipynb
```
c) Period Finding/
```
jupyter notebook period_finding.ipynb
```

## 2. Quantum Error Correction.


