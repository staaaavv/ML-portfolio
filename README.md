# ML-portfolio
# Vehicle Fault Prediction & Anomaly Detection using Autoencoders

**Project Overview:**  
This project explores a methodology for analyzing OBD-II data to predict critical vehicle parameters affecting performance and reliability. Using **artificial intelligence** and **machine learning**, the system automates fault diagnosis and anomaly detection through an **Autoencoder neural network**.

---

• **Dataset & Preprocessing**
- Selected **8 vehicle sensors** from OBD-II data  
- Preprocessed and normalized data using **MATLAB** for Autoencoder input  
- Dataset prepared to highlight meaningful patterns while reducing noise
- Sample file: `data/exp3_4drivers_1car_1routeNEW.xlsx`

---

• **Model Architecture & Training**
- **Autoencoder** with **20 neurons** in the hidden layer  
- **Regularization techniques:**  
  - L2 to prevent overfitting  
  - Sparsity regularization to focus on key features  
  - Sparsity proportion to control active neurons in the hidden layer  
- **Decoder transfer function:** `purelin` for reconstructing continuous values  
- **Training algorithm:** `trainscg` (scaled conjugate gradient)  
- **Training epochs:** 400 to learn normal data distribution  

---

• **Anomaly Detection**
- Reconstructed sensor data using the trained autoencoder  
- Calculated **reconstruction error (MSE)**  
- Defined anomaly threshold based on MSE  
- Compared original and reconstructed data  
- Visualized results through plots showing:  
  - MSE distribution  
  - Detected anomalies  
  - Original vs reconstructed data  

---

• **Key Highlights**
- Successfully detected deviations in sensor readings  
- Related anomalies to OBD-II fault codes and sensor specifications  
- Methodology can be extended to other OBD-II parameters, enhancing predictive maintenance capabilities

---

• **Technologies & Tools**
- **MATLAB** for preprocessing, training, and analysis  
- **Autoencoder Neural Networks**  
- Data visualization and evaluation techniques for fault prediction

---

• **How to Use**
1. Open MATLAB project/notebook (`.mlx`)  
2. Load OBD-II dataset (`data/` folder)  
3. Run training scripts to train the Autoencoder  
4. Apply reconstruction to detect anomalies  
5. Review MSE plots and anomaly reports

---

• **Contact**
For questions or collaboration, feel free to reach out via GitHub or Upwork.

