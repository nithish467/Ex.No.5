# EXPERIMENT 5: Comparing Prompting Techniques Through Engineering Problem-Solving Scenarios

## Date : 05/09/2026

## Name NITHISHKUMAR S

## Register No : 212223240109

## PROJECT TITLE

**LEAFGUARD – AI-Based Plant Disease Detection System**

## AIM

To compare different prompting techniques and evaluate their effectiveness in solving a real-world engineering problem using an AI-based plant disease detection scenario from the LEAFGUARD – AI-Based Plant Disease Detection System project.

## AI TOOLS REQUIRED

- ChatGPT

- Python

- Machine Learning

- Computer Vision

## EXPERIMENT OVERVIEW

**LEAFGUARD** is an AI-based plant disease detection system designed to identify diseases in plants by analyzing leaf images.

The system uses Artificial Intelligence, Machine Learning and Computer Vision techniques to analyze an uploaded leaf image and predict the possible disease affecting the plant.

Plant diseases can reduce crop production and affect agricultural productivity. Identifying diseases manually can be difficult and time-consuming, especially when farmers have limited access to agricultural experts.

The proposed AI system attempts to assist users by automatically analyzing plant leaf images and identifying possible diseases.

The system can identify diseases such as:

- Healthy Leaf

- Leaf Spot

- Powdery Mildew

- Rust

- Bacterial Blight

**For this experiment, the selected engineering problem is:**

How can an AI-based plant disease detection system analyze a leaf image, identify the possible disease, and provide a clear and useful prediction to the user?

The same engineering problem was given to ChatGPT using four different prompting techniques.

**The generated responses were then compared based on:**

- Relevance

- Accuracy

- Completeness

- Clarity

- Feasibility

- Usefulness

## SELECTED ENGINEERING SCENARIO

A user uploads an image of a plant leaf to the system.

The system should process the image and identify whether the leaf is healthy or affected by a disease.

The expected workflow is:
```
Leaf Image
    ↓
Image Preprocessing
    ↓
Feature Extraction
    ↓
Machine Learning Model
    ↓
Disease Classification
    ↓
Prediction
```
```
Example:

Input:
Image of Tomato Leaf

Expected Output:
Disease: Tomato Leaf Spot
```

## ENGINEERING PROBLEM

**The main engineering problem is to develop a system that can:**

Accept a plant leaf image.

Preprocess the image.

Extract useful visual features.

Classify the leaf condition.

Predict the possible disease.

Provide a clear result.

Handle different image conditions.

Achieve reliable classification performance.

## EXPECTED AI SOLUTION

The AI-based solution should:

Suggest a suitable dataset.

Explain image preprocessing.

Suggest an appropriate machine learning model.

Explain model training.

Suggest evaluation metrics.

Identify possible real-world problems.

Suggest a practical deployment method.

Explain limitations of the system.

## PROMPTING TECHNIQUE 1 – STRAIGHTFORWARD PROMPT

**Prompt**

Suggest a method to build an AI-based plant disease detection system using machine learning. Explain how to identify plant diseases from leaf images.

**AI-GENERATED OUTPUT**

An AI-based plant disease detection system can be developed using computer vision and machine learning.
```
The general workflow is:

Leaf Image
    ↓
Image Preprocessing
    ↓
Feature Extraction
    ↓
Machine Learning Model
    ↓
Disease Classification
    ↓
Disease Prediction
```
A labelled plant leaf image dataset can be used to train the model.

The images can be resized and normalized before training.

Possible machine learning and deep learning models include:

CNN

SVM

Random Forest

Transfer Learning

**A Convolutional Neural Network (CNN) is suitable for image classification because it can learn visual features from images.**

The model can be evaluated using:

Accuracy

Precision

Recall

F1-score

Confusion Matrix

## OBSERVATION

The straightforward prompt provides a basic solution for the plant disease detection problem.

It identifies the main technologies and gives a general workflow.

However, it does not provide detailed information about:

Dataset preparation

Image augmentation

CNN architecture

Training procedure

Deployment

Real-world challenges

## Limitations

Therefore, the response is useful for understanding the basic concept but requires a more detailed prompt for complete engineering implementation.

## PROMPTING TECHNIQUE 2 – ROLE-BASED PROMPTING

**Prompt**
```text
Act as a senior Computer Vision and Machine Learning Engineer. I am developing an AI-based Plant Disease Detection System for a final-year engineering project. The system should accept plant leaf images, preprocess them, classify the leaf using a deep learning model, and provide the predicted disease. Suggest a practical solution including dataset selection, preprocessing, model selection, training, evaluation and deployment. Explain the solution at a final-year engineering student level.
```

## AI-GENERATED OUTPUT

As a Computer Vision and Machine Learning Engineer, the system can be developed using a CNN-based image classification approach.

1. Dataset

A labelled plant leaf dataset should be used.

The dataset can contain different plant diseases and healthy leaf images.

Example classes include:

Healthy
Leaf Spot
Powdery Mildew
Rust
Bacterial Blight

The dataset should contain sufficient images for each class.

2. Image Preprocessing

Before training the model, the images should be preprocessed.

Common preprocessing techniques include:

Image resizing

Pixel normalization

Noise reduction

Image enhancement

For example, all images can be resized to:

128 × 128 pixels

3. Data Augmentation

Data augmentation can be used to increase the variety of training images.

Possible techniques include:

Rotation

Zoom

Width shifting

Height shifting

Brightness adjustment

Data augmentation can help the model generalize better to new images.

4. Model Selection

A CNN is suitable for this problem because it can automatically learn visual patterns from images.

The CNN can learn features such as:

Leaf shape

Spots

Color changes

Texture

Disease patterns

Transfer learning models can also be considered when a larger and more accurate model is required.

5. Model Training

The dataset can be divided into:

Training Dataset
Validation Dataset
Testing Dataset

The model learns from the training images and is evaluated using unseen testing images.

6. Evaluation

The model can be evaluated using:

Accuracy

Precision

Recall

F1-score

Confusion Matrix

7. Deployment

The trained model can be integrated into a web application.

Possible technologies include:

Python
TensorFlow/Keras
OpenCV
Flask
HTML
CSS
JavaScript

The user can upload a leaf image and receive the predicted disease.

## OBSERVATION

The role-based prompt generated a more professional and detailed response.

It covered:

Dataset

Image preprocessing

Data augmentation

CNN

Training

Evaluation

Deployment

Compared with the straightforward prompt, this response is more useful for actual project development.


## PROMPTING TECHNIQUE 3 – STEP-BY-STEP PROMPTING

**Prompt**

Perform a systematic engineering analysis for an AI-based Plant Disease Detection System.

Analyze the problem using the following steps:

Step 1: Understand the objective of the plant disease detection system.

Step 2: Identify the input and expected output.

Step 3: Explain the image preprocessing requirements.

Step 4: Suggest a suitable dataset and data preparation method.

Step 5: Select an appropriate machine learning/deep learning model and explain why it is suitable.

Step 6: Explain the model training process.

Step 7: Identify suitable evaluation metrics.

Step 8: Identify real-world challenges and edge cases.

Step 9: Suggest a practical deployment approach.

Step 10: Provide a final engineering recommendation.

The solution must be realistic and suitable for a final-year engineering project.

## AI-GENERATED OUTPUT

Step 1 – Understand the Objective

The objective is to develop an AI system that identifies plant diseases from leaf images.

The system should automatically determine whether the leaf is healthy or affected by a particular disease.

Step 2 – Input and Output

Input

Plant Leaf Image

## Output

Predicted Plant Disease

Example:

Input:
Tomato Leaf Image

Output:
Predicted Disease: Leaf Spot

Step 3 – Image Preprocessing

The image should be processed before being given to the model.

**Important preprocessing steps include:**

Image resizing

Pixel normalization

Noise reduction

Image augmentation

Step 4 – Dataset

A labelled plant disease dataset should be selected.

The dataset should contain:

Different plant species

Different disease categories

Healthy leaf images

Different lighting conditions

Different leaf orientations

The dataset should be divided into training, validation and testing sets.

Step 5 – Model Selection

CNN is suitable for this problem because it is designed for image-based classification.

CNN can learn features such as:
```
Edges
   ↓
Shapes
   ↓
Textures
   ↓
Spots / Patterns
   ↓
Disease Classification
```
Transfer learning can be used if higher accuracy is required.

Step 6 – Training

The CNN model is trained using labelled leaf images.

The training process can be represented as:
```
Input Image
     ↓
CNN
     ↓
Prediction
     ↓
Loss Calculation
     ↓
Backpropagation
     ↓
Weight Update
```
This process is repeated for multiple epochs.

Step 7 – Evaluation

The model can be evaluated using:

Accuracy

Precision

Recall

F1-score

Confusion Matrix

The confusion matrix can show which disease classes are commonly confused.

Step 8 – Real-World Challenges

Poor Lighting

Low-light images may reduce prediction accuracy.

Blur

Blurred photographs may hide disease patterns.

Complex Background

Grass, soil and other objects may make classification difficult.

Similar Diseases

Some diseases may have similar visual symptoms.

Unseen Diseases

The model may not correctly identify diseases that were not included in the training dataset.

Step 9 – Deployment

The trained model can be deployed as a web application.

The workflow can be:
```
User
 ↓
Upload Leaf Image
 ↓
Web Interface
 ↓
Backend
 ↓
Trained CNN Model
 ↓
Disease Prediction
 ↓
Display Result
```
Step 10 – Final Engineering Recommendation

A CNN-based plant disease classification system is feasible for a final-year engineering project.

The project should initially focus on a limited number of disease classes.

After achieving reliable performance, the system can be extended with:

More plant species

More diseases

Mobile application

Real-time camera detection

Cloud deployment

Disease severity estimation

## OBSERVATION

Step-by-step prompting produced a systematic engineering analysis.

The AI followed the requested sequence and covered:

Objective

Input/output

Preprocessing

Dataset

Model

Training

Evaluation

Challenges

Deployment

Recommendation

This makes the response easier to understand and useful for project planning.

## COMPARISON OF PROMPTING TECHNIQUES

**Prompting Technique**

Relevance

Accuracy

Completeness

Clarity

Feasibility

Usefulness

**Straightforward Prompt**

Good

Good

Medium

Good

Very Good

Good

**Role-Based Prompt**

Very Good

Very Good

Good

Very Good

Very Good

Very Good

**Constraint-Based Prompt**

Excellent

Excellent

Excellent

Excellent

Excellent

Excellent

**Step-by-Step Prompt**

Excellent

Excellent

Excellent

Excellent

Excellent

Excellent

### DETAILED ANALYSIS

**Straightforward Prompt**

The straightforward prompt produced a general solution.

It was useful for obtaining basic information about:

CNN

Dataset

Preprocessing

Evaluation

However, it did not provide detailed project-specific requirements.

**Role-Based Prompt**

The role-based prompt instructed ChatGPT to act as a Computer Vision and Machine Learning Engineer.

This resulted in:

More professional suggestions.

Better technical details.

More project-oriented information.

Better explanation of deployment.

Constraint-Based Prompt

The constraint-based prompt provided explicit requirements.

It produced a highly structured response and covered important engineering requirements.

It was better at controlling the output because the expected structure and limitations were clearly specified.

Step-by-Step Prompt

The step-by-step prompt instructed ChatGPT to solve the problem systematically.

It provided a logical flow from:
```
Problem
   ↓
Input
   ↓
Preprocessing
   ↓
Dataset
   ↓
Model
   ↓
Training
   ↓
Evaluation
   ↓
Challenges
   ↓
Deployment
   ↓
Recommendation
```
This made the solution easy to follow.

DOES CHATGPT CONSISTENTLY PROVIDE BETTER RESULTS WITH BASIC PROMPTS?

No.

The quality of the response depends on the complexity of the problem and the amount of information provided in the prompt.

For simple questions, a straightforward prompt can be sufficient.

For complex engineering problems, structured and detailed prompts generally provide better results.

EXAMPLE WHERE A NAÏVE PROMPT WORKS WELL

## For example:

What is a CNN?

A simple prompt is sufficient because the expected answer is a basic explanation.

Another example:

What is image preprocessing?

A basic prompt can also provide an appropriate response.

However, a complex engineering problem such as:

Design an AI-based plant disease detection system including dataset selection, preprocessing, model training, evaluation, deployment and limitations.

requires a more detailed prompt.

## FINAL SELECTED PROMPTING TECHNIQUE

Selected Technique

Constraint-Based + Step-by-Step Prompting

This technique was selected because it provides:

Clear project requirements.

Structured analysis.

Better output control.

High completeness.

Technical depth.

Practical recommendations.

Consideration of real-world challenges.

This technique is suitable for engineering problems because engineering projects usually involve multiple requirements and constraints.

## REFINED / FINAL PROMPT

Act as a Senior Computer Vision and Machine Learning Engineer assisting with a final-year engineering project.

I am developing a project called LEAFGUARD – AI-Based Plant Disease Detection System.

The system should accept an image of a plant leaf, preprocess the image, classify it using a deep learning model, and predict whether the plant is healthy or affected by a particular disease.

The system should support multiple disease categories such as:

Healthy

Leaf Spot

Powdery Mildew

Rust

Bacterial Blight

Design a practical and feasible solution suitable for a final-year engineering project.

Follow these requirements:

Explain the problem definition.

Suggest a suitable plant disease dataset.

Explain image preprocessing.

Include data augmentation.

Select a suitable CNN/deep learning model.

Explain the training process.

Explain training, validation and testing.

Include accuracy, precision, recall and F1-score.

Include confusion matrix analysis.

Explain the complete system architecture.

Suggest suitable implementation technologies.

Explain real-world challenges such as poor lighting, blur, complex backgrounds and unseen diseases.

Suggest a practical deployment method.

Mention system limitations.

Suggest future improvements.

Present the solution using the following structure:

Problem Definition → System Architecture → Dataset → Preprocessing → Data Augmentation → Model Selection → Training → Evaluation → Testing → Deployment → Challenges → Limitations → Future Improvements → Final Recommendation

Keep the solution realistic, technically feasible and suitable for implementation by final-year engineering students.

ENGINEERING VALIDATION

The refined prompt was validated against the engineering requirements.

Engineering Requirement

Validation

Plant leaf image input

✓

Disease classification

✓

Image preprocessing

✓

Dataset requirement

✓

Data augmentation

✓

CNN model

✓

Model training

✓

Validation and testing

✓

Accuracy evaluation

✓

Precision evaluation

✓

Recall evaluation

✓

F1-score evaluation

✓

Confusion matrix

✓

Deployment

✓

Real-world challenges

✓

Limitations

✓

Future improvements

✓

Final-year project feasibility

✓

SYSTEM ARCHITECTURE
```
                 ┌──────────────────────┐
                 │   Plant Leaf Image   │
                 │        Input         │
                 └──────────┬───────────┘
                            │
                            ↓
                 ┌──────────────────────┐
                 │ Image Preprocessing  │
                 │ Resize / Normalize   │
                 └──────────┬───────────┘
                            │
                            ↓
                 ┌──────────────────────┐
                 │  Data Augmentation   │
                 └──────────┬───────────┘
                            │
                            ↓
                 ┌──────────────────────┐
                 │      CNN Model       │
                 │ Feature Extraction   │
                 └──────────┬───────────┘
                            │
                            ↓
                 ┌──────────────────────┐
                 │   Classification     │
                 │       Layer          │
                 └──────────┬───────────┘
                            │
                            ↓
                 ┌──────────────────────┐
                 │   Disease Prediction │
                 └──────────────────────┘
```
## SAMPLE PREDICTION
```
Input

Plant Leaf Image

Processing

Image
 ↓
Resize
 ↓
Normalize
 ↓
CNN
 ↓
Classification
```
## Output
```
Predicted Disease: Leaf Spot
Confidence: 95%
```
## ENGINEERING BENEFITS

The proposed system can provide:

Automated plant disease identification.

Faster preliminary disease detection.

Assistance to farmers and users.

Image-based disease classification.

Easy integration with web applications.

Possibility of future mobile deployment.

## LIMITATIONS

The system may provide incorrect predictions when:

The image quality is poor.

The leaf is heavily damaged.

The image contains multiple leaves.

Lighting conditions are poor.

The background is complex.

The disease is not included in the training dataset.

Two diseases have visually similar symptoms.

## FUTURE ENHANCEMENTS

Future versions can include:

Real-time camera-based detection.

Mobile application.

More plant species.

More disease classes.

Disease severity estimation.

Treatment recommendation with expert validation.

Cloud-based model deployment.

Real-time field monitoring.

Multilingual user interface.

Integration with agricultural advisory systems.

## OVERALL FINDINGS

The experiment demonstrates that different prompting techniques can produce different levels of AI-generated engineering solutions.

The Straightforward Prompt provided a basic understanding of the plant disease detection system.

The Role-Based Prompt produced a more professional and technically detailed response.

The Constraint-Based Prompt provided better control and ensured that important project requirements were addressed.

The Step-by-Step Prompt produced a systematic engineering analysis.

The combination of Constraint-Based and Step-by-Step Prompting produced the most comprehensive and useful solution.

## CONCLUSION

The experiment was successfully conducted using ChatGPT for the LEAFGUARD – AI-Based Plant Disease Detection System project.

Four prompting techniques were applied to the same engineering problem:

Straightforward Prompting

Role-Based Prompting

Constraint-Based Prompting

Step-by-Step Prompting

The generated responses were compared based on:

Relevance

Accuracy

Completeness

Clarity

Feasibility

Usefulness

The results show that a simple prompt can provide basic information, but detailed and structured prompts generate more practical engineering solutions.

The Constraint-Based + Step-by-Step prompting technique was selected as the most effective technique because it provided clear requirements, systematic analysis, technical depth and practical recommendations.

Therefore, the experiment demonstrates that effective prompt engineering can improve the quality, consistency and usefulness of AI-generated solutions for real-world engineering problems.

## RESULT

The prompt comparison experiment was successfully executed using ChatGPT. Four different prompting techniques were applied to the AI-based plant disease detection problem. The generated outputs were evaluated and compared based on relevance, accuracy, completeness, clarity, feasibility and usefulness. Constraint-Based and Step-by-Step prompting produced the most comprehensive, structured and useful engineering solution.
