# Shor's Algorithm Tutorial

Now jump back into your qiskit environment again:
```
conda activate ENV_NAME
source ./ENV_NAME/bin/activate
```
And open the second tutorial in your chosen format. Note if you're using the [IBM server](https://quantum-computing.ibm.com/), you can just upload my jupyter notebooks.


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

They build upon eachother to make sure to go through the list sequentially!

# How to use the IBM Cloud Computer

At any time if you want to run some code on the IBM quantum computer, you'll need to do the following. You'll have to create an IBMQ account to do this.
