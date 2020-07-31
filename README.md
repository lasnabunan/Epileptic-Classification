# Epileptic-Classification
There are six Colab files in this repository. Each file represent a Level in Wavelet Transform to extract the features from the EEG Signals.
First, the signals are extracted in a Dataframe. These Signals are EEG Signals. The dataset is from the Bonn University.
The Dataset is divided into two groups. First group comprises of the Datasets A, B, C, D which are labelled as Non- Seizure EEG Signals. Second group comprises of the Dataset E, which are labelled as Siezure EEG Signals.
The signals are then used to extract the features using Wavelet Transform with 'Bior' family. These features are as follows: HFD, PFD, and SVD Entropy.
Using these features as an input to the ANN models, the accuracy results are calculated.
There are different types of ANN Models used in these files. 
Best accuracy results were obtained from the Levenbergh- Marquardt Backpropagation Algorithm.
The results from all the files havebeen compiled and is uploaded as a pdf file.

## WORK FLOW
* **REQUIREMENTS:**
This project requires the extraction of features from the EEG data signals. In python, this
part can be done using an open source library ‘pyeeg’. The EEG signals are decomposed
in wavelets using ‘PyWavelet’ package in python.
* **DataSet:**
The Dataset is loaded in the google colab. This Dataset is taken from Bonn University.
The Dataset is divided in 5 sets, in which Set A, B, C and D are labelled as Non-Seizure
category, class “0” while the Set E is labelled as Seizure category, class “1”. These sets
are used to prepare the two matrices containing the sampled signals.
* **Wavelet Transform:**
The two matrices are then passed through a Wavelet filter with different levels, 1-6
and the decomposed signals are being stored in the matrices for each category. The
filters used are of the ‘Bior’ family.
* **eature Extraction:**
Once the Decomposed signals are stored in the matrices, these matrices are then
passed through the feature extraction unit using PYEEG package in python. The
features extracted are Petrosian Fractal Dimension (PFD), Higuchi Fractal Dimension
(HFD) and Singular Value Decomposition Entropy.
* **Training and Test Sets:**
The entire feature sets are then distributed in the training and test sets where 80% is
training set and 20% is the test set.
* **Classification Models:** Different Models are trained using the training set.
1. ANN using Linear Activation Function in the output layer
2. SVM Classification.
3. ANN using Sigmoid Activation Function
4. ANN using Linear Activation Function in the output layer using Cross Validation
5. SVM Classification using Cross Validation.
6. ANN using Sigmoid Activation Function using Cross Validation.
The Accuracies of the models are then displayed using the graph and stored in an excel
file.

![Diagram](https://github.com/lasnabunan/Epileptic-Classification/blob/master/WORK%20FLOW.png)
