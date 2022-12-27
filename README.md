#Quantum = 
10 lines of code to hack BTC with a quantum computer.

![image](https://user-images.githubusercontent.com/51065039/209723930-4aa51a81-6ca8-42d1-92cb-21819683f163.png)


//
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
//
