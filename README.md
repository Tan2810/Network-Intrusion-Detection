# Network Intrusion Detection Using the UNSW-NB15 Dataset

## Overview
This project aims to develop machine learning models for detecting network intrusions using the UNSW-NB15 dataset. It focuses on understanding the dataset, performing feature selection, and building models that identify and classify various network attacks. The project covers data preprocessing, training, visualization, and multi-class classification to evaluate attack probabilities.

## Project Structure



## Notebooks and Analysis
### 1. Data Analysis and Training (`nb15_training.ipynb`)
- Explores the dataset, visualizes attack distributions, and performs correlation analysis.
- Identifies top features that are important for determining network intrusions.
- Creates visualizations such as heatmaps and bar charts to show feature importance and attack distributions.

### 2. IP-Based Prediction (`Ip_prediction.ipynb`)
- Implements a model that predicts the likelihood of an IP address being part of an attack.
- Utilizes `RandomForestClassifier` and `OneHotEncoder` for training and probability estimation.
- Provides probability scores indicating potential intrusion risk for specific IPs.

### 3. Feature-Based Probability Analysis (`Features_Probablity.ipynb`)
- Selects relevant features for training (e.g., `sttl`, `ct_state_ttl`, `Sload`).
- Trains models to determine if a network packet is an attack based on feature inputs.
- Evaluates model performance using precision, recall, and F1-score metrics.

### 4. Multi-Class Classification (`targets.py`)
- Implements multi-class classification to predict the type of attack (e.g., DoS, Fuzzers, Exploits).
- Uses `RandomForestClassifier` to output probabilities for various attack types.

## Visualizations
- **Attack Frequencies**: Shows the distribution of different types of network attacks.
- **Feature Importance Heatmap**: Highlights the top features influencing network intrusion detection.

## How to Use This Project
### Clone the Repository
```bash
git clone https://github.com/Tan2810/Network-Intrusion-Detection.git
cd Network-Intrusion-Detection

# Install Dependencies
pip install -r requirements.txt

# Run Jupyter Notebooks
jupyter notebook

# Running Scripts
python notebooks/targets.py
```
## Results and Outcomes
### Feature Selection
- The selected top features contributed to improved model performance, enhancing the detection of network intrusions.


## IP and Feature-Based Predictions
### 
- The models demonstrated high accuracy in classifying network traffic.

## Multi-Class Classification
### 
- The multi-class model successfully provided probabilities for various attack types, offering better insight into potential threats.

## Future Enhancements
### Future Enhancements:
### 
-  Advanced Models: Integrate deep learning models like LSTM for sequence-based intrusion detection.
-  Explainability: Utilize tools like SHAP or LIME to make model predictions more interpretable.
-  Real-Time Deployment: Modify models for real-time intrusion detection systems."

## Contributing
### 
Contributions are welcome! Fork the repository and submit a pull request.

## License
### 
This project is licensed under the MIT License. See the LICENSE file for more details.

## Contact
For questions or collaborations, please contact [Tanmay Bandaru](mailto:tanmaybandaru@gmail.com).





