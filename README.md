# Memory-Defender
Project Overview
Memory Defender is a tool designed to detect fileless malware using the CIC-MalMem-2022 dataset, which contains memory dump samples labeled as benign or malicious. The project aims to provide a reliable method for analyzing memory dumps and determining the maliciousness of a given sample. To use Memory Defender, provide a memory dump sample as input. The system will then process the data and output whether the sample is identified as malicious or benign.

Installation
To use Memory Defender, ensure you have Python 3 installed on your system. You can set up the required environment by running the following command to install dependencies from the provided requirements.txt file

Workflow
1. Data Preprocessing:
   - Check for null values and duplicate entries in the dataset.
   - Clean the data to ensure high-quality input for model training.

2. Feature Engineering:
   - Perform label encoding to convert categorical variables into numerical format.
   - Select relevant features using feature selection techniques.

3. Model Training:
   - Perform hyperparameter tuning to optimize the model's performance.
   - Train the model using the processed data.

4. Model Evaluation:
   - Evaluate the model's performance using metrics such as accuracy, precision, recall, and F1 score.
   - Determine the model's effectiveness in detecting fileless malware.

Datasets
The CIC-MalMem-2022 dataset used in this project contains obfuscated malware samples. Obfuscated malware hides to avoid detection and extermination, making it challenging to detect using traditional methods. The dataset includes Spyware, Ransomware, and Trojan Horse malware, providing a balanced set for testing obfuscated malware detection systems. The memory dump process in this dataset uses debug mode to avoid showing up in memory dumps, creating a more realistic representation of a malware attack scenario.

Model 
Comparison Furthermore, the performance comparison was conducted using accuracy, F1 score, and precision between the proposed model and models developed by Carrier (2022), Talukder (2022), Daryle Q. Smith (2022), Murat Dener (2022), and Lourdes Bruna Moralejo (2023). The comparison was performed on the CIC-MalMem-2022 dataset, evaluating each model's effectiveness in detecting obfuscated malware in memory dumps.

Environment
Memory Defender was developed using Google Colab as the development environment and Python 3 for coding and analysis.
