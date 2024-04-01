# Quantum error mitigation - Zero-Noise Extrapolation (ZNE)
Implementation of unitary folding to achieve zero-noise extrapolation for quantum error mitigation

**Background:**

Quantum computing hardware in the noisy intermediate-scale quantum (NISQ) era is noisy and error-prone, limiting the scope of quantum computations. Therefore, it is necessary to implement some methods to control this error to faciltate practical quantum computing. Quantum Error Mitigation (QEM) is a near-term approach that accepts contemporary hardware noisiness and uses post-processing to reduce noise or to infer the noiseless value.

**Zero-Noise Extrapolation (ZNE):**

Zero-Noise Extrapolation is a popular quantum error mitigation technique that involves performing a set of quantum computations that purposefully scale-up the noise so as to then extrapolate the value of an observable in the zero-noise limit. 

**Contents of this GitHub repository:**

1. Folding_Global.ipynb - this implements Global/Circuit folding for Circuit #1, which is a randomly generated quantum circuit that guarantees the sole result is |0>
2. Folding_Local.ipynb  - this implements Local/Gate folding for Circuit #2, which is manually-created randomly generated quantum circuit. One of its results is |0>
3. Zero_noise_extrapolation__ZNE_.pdf
4. ZNE_circuit_folding.png - This is a result of the Global/Circuit folding ZNE
5. ZNE_gate_folding.png - This is a result of the Local/Gate folding ZNE

**Getting started guide**
1. Open Folding_Global.ipynb or Folding_Local.ipynb on your local machine. I recommend that you use a virtual environment. I used Python 3.12 and Qiskit 1.0.2. A list of package versions is at the bottom of this readme.md
2. Run the Jupyter notebook cells sequentially from the top. There is a table of contents, section headings, and comments throughout the notebook.
3. The final cells create the figures to compare the noisy data against the noiseless data and the extrapolates
4. There is an introductory .pdf regarding the theory of zero-noise extrapolation called Zero_noise_extrapolation__ZNE_.pdf
5. To the best of my knowledge, I have listed all packages that I used below. It is possible that I missed one and that causes the notebook(s) to not run when you try. I apologise for that and I am happy to work with you to figure out which package(s) I did not list.
6. Owing to the noisy nature of the gates and the probabilistic nature of these noisy simulations, it is possible that you cannot exactly reproduce my figures. 

**Result of global/circuit-based ZNE**:

![ZNE](https://github.com/drdren/Quantum-error-mitigation/assets/104710745/395043c2-a915-4809-b5d9-f03db0d181bc)

Using linear, Richardson, and exponential extrapolation. 

**Result of local/gate-based ZNE**:

![ZNE_gate_folding](https://github.com/drdren/Quantum-error-mitigation/assets/104710745/7a899f74-0c74-4e90-8d15-4f3cdd06de75)

Using linear, Richardson, and exponential extrapolation. 

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
