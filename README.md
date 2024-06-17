# AD-classification-Confidence

This repository contains a comprehensive machine learning pipeline for classifying Alzheimer's disease labels from neuroimaging data. The project involves data preprocessing, handling class imbalance with SMOTE, implementing a custom neural network layer for confidence scores, and evaluating model performance using Leave-One-Out cross-validation.

## Folder Structure

### `AD_classification_code`

The `AD_classification_code` folder contains the Python code for computing confidence temperatures ranging from 0.5 to 2.5 in 0.5 steps. Each of the following five Jupyter notebooks (`.ipynb` files) corresponds to a specific confidence temperature value:
- `Demntia_Classifcation_&_Confidence_with_Temp_0.5.ipynb`: Code for confidence temperature 0.5
- `Demntia Classifcation & Confidence with Temp 1.0.ipynb`: Code for confidence temperature 1.0
- `Demntia Classifcation & Confidence with Temp 1.5.ipynb`: Code for confidence temperature 1.5
- `Demntia Classifcation & Confidence with Temp 2.0.ipynb`: Code for confidence temperature 2.0
- `Demntia_Classifcation_&_Confidence_with_Temp_2.5.ipynb`: Code for confidence temperature 2.5

### `Sample_data`

The `Sample_data` folder contains the dataset used in this project:
- `Data_ADNIMerge_procssedNeuroImaging.csv`: The processed dataset for Alzheimer's disease classification.

### Running the Notebooks in Google Colab

To run a Jupyter notebook from this repository in Google Colab, follow these steps:

1. **Open Google Colab**: Go to [Google Colab](https://colab.research.google.com/).

2. **Open a GitHub Notebook**: Click on the "GitHub" tab.

3. **Authenticate with GitHub (if needed)**: You might need to authenticate your GitHub account to allow access.

4. **Paste the GitHub URL**: Copy and paste the URL of your notebook into the provided field. For example, to open the notebook for confidence temperature 0.5, use: (https://github.com/Afolabialausa/Alzheimer-s-Disease-Classification-/blob/main/AD_classification_code/Demntia_Classifcation_&_Confidence_with_Temp_0.5.ipynb)

5. **Open the Notebook**: Click on the notebook from the search results to open it in Colab.

## Key Features

- **Heterogeneous Data Utilisation**: Incorporation of diverse data sources including cognitive and functional assessments, tau-PET and MRI neuroimaging, medical/family history, demographic data, and APoE genotype for a comprehensive analysis.
- **Confidence Estimation**: A novel approach using a softmax confidence metric based on the network’s output activity to evaluate classification confidence at the individual level.
- **Custom Neural Network Layer**: Implementation of a custom ConfidenceSoftmax layer that computes confidence scores for each model prediction.
- **Robust Model Evaluation**: Application of Leave-One-Out Cross-Validation (LOOCV) to ensure the reliability and robustness of the model's performance.
- **Optimised Confidence Temperature**: Investigation of different confidence softmax temperature values to determine the optimal temperature for the most reliable confidence scores.

## Usage

1. **Preprocessing**: Open the Jupyter notebook for the desired confidence temperature (e.g., `Demntia_Classifcation_&_Confidence_with_Temp_0.5.ipynb`) and run the scripts to prepare the data. This includes handling missing data and normalising the dataset.
2. **Training**: Execute the training cells in the same notebook to train the neural network.
3. **Evaluation**: Continue running the notebook to assess model performance. The evaluation includes calculating accuracy, F1 score, precision, recall, and confidence scores for each class prediction.
4. **Visualisation**: The notebook includes cells to visualise the results and confidence scores.

For detailed instructions on how to run each step, please refer to the comments and markdown cells within each Jupyter notebook.

## Contributing

We welcome contributions to this project. Please fork the repository, create a new branch, and submit a pull request with your changes.

## Licence

This project is licensed under the GNU General Public License Version 3 - see the LICENSE file for details.
