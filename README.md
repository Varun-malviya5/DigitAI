# DigitAI

**DigitAI** is a multi-digit classification project that uses the SVHN dataset and a deep neural network (ANN).  
The focus is to classify digits by tuning the number of hidden layers, using Dropout and Batch Normalization, and adjusting the learning rate and batch size.  
This project uses only fully connected layers and does not use any convolutional layers.

---

## Project Structure

DigitAI/
├── data/
│ └── SVHN_single_grey1.h5
├── Multi_digits_classification.ipynb
├── README.md

yaml
Copy
Edit

---

## Description

- Dataset: Street View House Numbers (SVHN)
- Model: Deep Artificial Neural Network (ANN)
- Methods used: Hidden layer tuning, Dropout, Batch Normalization, learning rate and batch size tuning
- Goal: Achieve good accuracy without using CNNs

---

## How to Run

1. **Clone the repository**

   ```bash
   git clone https://github.com/Varun-malviya5/DigitAI.git
   cd DigitAI
2. Install dependencies

Install the required Python libraries:

bash
Copy
Edit
pip install tensorflow numpy matplotlib h5py scikit-learn
3. Run the notebook

Open Multi_digits_classification.ipynb in Jupyter Notebook, VS Code, or Google Colab and run the cells step by step.

4. Train the model

You can adjust:

Number of hidden layers

Dropout rates

Batch Normalization placement

Learning rate and batch size

The training and validation accuracy will help you see what works best.

5. Evaluate

The notebook shows the test accuracy and predictions on unseen test data.

Results
This ANN model reaches about 76% test accuracy on the SVHN dataset.
The accuracy was improved by:

Adding more hidden layers

Using Dropout to reduce overfitting

Adding Batch Normalization for stable training

Tuning the learning rate and batch size

Dataset
The dataset file SVHN_single_grey1.h5 contains the training and test data in grayscale 32x32 format.

Labels are one-hot encoded for multi-class classification.

Notes
This project only uses fully connected layers to show how much accuracy can be achieved without CNNs.

You can extend this project by adding a CNN version for comparison in the future.

If the dataset is large, avoid pushing it to GitHub. Store it in a data/ folder locally.