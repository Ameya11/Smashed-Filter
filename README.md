Here's a README for your project:

---

# CS 754: Smashed Filter: GLMC Classifier 
## Objective

This project aims to classify musical instruments into one of ten categories using the NSynth dataset. The categories are:
- **Bass**
- **Brass**
- **Flute**
- **Guitar**
- **Keyboard**
- **Mallet**
- **Organ**
- **Reed**
- **String**
- **Vocal**

## Dataset

The dataset used for this project is the NSynth dataset, which contains recordings of musical instruments. Each instrument class has distinct characteristics, such as:
- **Time**
- **Pitch**
- **Rhythm**
- **Harmony**

The dataset is stored in the `dataset` folder.

## Methodology

### Compressed Measurements
A Gaussian measurement matrix was used to obtain compressed measurements of the input data, reducing the dimensionality while preserving essential information.

### Cross-Validation
A 5-fold cross-validation technique was implemented to ensure that the model generalizes well to unseen data.

### Prediction
The model computes the class likelihood for each class label based on the observed features. It then selects the class label with the maximum likelihood as the predicted class for the input data point.

### Addition of Gaussian Noise
To assess the robustness of the model, Gaussian noise was added to the input data. The model's performance was then compared with and without the added noise.

## Performance Evaluation

The performance of the Gaussian Mixture Model for Likelihood Classification (GMLC) was evaluated using the following metrics:
- **Accuracy**
- **Precision**
- **Recall**
- **F1 Score**

These metrics were calculated for both noisy and non-noisy data to assess the model's robustness.

## Code

The code for this project is provided in a Jupyter Notebook (`.ipynb`), which is included in this repository. The notebook contains all the necessary steps, from data loading to model evaluation.

## Results

The results of the model's performance, both with and without Gaussian noise, are presented in the notebook. Detailed evaluations, including accuracy, precision, recall, and F1 score, are provided.

## How to Run

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/Ameya11/musical-instrument-classification.git
   ```
2. **Run the Jupyter Notebook**:
   Open the Jupyter Notebook in your preferred environment and run the cells to see the model in action.



---

This README provides an overview of the project, details on how to use the code, and how to evaluate the model. Let me know if you need any further adjustments!
