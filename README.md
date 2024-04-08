Automated ECG Classification Using RNN and LSTM

Introduction
This project aims to automate the classification of electrocardiogram (ECG) data by leveraging the power of deep learning, specifically Recurrent Neural Networks (RNN) with Long Short-Term Memory (LSTM) units. An ECG is a non-invasive test that records the electrical activity of the heart, providing essential information about its rhythm and pace. By accurately classifying ECG signals into six categories—non-ectopic (normal) [N], supraventricular [S], ventricular [V], fusion [F], unknown beat [Q], and newly identified block [B]—this project seeks to mimic human diagnostic abilities and enhance accessibility to quality cardiac care.

Background
Our work is inspired by existing studies on ECG data preparation, feature extraction, and classification using machine learning models. We extend these efforts by incorporating LSTM networks to handle the sequential nature of ECG signals, addressing the limitations of traditional feed-forward networks and improving upon a baseline model built with Support Vector Machine (SVM) and Principal Component Analysis (PCA).

Dataset
We utilized the MIT-BIH Arrhythmia Database, comprising 48 half-hour excerpts from 24-hour ambulatory ECG recordings, enriched by adding a new class for block beats [B]. This enhancement aims to increase classification granularity and address the class imbalance inherent in the dataset.

Model Architecture
The project evolves from a baseline SVM model to an advanced LSTM network. LSTM's ability to remember long-term dependencies makes it particularly suitable for sequential data like ECG signals. Our model includes 100 hidden layers and 6 output layers, with a total of 41,806 parameters, indicating its complexity and capability to capture intricate details within ECG data.

Installation and Usage
Prerequisites: Ensure you have Python 3.8+ and pip installed.
Dependencies: Install all dependencies by running pip install -r requirements.txt.
Running the Model: To train the model, execute python train_model.py. To evaluate the model on new data, run python evaluate_model.py.
Data Processing
A detailed overview of the data processing steps is provided, including signal isolation, feature extraction, and data augmentation, to prepare the data for both the baseline and primary models.

Results
Our LSTM model achieved an accuracy of 78.06231% at the 30250th iteration, demonstrating its effectiveness in ECG signal classification. The baseline SVM model showed modest accuracy, underscoring the advancement achieved with the LSTM model.

Testing
The model was tested on the "Icentia11k Single Lead Continuous Raw Electrocardiogram Dataset," achieving an accuracy of 68.1330% on new data. This test underscores the model's generalizability and potential for real-world application.

Discussion and Ethical Considerations
The project discusses the challenges of biased datasets, the necessity of data augmentation, and ethical considerations surrounding AI in healthcare. Transparency and fairness are emphasized as crucial to the responsible deployment of AI technologies.

Contributions
Contributions are welcome, and potential contributors are encouraged to read through the CONTRIBUTING.md document for guidelines on how to submit pull requests, report issues, or add to the documentation.

License
This project is made available under the MIT License.

Acknowledgments
We acknowledge the creators of the MIT-BIH Arrhythmia Database and the Icentia11k dataset for providing the data essential to this research. Additionally, we thank the researchers whose studies laid the groundwork for our project.

#Links
Model Snapshot: https://bit.ly/CardioCareModelSnapshot
Project Documentation: https://bit.ly/CardioCareDocuments
