# DogClassifier

Dog Classification Model Explanation:

This Python code is for a dog classifica;on model that uses machine learning techniques to classify images of dogs into specific breeds. Here's a simplified breakdown of its funcionality:

Data Preparaon:
• Load image labels from a CSV file.
• Choose specific dog breeds (e.g., 'scoKsh_deerhound', 'maltese_dog', 'bernese_mountain_dog')
for classifica;on.
• Convert images to a standardized format, normalize pixel values, and perform one-hot encoding
on breed labels.

Model Training:
• Split the dataset into training, validation, and test sets.
• Train three machine learning models: Random Forest, Support Vector Machine (SVM), and KNearest Neighbors (KNN).

Evalua1on:
• Evaluate the trained models on a test set and print accuracy and F1 score for each model.
• Create a bar chart comparing the performance of the models.
• Confusion Matrices:
• Generate confusion matrices for each model, illustra;ng how well they classify images into the
chosen dog breeds.

Model Saving:
• Save the trained Random Forest model to a file using the Joblib library.

Interac1ng with the Code:
For future users:
• Adjust the list of selected dog breeds in the CLASS_NAMES variable.
• Ensure the dataset path and file names match your setup.
• Run the code step by step or in its en;rety to train and evaluate the models.
• Use the saved Random Forest model for making predic;ons on new images.


    
