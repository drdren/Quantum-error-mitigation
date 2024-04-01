# Quantum error mitigation - Zero-Noise Extrapolation (ZNE)
Implementation of unitary folding for quantum error mitigation

Background: 
Quantum computing hardware in the noisy intermediate-scale quantum (NISQ) era is noisy and error-prone, limiting the scope of quantum computations. Therefore, it is necessary to implement some methods to control this error to faciltate practical quantum computing. Quantum Error Mitigation (QEM) is a near-term approach that accepts contemporary hardware noisiness and uses post-processing to reduce noise or to infer the noiseless value.

Zero-Noise Extrapolation (ZNE):
Zero-Noise Extrapolation is a popular quantum error mitigation technique that involves performing a set of quantum computations that purposefully scale-up the noise so as to then extrapolate the value of an observable in the zero-noise limit. 

