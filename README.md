# Resume Classification Using Natural Language Processing

## Introduction:
This project aims to automate the resume classification process in the Human Resources Management (HRM) department, reducing the need for human intervention and streamlining the hiring process.

## Objectives:
- To classify resumes into predefined categories.
- To extract important information from resumes.
- To implement a user-friendly interface for HR personnel.

## Dataset:
The dataset consists of five different types of resumes. It is organized into a CSV file with the following columns:

- Resume Name: The name of the resume file.
- Resume Text: The content of the resume.
- Labels: The classification labels corresponding to each resume.

## Data Preprocessing
1. Text Cleaning:
- Tokenization: Splitting the text into individual words.
- Stopword Removal: Eliminating common words that add little value (e.g., "and," "the").
- Punctuation and Number Removal: Stripping out unwanted characters.
2. Stemming and Lemmatization:
- Applying stemming and lemmatization to reduce words to their base forms.
3. Feature Extraction:
- TF-IDF Vectorizer: Used to convert the cleaned text data into numerical features suitable for machine learning algorithms.
4. Data Balancing:
- SMOTE (Synthetic Minority Over-sampling Technique): Applied to balance the dataset, ensuring that all resume categories are adequately represented.

## Model Training:
Ten different classification models were evaluated, including:
- Logistic Regression
- Decision Trees
- Random Forests
- Support Vector Machines (SVM)
  and others.

## Results:
Logistic Regression was identified as the best-performing model based on accuracy metrics obtained from both training and testing datasets. The model demonstrated effective classification capabilities across all resume types.

## Deployment
The trained Logistic Regression model and the TF-IDF vectorizer were saved to the local machine. For deployment, I used Streamlit, which provides a simple interface for users to input a resume and receive:
- The predicted type of resume.
- Key information extracted from the resume text.

## Conclusion
This project successfully automates the resume classification process, making it easier for HR personnel to evaluate candidates efficiently. The deployment of the model via Streamlit further enhances usability, allowing for quick and accessible resume assessments.
