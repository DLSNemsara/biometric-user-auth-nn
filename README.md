## **Biometric User Authentication with Neural Networks**
A MATLAB-based project implementing neural network models for biometric user authentication. The project includes both optimized and non-optimized neural networks for user classification, along with variance analysis scripts for feature analysis.

---

### **Table of Contents**
1. [Project Description](#project-description)
2. [Folder Structure](#folder-structure)
3. [Setup and Installation](#setup-and-installation)
4. [Usage Instructions](#usage-instructions)
5. [Methodology](#methodology)
6. [Contributing](#contributing)
7. [License](#license)

---

### **1. Project Description**
This project explores the use of neural networks for biometric user authentication. It involves:
- **Variance Analysis:** To analyze inter- and intra-user feature variance.
- **Neural Network Models:** For user classification.
  - **Non-Optimized Models:** Basic neural network implementations.
  - **Optimized Models:** Neural networks optimized for improved accuracy and efficiency.

The project utilizes MATLAB for dataset handling, variance computations, and neural network training.

---

### **2. Folder Structure**
```
Root/
│
├── CW-Data/                          # Contains dataset files used across tasks
│   ├── U01_Acc_FreqD_FDay.mat
│   ├── U01_Acc_FreqD_MDay.mat
│
├── Neural_Networks/                  # Neural network models
│   ├── non_optimized/                # Non-optimized neural networks
│   │   ├── load_dataset.m
│   │   ├── nn_user01.m
│   │   ├── nn_user02.m
│   │   ├── ...
│   │   ├── nn_user10.m
│   │
│   ├── optimized/                    # Optimized neural networks
│       ├── load_dataset_optimized.m
│       ├── opt_nn_user01.m
│       ├── opt_nn_user02.m
│       ├── ...
│       ├── opt_nn_user10.m
│
├── Variance_Analysis/                # Variance analysis scripts
│   ├── compute_intra_variance.m
│   ├── compute_inter_variance.m
│
├── README.md                         # Project documentation
```

---


### **3. Setup and Installation**
Follow these steps to set up the project on your local machine:

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/DLSNemsara/biometric-user-auth-nn.git
   cd biometric-user-auth-nn
   ```

2. **Ensure MATLAB is Installed:**
   - MATLAB **R2021b** or later is recommended.
   - Required Toolboxes:
     - **Neural Network Toolbox**
     - **Statistics and Machine Learning Toolbox**

3. **Dataset Preparation:**
   - The complete dataset (`.mat` files) is located in the `CW-Data`/ folder.
   - For convenience, you may copy the dataset to the respective script directories (`Neural_Networks/non_optimized/`, `Neural_Networks/optimized/`, and `Variance_Analysis/`) to avoid MATLAB path-related issues when running the code.

---


#### **Running Variance Analysis**
1. Open MATLAB.
2. Navigate to the `Variance_Analysis/` folder.
3. Run the scripts:
   ```matlab
   compute_intra_variance
   compute_inter_variance
   ```

#### **Training and Testing Neural Networks**
1. **Non-Optimized Models:**
   - Navigate to the `Neural_Networks/non_optimized/` folder.
   - Load the dataset:
     ```matlab
     load_dataset
     ```
   - Run a neural network for a specific user, e.g., User 1:
     ```matlab
     nn_user01
     ```

2. **Optimized Models:**
   - Navigate to the `Neural_Networks/optimized/` folder.
   - Load the dataset:
     ```matlab
     load_dataset_optimized
     ```
   - Run an optimized neural network for a specific user, e.g., User 1:
     ```matlab
     opt_nn_user01
     ```

---


### **5. Methodology**
#### **1. Variance Analysis:**
   - **Intra-Variance:** Computes the variability within a user's biometric data.
   - **Inter-Variance:** Computes the variability between different users.

#### **2. Neural Network Models:**
   - **Non-Optimized Models:** Simple architectures to understand baseline performance.
   - **Optimized Models:** Architectures fine-tuned with additional layers and parameters to improve results.

---

### **6. Contributing**
Contributions are welcome! Please follow these steps:
1. Fork this repository.
2. Create a new branch:
   ```bash
   git checkout -b feature-name
   ```
3. Commit your changes and push the branch:
   ```bash
   git push origin feature-name
   ```
4. Open a Pull Request.

---

### **7. License**
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

---
