# Epileptic-Classification
There are six Colab files in this repository. Each file represent a Level in Wavelet Transform to extract the features from the EEG Signals.
First, the signals are extracted in a Dataframe. These Signals are EEG Signals. The dataset is from the Bonn University.
The Dataset is divided into two groups. First group comprises of the Datasets A, B, C, D which are labelled as Non- Seizure EEG Signals. Second group comprises of the Dataset E, which are labelled as Siezure EEG Signals.
The signals are then used to extract the features using Wavelet Transform with 'Bior' family. These features are as follows: HFD, PFD, and SVD Entropy.
Using these features as an input to the ANN models, the accuracy results are calculated.
There are different types of ANN Models used in these files. 
Best accuracy results were obtained from the Levenbergh- Marquardt Backpropagation Algorithm.
The results from all the files havebeen compiled and is uploaded as a jpeg file.
