#Quantum-BTC-run = 
** USE OF THIS INTELLECTUAL PROPERTY = SELF-DAMAGES ** DO NOT USE **
THE FOLLOWING ARE 10 lines of code to hack BTC with a quantum computer.
THE USER CAN BE TRACED, SO EVEN IF YOU GET YOUR HANDS ON A Q-COMPUTER, I WOULD NOT USE THIS CODE IF I WERE YOU.
THE CODE PRESENTED HERE IS PRESENTED TO PROVE THAT IT CAN BE DONE, THE GOVERNMENT/BANKERS CAN DO THIS NOW = WHO CURRENTLY OWNS/OPERATES/ACCESSES QUANTUM COMPUTERS?=short-list.
IF AN AMATURE CODER CAN FIGURE THIS OUT, WHAT DO YOU THINK THE GOVERNMENT SYSTEM CODING ENGINEERS ARE CAPABLE OF?

![image](https://user-images.githubusercontent.com/51065039/209723930-4aa51a81-6ca8-42d1-92cb-21819683f163.png)

from qiskit.aqua.algorithms import Shor
from qiskit.aqua. import QuantumInstance
from qiskit import Aer
key = 21
base = 2
backend = Aer.get_backend('qasm_simulator')
qi = QuantumInstance(backend=backend, shots=1024)
shors = Shor(N=key, a=base, quantum_instance=qi)
results = shors.run()
print(results['factors'])
