# Machine Learning for prediction of elastic constants of isotropic material in Resonance Ultrasound Spectroscopy (RUS)

## Project Description
This project applies machine learning and deep learning techniques to analyze and predict material properties using data obtained from Resonance Ultrasound Spectroscopy (RUS). The goal is to classify material types, including metals, polymers, and ceramics, and collect their material properties such as Young's modulus, Poisson's ratio, and density. The data is simulated to obtain the resonance frequencies of each material. Machine learning and deep learning models are applied to predict Young's modulus and Poisson's ratio based on inputs such as eigenfrequencies, density, and geometric parameters.


## Process overview
1. **Forward Model**  
   i. **Data Collection**:
   - Extract the list of Young's modulus and density from the Ashby chart for metals, polymers, and ceramics.
   - From various research papers and sources, find the Poisson's ratio of some material samples and determine the range of Poisson's ratio for each material class.
   - Compile a complete dataset of material properties containing density, Young's modulus, and Poisson's ratio for all material classes.

   ii. **Simulation**:
   - Develop a model to calculate eigenfrequencies using COMSOL Multiphysics with numerical finite element methods (FEM).
   - Use MATLAB LiveLink to generate the eigenfrequencies of each sample for various dimensions of cuboids and cylinders.
   - Collect the final dataset of material properties and resonance frequencies for each material class and each shape.


2. **Reverse Model**:  
  i. **Model Training**:  
   - Applied machine learning models (Random Forest, Support Vector Machines, etc.) and deep learning models to predict Young's modulus and Poisson's ratio from the extracted features.

6. **Model Evaluation**:  
   - Evaluated model performance based on metrics such as accuracy, mean absolute error (MAE), and mean squared error (MSE).

7. **Results Visualization**:  
   - Visualized the prediction 
## Installation
To set up the project locally, follow these steps:

```bash
git clone https://github.com/username/ML-for-RUS.git
cd ML-for-RUS
pip install -r requirements.txt
