# Final Project & Weekly Coding Challenges

- Below is a concise overview along with links to GitHub repositories for the Final Project and weekly challenges.
- Complete documentation for each challenge is available in the respective repository’s README.md file.

---

## Final Project

### AES_Core: Hardware Accelerator for AES Cryptographic Algorithm  
#### GitHub Repository  
- 🔗 [Final_Project](https://github.com/neiltauro/AES_Core-A-Hardware-Accelerator-for-AES-Cryptographic-Algorithm.git)
#### Documentation  
- 🔗 [Doc](https://github.com/neiltauro/AES_Core-A-Hardware-Accelerator-for-AES-Cryptographic-Algorithm/blob/main/doc/Documentation.pdf)   
#### Summary  
- Designed and implemented a hardware accelerator for the AES cryptographic algorithm.  
- The accelerator is developed using SystemVerilog and integrated into a Python-based AES software environment via a wrapper interface.  
- The project accelerates core AES operations such as encryption and decryption by offloading computation to the hardware module.  
- Comprehensive testing includes co-simulation with cocotb and integration with Python scripts to validate functionality and performance.  
- The design emphasizes modularity and aims for synthesizability on FPGA targets.

---

### Challenge #5 – Analyzing and Profiling Python Bytecode  
#### GitHub Repository  
- 🔗 [W01_C05_PyBytecode](https://github.com/neiltauro/HW_for_AI_C5.git)  
#### Summary  
- This effort focuses on identifying the most frequently executed Python bytecode instructions from various scripts and profiling their performance.  
- Sample workloads include:  
  - QuickSort  
  - Crypto
  - Matrix Multiplication  

### Challenge #6 – Perceptron Visualization for Logic Gates  
#### GitHub Repository  
- 🔗 [W02_C06_Perceptron](https://github.com/neiltauro/HW_for_AI_Challange_6_7_8.git)  
#### Summary  
- Implements perceptrons that learn basic logic gates like AND, OR, NAND, and NOR.  
- Separate Python scripts exist for each gate: `Simple_Perceptron_<gate_name>.py`.

### Challenge #7 – Visualizing Perceptron Training  
#### GitHub Repository  
- 🔗 [W02_C07_Perceptron](https://github.com/neiltauro/HW_for_AI_Challange_6_7_8.git)  
#### Summary  
- Visualizes perceptron learning processes using `matplotlib` to display decision boundaries and data points.  
- Each logic gate has an associated visualization script: `visualize_<gate_name>.py`.  
- The repository README contains GIF animations showing the training progress.  
- Created a single-layer perceptron for the XOR gate in `Simple_Perceptron_XOR.py` and its visualization in `Visualize_XOR.py`, demonstrating why XOR isn’t linearly separable.  
- This illustrates the requirement for multi-layer architectures to handle XOR and XNOR gates.

### Challenge #8 – Multi-layer Perceptron for XOR and XNOR Gates  
#### GitHub Repository  
- 🔗 [W02_C08_Perceptron](https://github.com/neiltauro/HW_for_AI_Challange_6_7_8.git)  
#### Summary  
- Demonstrates multi-layer perceptron implementation for learning XOR and XNOR gates.  
- Scripts include `Multi_Layer_Perceptron_XOR.py` and `visualize_multi_XOR.py`.

### Challenge #10 – Detecting Performance Bottlenecks in Frozen Lake Environment  
#### GitHub Repository  
- 🔗 [W03_C10_Frozen_Lake](https://github.com/neiltauro/HW_for_AI_Challenge12_FrozenLake.git)  
#### Summary  
- Investigates computational bottlenecks in the Frozen Lake Q-learning problem.  
- Uses Gymnasium’s Frozen Lake environment and implements Q-learning algorithm.  
- Identifies the `Q-table update` function as the primary bottleneck.
- Python Q-learning implementation  
- Verilog hardware module for Q-value updates
- Hardware-software co-simulation using `cocotb`  
- Benchmark framework comparing hardware and software performance.

### Challenge #12 – Software-only Implementation and Cocotb Testbench Setup  
#### GitHub Repository  
- 🔗 [C12_Frozen_Lake](https://github.com/neiltauro/HW_for_AI_Challenge12_FrozenLake.git)  
#### Summary  
- Started implementing the pure software baseline.  
- Selected `cocotb` as the testbench framework.  

### Challenge #22 – Exploring Neuromorphic Computing Concepts  
#### GitHub Repository  
- 🔗 [C22_Neuromorphic_Computing](https://github.com/neiltauro/HW_for_AI_Challange_22.git)  
#### Summary  
- Studied fundamental principles and applications of neuromorphic computing.  

### Challenge #26 – Utilizing BrainChip’s IP for Edge AI  
#### GitHub Repository  
- 🔗 [C26_BrainChip](https://github.com/neiltauro/HW_for_AI_Challange_26.git)  
#### Summary  
- Investigated BrainChip’s Akida IP for AI at the edge.

### Challenge #28 – Utilizing BrainChip’s IP for Edge AI  
#### GitHub Repository  
- 🔗 [C28_Memristor_Model](https://github.com/neiltauro/HW_for_AI_Challange_28.git)  
#### Summary  
- Modeled and simulated a memristor — a two-terminal electronic component whose resistance evolves based on its history of current flow.
  
