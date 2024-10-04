# Credit Card Fraud Detection

This project aims to detect fraudulent credit card transactions using machine learning techniques. The dataset used for this task contains transactions made by European cardholders in September 2013. The dataset consists of 284,807 transactions, out of which 492 are frauds. The goal is to build a model that accurately identifies these fraudulent transactions.

## Dataset

The dataset used is provided in the file `creditcard.csv`, which contains the following features:
- **V1 to V28**: The result of a PCA transformation of the dataset to protect the confidentiality of sensitive information.
- **Time**: Number of seconds elapsed between this transaction and the first transaction in the dataset.
- **Amount**: The amount of the transaction.
- **Class**: The target variable (0 for non-fraudulent transactions, 1 for fraudulent transactions).

## Project Files

- **ML___Credit_Card_Fraud_Detection.ipynb**: The Jupyter Notebook containing the code for data preprocessing, model training, and evaluation.
- **creditcard.csv**: The dataset used for training and testing the model.

## Requirements

To run the project, the following Python libraries are required:
- `numpy`
- `pandas`
- `matplotlib`
- `seaborn`
- `scikit-learn`

Install the required libraries with the following command:
```bash
pip install numpy pandas matplotlib seaborn scikit-learn
```

## How to Run

1. Clone the repository to your local machine:
   ```bash
   git clone https://github.com/your_username/Credit-Card-Fraud-Detection.git
   ```
2. Navigate to the project directory:
   ```bash
   cd Credit-Card-Fraud-Detection
   ```
3. Open the Jupyter Notebook and run the cells:
   ```bash
   jupyter notebook ML___Credit_Card_Fraud_Detection.ipynb
   ```

## Model Training

The dataset is split into training and testing sets using an 80-20 split. We use the `RandomForestClassifier` from scikit-learn to build the fraud detection model. The model is evaluated based on accuracy, precision, recall, and the F1-score.

## Output

Below is a screenshot of the output:

![confusion-matrix](https://github.com/user-attachments/assets/cd261604-5a6d-4764-b82a-92dc9846e715)

## Conclusion

This model successfully detects fraudulent credit card transactions with a high level of accuracy. However, given the class imbalance (fraudulent transactions represent only 0.172% of the dataset), further techniques like oversampling, undersampling, or using more advanced machine learning algorithms can be explored to improve performance.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

