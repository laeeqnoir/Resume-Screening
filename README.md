
# Resume Screening System

A machine learning-based application that analyzes resumes and predicts suitable job categories using Natural Language Processing (NLP) and text classification.

## Features

- Extracts text from PDF and DOCX resumes.
- Cleans and preprocesses resume text.
- Converts text into numerical features using TF-IDF.
- Uses a trained machine learning classification model to predict job categories.
- Uses a label encoder to convert predicted labels into readable categories.
- Includes sample resumes for testing.

## Technologies Used

- Python
- Scikit-learn
- Pandas
- NumPy
- Streamlit
- TF-IDF Vectorization
- Natural Language Processing (NLP)
- PyPDF2
- python-docx

## Project Structure

```text
Resume-Screening/
├── app.py
├── Resume_Screening.ipynb
├── requirements.txt
├── clf.pkl
├── tfidf.pkl
├── encoder.pkl
├── sample_resume.pdf
├── sample_resume_software_engineer.pdf
├── UpdatedResumeDataSet.csv
├── README.md
├── LICENSE
└── .gitignore
```

## Installation

### 1. Clone the repository

```bash
git clone https://github.com/laeeqnoir/Resume-Screening.git
cd Resume-Screening
```

### 2. Create a virtual environment

```bash
python3 -m venv .venv
```

Activate it on macOS or Linux:

```bash
source .venv/bin/activate
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

## Run the Application

Launch the Streamlit application:

```bash
streamlit run app.py
```

Open the local URL displayed in your terminal to access the application.

## Machine Learning Workflow

1. **Data collection:** Load the resume dataset.
2. **Text preprocessing:** Clean and normalize resume text.
3. **Feature extraction:** Transform text into numerical features using TF-IDF.
4. **Model training:** Train a classification model to categorize resumes.
5. **Prediction:** Process a new resume and predict its job category.
6. **Label decoding:** Convert the predicted label into a human-readable category.

## Model Artifacts

- `clf.pkl` — Trained classification model.
- `tfidf.pkl` — Fitted TF-IDF vectorizer.
- `encoder.pkl` — Fitted label encoder.

These files allow the application to load previously trained components without retraining the model each time.

## Future Improvements

- Evaluate the model using precision, recall, F1-score, and a confusion matrix.
- Improve text preprocessing and feature engineering.
- Add model comparison and hyperparameter tuning.
- Expand support for different resume formats.
- Deploy the application for public access.
- Evaluate the system for bias and fairness across candidate groups.

## Disclaimer

This project is intended for educational and research purposes. Predictions should not be used as the sole basis for employment decisions. Resume screening systems can introduce bias and should be evaluated carefully.

## Author

**Laeeq uz zaman**

GitHub: [@laeeqnoir](https://github.com/laeeqnoir)
