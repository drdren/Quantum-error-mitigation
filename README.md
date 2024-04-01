# Quantum error mitigation - Zero-Noise Extrapolation (ZNE)
Implementation of unitary folding to achieve zero-noise extrapolation for quantum error mitigation

**Background:**

Quantum computing hardware in the noisy intermediate-scale quantum (NISQ) era is noisy and error-prone, limiting the scope of quantum computations. Therefore, it is necessary to implement some methods to control this error to faciltate practical quantum computing. Quantum Error Mitigation (QEM) is a near-term approach that accepts contemporary hardware noisiness and uses post-processing to reduce noise or to infer the noiseless value.

**Zero-Noise Extrapolation (ZNE):**

Zero-Noise Extrapolation is a popular quantum error mitigation technique that involves performing a set of quantum computations that purposefully scale-up the noise so as to then extrapolate the value of an observable in the zero-noise limit. 

**Contents of this GitHub repository:**

1. 
2. 

**Installation guide**

1. Open an instance of Conda Prompt. Type:
```
conda create --name <name-of-my-environment>
```
where ```<name-of-my-environment>``` is the user-defined name of the environment

2. Type ```y``` to proceed.
3. Activate the Conda virtual environment by typing:
```python
conda activate name-of-my-environment
```
4. Within this environment, we need to install Python, Qiskit, and other packages. Type in Conda Prompt:
```python
conda create -n myenv python=3.12
pip install qiskit
pip install qiskit-ibm-runtime
pip install qiskit[visualization]
pip install jupyter
pip install qiskit-aer
pip install matplotlib
pip install numpy
pip install scipy
pip install qiskit-experiments
```
5. To open Jupyter Notebook for running and developing the code, type in Conda prompt:
```conda
jupyter notebook path/to/notebook.ipynb
```

**Package versions**

```
ibm-cloud-sdk-core        3.19.2
ibm-platform-services     0.53.0
jupyter                   1.0.0
jupyter_client            8.6.1
jupyter-console           6.6.3
jupyter_core              5.7.2
jupyter-events            0.10.0
jupyter-lsp               2.2.4
jupyter_server            2.13.0
jupyter_server_terminals  0.5.3
jupyterlab                4.1.5
jupyterlab_pygments       0.3.0
jupyterlab_server         2.25.4
jupyterlab_widgets        3.0.10
matplotlib                3.8.3
matplotlib-inline         0.1.6
numpy                     1.26.4
pip                       23.3.1
qiskit                    1.0.2
qiskit-aer                0.13.3
qiskit-experiments        0.6.0
qiskit-ibm-runtime        0.22.0
qtconsole                 5.5.1
rustworkx                 0.14.2
scipy                     1.12.0
symengine                 0.11.0
```
