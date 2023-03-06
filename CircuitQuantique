from qiskit import QuantumCircuit, execute, Aer

# Créer un circuit quantique avec un qubit
qc = QuantumCircuit(1, 1)

# Appliquer une porte de Hadamard au qubit
qc.h(0)

# Mesurer le qubit
qc.measure(0, 0)

# Exécuter une simulation de mesure avec un simulateur de Qiskit
backend = Aer.get_backend('qasm_simulator')
job = execute(qc, backend, shots=1000)
result = job.result()

# Afficher les résultats de la simulation
print(result.get_counts(qc))
