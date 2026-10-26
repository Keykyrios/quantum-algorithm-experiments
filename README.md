# Quantum Algorithm Experiments

Lab assignment for an undergraduate Quantum Technologies course, submitted on 8 April 2026. The work involved implementing and running six quantum algorithms — first on a local simulator (Qiskit Aer), then on real hardware through the IBM Quantum Platform.

## What's in this repo

This repository contains **reports and execution evidence only**, not source code. The original Python/Qiskit scripts used to build and run the circuits are not available.

### Main report

[`Quantum_Algorithms_Simulation_and_IBM_Hardware_Execution.pdf`](Quantum_Algorithms_Simulation_and_IBM_Hardware_Execution.pdf) — The full lab report covering all six algorithms:

| Algorithm | Contents |
|---|---|
| Deutsch | Circuit diagram, simulated and IBM outputs |
| Deutsch-Jozsa | Circuit diagram, simulated and IBM outputs |
| Bernstein-Vazirani | Circuit diagram, simulated and IBM outputs |
| Simon's | Circuit diagram, simulated and IBM outputs, classical equation-solving step |
| Grover's | Circuit diagram, simulated and IBM outputs, measurement histograms |
| Shor's | Input-generation output, simulated and IBM outputs, measurement histograms |

Each section shows side-by-side screenshots of the circuit/output from local simulation and from IBM Quantum.

### IBM execution reports

Individual PDFs captured from the IBM Quantum Platform, documenting job status, transpiled circuit views, shot counts, and measurement probability distributions.

| File | Algorithm | Backend |
|---|---|---|
| [`reports/deutsch-ibm.pdf`](reports/deutsch-ibm.pdf) | Deutsch | IBM Quantum |
| [`reports/deutsch-jozsa-ibm.pdf`](reports/deutsch-jozsa-ibm.pdf) | Deutsch-Jozsa | IBM Quantum |
| [`reports/bernstein-vazirani-ibm.pdf`](reports/bernstein-vazirani-ibm.pdf) | Bernstein-Vazirani | IBM Quantum |
| [`reports/simons-ibm.pdf`](reports/simons-ibm.pdf) | Simon's | IBM Quantum |
| [`reports/grovers-ibm.pdf`](reports/grovers-ibm.pdf) | Grover's | IBM Quantum |
| [`reports/shors-ibm.pdf`](reports/shors-ibm.pdf) | Shor's | IBM Quantum |

Some jobs ran on `ibm_fez` and `ibm_kingston` backends. The reports show completed execution status along with measurement distributions.

## Notes

- All circuits were executed using IBM Quantum's free-tier access with default shot counts.
- Results from real hardware include noise and decoherence effects, so outputs differ from ideal simulation — this is expected and discussed in the report.
- No claim is made about quantum advantage or large-scale factoring; Shor's algorithm was run on a small example for demonstration purposes.
