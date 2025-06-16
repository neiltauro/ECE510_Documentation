# Final Project & Weekly Coding Challenges

- Below is a concise overview along with links to GitHub repositories for the Final Project and weekly challenges.
- Complete documentation for each challenge is available in the respective repository’s README.md file.

---

## Final Project

### AES_Core: Hardware Accelerator for AES Cryptographic Algorithm  
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
- 🔗 [W02_C06_Perceptron](https://github.com/neiltauro/HW_for_AI_C5.git)  
#### Summary  
- Implements perceptrons that learn basic logic gates like AND, OR, NAND, and NOR.  
- Separate Python scripts exist for each gate: `Simple_Perceptron_<gate_name>.py`.

### Challenge #7 – Visualizing Perceptron Training  
#### GitHub Repository  
- 🔗 [W02_C07_Perceptron](https://github.com/A-m-e-y/W02_C06_Perceptron)  
#### Summary  
- Visualizes perceptron learning processes using `matplotlib` to display decision boundaries and data points.  
- Each logic gate has an associated visualization script: `visualize_<gate_name>.py`.  
- The repository README contains GIF animations showing the training progress.  
- Created a single-layer perceptron for the XOR gate in `Simple_Perceptron_XOR.py` and its visualization in `Visualize_XOR.py`, demonstrating why XOR isn’t linearly separable.  
- This illustrates the requirement for multi-layer architectures to handle XOR and XNOR gates.

### Challenge #8 – Multi-layer Perceptron for XOR and XNOR Gates  
#### GitHub Repository  
- 🔗 [W02_C08_Perceptron](https://github.com/A-m-e-y/W02_C06_Perceptron)  
#### Summary  
- Demonstrates multi-layer perceptron implementation for learning XOR and XNOR gates.  
- Scripts include `Multi_Layer_Perceptron_XOR.py` and `visualize_multi_XOR.py`.

#### Additional Slack Challenges  
- Developed perceptrons with multiple outputs:  
  - Single-layer, multi-output perceptron (`Simple_Perceptron_Multi_Gates.py`)  
  - Multi-layer, multi-output perceptron (`Multi_Layer_Perceptron_All_Gates.py`)

### Challenge #9 – Final Project: CNN Digit Recognition for 240x240 Images  
#### Summary  
- Selected final project topic: “CNN Digit Recognizer for 240x240 resolution images.”  
- Completed answers to Helmier’s questions in a document.  
- Began software-only implementation phase.  
- For progress updates, see the [Project Journal](project_journal.md).

---

## Week 3

### Challenge #10 – Detecting Performance Bottlenecks in Frozen Lake Environment  
#### GitHub Repository  
- 🔗 [W03_C10_Frozen_Lake](https://github.com/A-m-e-y/W03_C10_Frozen_Lake)  
#### Summary  
- Investigates computational bottlenecks in the Frozen Lake Q-learning problem.  
- Uses Gymnasium’s Frozen Lake environment and implements Q-learning algorithm.  
- Identifies the `Q-table update` function as the primary bottleneck.  
- Performance comparisons and benchmarks are available here: [Link](https://github.com/A-m-e-y/W03_C10_Frozen_Lake?tab=readme-ov-file#performance-comparison)

#### Hardware Acceleration  
- Created a hardware acceleration solution available in:  
  - 🔗 [Frozen_Lake_HW_Accelerator](https://github.com/A-m-e-y/Frozen_Lake_HW_Accelerator)  
- Includes:  
  - Python Q-learning implementation  
  - Verilog hardware module for Q-value updates  
  - Hardware-software co-simulation using `cocotb`  
  - Benchmark framework comparing hardware and software performance.

### Challenge #11 – GPU Acceleration of Frozen Lake Q-learning  
#### GitHub Repository  
- 🔗 [W03_C11_Frozen_Lake](https://github.com/A-m-e-y/W03_C10_Frozen_Lake)  
#### Summary  
- Offloads the Q-table update computations to GPU using `CuPy` library on an Nvidia RTX 3050 GPU.  
- Provides detailed performance comparison here: [Link](https://github.com/A-m-e-y/W03_C10_Frozen_Lake?tab=readme-ov-file#performance-comparison)

### Challenge #12 – Software-only Implementation and Cocotb Testbench Setup  
#### Summary  
- Started implementing the pure software baseline.  
- Selected `cocotb` as the testbench framework.  
- For detailed updates, check the [Project Journal](https://a-m-e-y.github.io/ECE_510_Documentation/project_journal.html).

---

## Week 4

### Challenge #13 – SAXPY Performance Benchmarking on CPU and GPU  
#### GitHub Repository  
- 🔗 [W04_C13_SAXPY](https://github.com/A-m-e-y/W04_C13_SAXPY)  
#### Summary  
- Benchmarks SAXPY operations on CPU (i5-12450H) and GPU (Nvidia RTX-3050 4GB VRAM).  
- Highlights that raw GPU horsepower is insufficient without addressing memory bottlenecks and execution patterns.  
- Shows GPU acceleration benefits when minimizing data transfers, boosting arithmetic intensity, and optimizing data locality.  
- Findings and visualizations are documented here: [Link](https://github.com/A-m-e-y/W04_C13_SAXPY#-visualization-1-cpu-vs-gpu-total-time-log-scale)

### Challenge #14 – Fibonacci Sequence Computation Using CUDA  
#### GitHub Repository  
- 🔗 [W04_C14_Fibonacci](https://github.com/A-m-e-y/W04_C14_Fibonacci)  
#### Summary  
- Implements Fibonacci number calculations on GPU using CUDA.  
- Compares GPU kernel speed vs CPU implementation, revealing that GPU overhead (memory allocations and transfers) significantly affects total runtime.  
- Demonstrates that only a fraction of GPU time is spent in actual computation.  
- Detailed results and charts are in the README: [Link](https://github.com/A-m-e-y/W04_C14_Fibonacci#-full-metrics-breakdown)

---

## Week 5

### Challenge #16 – SAXPY Benchmark Using PyTorch  
#### GitHub Repository  
- 🔗 [W05_C16_feedforward_NN](https://github.com/A-m-e-y/W05_C16_feedforward_NN)  
#### Summary  
- Benchmarks a fully connected neural network (FCNN) with varying hidden layers (1 to 10).  
- Compares runtime on:  
  - CUDA custom kernel  
  - PyTorch GPU backend  
  - PyTorch CPU backend  
- Includes full overhead accounting (memory allocation, host-device copies, kernel launch).  
- Data and performance graphs are available here: [Link](https://github.com/A-m-e-y/W05_C16_feedforward_NN#collected-results)

### Challenge #17 – Bubble Sort on a Systolic Array  
#### GitHub Repository  
- 🔗 [W05_C17_BubbleSort_Systolic_Array](https://github.com/A-m-e-y/W05_C17_BubbleSort_Systolic_Array)  
#### Summary  
- Implements bubble sort in pure Python (CPU) and as a systolic array simulation in NumPy.  
- Benchmarks and compares both across input sizes.  
- Provides animated visualization of systolic array sorting: [Link](https://github.com/A-m-e-y/W05_C17_BubbleSort_Systolic_Array#visualization-of-a-systolic-array)

---

## Week 6

### Challenge #19 – Binary Leaky Integrate-and-Fire (LIF) Neuron  
#### GitHub Repository  
- 🔗 [W06_C19_Binary_LIF_Neuron](https://github.com/A-m-e-y/W06_C19_Binary_LIF_Neuron)  
#### Summary  
- Builds a binary LIF neuron model in Python.  
- Simulates responses to different inputs and analyzes its behavior.

---

## Week 7

### Challenge #22 – Exploring Neuromorphic Computing Concepts  
#### GitHub Repository  
- 🔗 [W07_C22_Neuromorphic_Computing](https://github.com/A-m-e-y/W07_C22_Neuromorphic_Computing)  
#### Summary  
- Studies fundamental principles and applications of neuromorphic computing.  
- Implements simple spiking neural network models.  
- Compares efficiency against traditional computing methods.

---

## Week 8

### Challenge #24 – Simulation on EBRAINS BrainScaleS-2 Neuromorphic Hardware  
#### GitHub Repository  
- 🔗 [W08_C24_EBRAINS_BrainScaleS2](https://github.com/A-m-e-y/W08_C24_EBRAINS_BrainScaleS2)  
#### Summary  
- Runs simulations on the BrainScaleS-2 platform.  
- Examines hardware architecture and programming model.  
- Analyzes performance benefits compared to conventional simulation.

---

## Week 9

### Challenge #26 – Utilizing BrainChip’s IP for Edge AI  
#### GitHub Repository  
- 🔗 [W09_C26_BrainChip](https://github.com/A-m-e-y/W09_C26_BrainChip)  
#### Summary  
- Investigates BrainChip’s Akida IP for AI at the edge.  
- Implements sample applications with the Akida SDK.  
- Evaluates performance and efficiency on edge devices.
