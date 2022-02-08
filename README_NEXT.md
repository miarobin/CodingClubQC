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

### Configure your IBM Quantum credentials

1. Create an IBM Quantum account or log in to your existing account by visiting
   the [IBM Quantum login page].

2. Copy (and/or optionally regenerate) your API token from your
   [IBM Quantum account page].

3. Take your token from step 2, here called `MY_API_TOKEN`, and run:

   ```python
   from qiskit import IBMQ
   IBMQ.save_account('MY_API_TOKEN')
   ```

   The command above stores your credentials locally in a configuration file called `qiskitrc`.
   By default, this file is located in `$HOME/.qiskit`, where `$HOME` is your home directory. If
   you are still using `Qconfig.py`, please delete that file and run the command above.

### Accessing your IBM Quantum backends

After calling `IBMQ.save_account()`, your credentials will be stored on disk.
Once they are stored, at any point in the future you can load and use them
in your program simply via:

```python
from qiskit import IBMQ

provider = IBMQ.load_account()
backend = provider.get_backend('ibmq_qasm_simulator')
```

Alternatively, if you do not want to save your credentials to disk and only
intend to use them during the current session, you can use:

```python
from qiskit import IBMQ

provider = IBMQ.enable_account('MY_API_TOKEN')
backend = provider.get_backend('ibmq_qasm_simulator')
```
