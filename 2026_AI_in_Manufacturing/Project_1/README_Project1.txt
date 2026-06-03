
Project 1: Predicting Fatigue-Life Class from Process Parameters
================================================================

In this mini project, you will work with a small additive manufacturing dataset.
Your task is to use basic supervised machine learning models to predict whether
a printed specimen belongs to a short-life or long-life fatigue group.

This project is designed for beginners. You do not need to know the full physics
of fatigue or additive manufacturing to complete it. The main goal is to practice
the machine learning workflow using a real manufacturing-style dataset.

Dataset
-------
File name:
data/project1_process_parameters_fatigue_class.csv

Each row in the dataset represents one printed fatigue specimen.

The dataset contains:

1. Input features
   These are the process parameters used during printing.

   - power
     Laser power used during printing.

   - scan_speed
     Speed at which the laser moved during printing.

   - hatch_spacing
     Distance between neighboring laser scan lines.

   - layer_thickness
     Thickness of each printed layer.

   - ved
     Volumetric energy density. This combines power, scan speed,
     hatch spacing, and layer thickness into one process-related value.

2. Target label
   This is the value your model will try to predict.

   - fatigue_life_class
     The specimen is labeled as either:
     - short_life
     - long_life

What you need to do
-------------------
Your job is to build a classification model.

A classification model predicts categories. In this project, the two categories are:

- short_life
- long_life

Suggested workflow
------------------
1. Load the CSV file using pandas.
2. Look at the first few rows of the dataset.
3. Check how many specimens are short_life and how many are long_life.
4. Select the process parameters as input features.
5. Select fatigue_life_class as the target.
6. Split the dataset into training and testing sets.
7. Train one or more supervised learning models.
8. Test the models on the testing data.
9. Compare the results.
10. Discuss what the results mean.

Models you can try
------------------
You may try models such as:

- Decision Tree
- Random Forest
- Support Vector Machine
- Bagging Classifier
- XGBoost, if it is available on your computer

Evaluation
----------
To evaluate the models, you can use:

- accuracy
- confusion matrix
- classification report
- precision
- recall
- F1-score

Important discussion point
--------------------------
Do not worry if the accuracy is not very high.

That is part of the lesson.

In real manufacturing datasets, the number of samples is often small, and many
specimens may have very similar process parameters. When the input features do
not vary much, machine learning models may struggle to make strong predictions.

So the main question for this project is:

Can process parameters alone predict whether a printed specimen will have
short or long fatigue life?
