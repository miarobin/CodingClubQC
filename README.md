# CodingClubQC
See the preceeding presentation [here](https://github.com/miarobin/CodingClubQC/blob/main/VeryBasicQuantumComputing.pdf).
See a guide to quantum gates HERE.

## Instructions for Qiskit
Now that you've all seen the above presentation, these are some simple instructions to work qiskit. 

### Option 1 : The Qiskit Server
1. Go [here](https://quantum-computing.ibm.com/).
2. Click the 'IBMid' button & follow the steps to create an account.
3. Once you're in, you can:   
    a) Launch the *'IBM Quantum Composer'* and make circuits using their visual tool.\
    b) Launch the *'IBM Quantum Lab'* which is essentially just a jupyter notebook.
4. If you want to go through the example, go to *'Getting Started With Qiskit'*.\
   If you want to create your own notebook, click*'Qiskit v___ (ipykernel)'*. 

### Option 2 : Download Qiskit in a Virtual Environment
1. Create a minimal python 3 environment with only python installed, by typing into the terminal:/
    a) With **anaconda**:
    ```
    conda create -n ENV_NAME python=3
    conda activate ENV_NAME
    ```
    b) With **venv**:
    ```
    python3 -m venv ENV_NAME
    source ./ENV_NAME/bin/activate
    ```
2. Install qiskit package with pip:
    ```
    pip install qiskit                    *standard installation*
    pip install qiskit[visualization]     *if you want fancy graphics*
    pip install 'qiskit[visualization]'   *if you're on MacOS*
    ```
3. Clone this github repository 
    ```
    git clone git@github.com:miarobin/CodingClubQC.git
    ```
4. Decide if you'd like to use the Jupyter notebook (a) or the python script (b):\
   a) **Jupyter Notebook** - All graphs/circuit diagrams are produced & shown in the notebook.
   ```
   jupyter notebook part1_notebook.ipynb
   ```
   If you'd like the qiskit notebook, which is much more detailed in explaining each step, you can find it [here](https://github.com/Qiskit/qiskit-tutorials/blob/master/tutorials/circuits/1_getting_started_with_qiskit.ipynb).\
   b) **Python Script** - All graphs/circuit diagrams are saved as pdf's.
   ```
   python3 scriptTutorial.py
   ```

Now you're done! You may quantum compute to your heart's content. 


## Build a Toffoli Gate
To build your own Toffoli gate with only two qubit gates:
```
jupyter notebook part2_notebook.ipynb
```
