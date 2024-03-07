# Spam Detection using Logistic Regression

This repository contains Python code for detecting spam emails using Logistic Regression. The model is trained on a dataset containing email messages labeled as spam or ham (not spam).

## Dependencies

- numpy
- pandas
- scikit-learn

## Installation

You can install the required dependencies using pip:

```bash
pip install numpy pandas scikit-learn
```

## Usage

1. Clone the repository:

```bash
git clone <repository_url>
cd <repository_directory>
```

2. Ensure you have a CSV file containing email data. By default, the code assumes the file is named `spam.csv` and contains columns named `Message` and `Category` (spam or ham).

3. Run the Jupyter Notebook script:

The script will perform the following steps:

### Data Collection & Pre-Processing

- Load the data from the CSV file into a pandas DataFrame.
- Replace null values with an empty string.
- Label encode the categories: spam as 0, ham as 1.

### Splitting the Data

- Split the data into training and test sets.

### Feature Extraction

- Convert text data into feature vectors using TF-IDF vectorization.

### Training the Model

- Train a Logistic Regression model using the training data.

### Evaluating the Model

- Evaluate the accuracy of the model on both training and test data.

### Building a Predictive System

- Connect to a Gmail account using IMAP.
- Fetch emails from the inbox.
- Predict whether each email is spam or not using the trained model.

## Configuration

- Update the file path in the code to point to your CSV file if it's not named `spam.csv`.
- Adjust the IMAP settings (`user`, `password`, `imap_url`) according to your email provider.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
