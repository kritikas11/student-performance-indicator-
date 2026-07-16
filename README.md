# Student Performance Indicator

An end-to-end Machine Learning project that predicts a student's Mathematics score based on demographic information, parental education level, lunch type, test preparation status, and exam scores.

## Features

- Data Ingestion Pipeline
- Data Transformation Pipeline
- Model Training and Evaluation
- Multiple Regression Models Comparison
- Model and Preprocessor Serialization
- Flask-based Prediction Interface

## Project Structure

```text
student-performance-indicator/
│
├── artifacts/
├── notebook/
├── src/
│   ├── components/
│   │   ├── data_ingestion.py
│   │   ├── data_transformation.py
│   │   └── model_trainer.py
│   │
│   ├── pipeline/
│   │   └── predict_pipeline.py
│   │
│   ├── exception.py
│   ├── logger.py
│   └── utils.py
│
├── templates/
├── app.py
├── application.py
├── requirements.txt
└── README.md
```

## Dataset Features

### Input Features

- Gender
- Race / Ethnicity
- Parental Level of Education
- Lunch Type
- Test Preparation Course
- Reading Score
- Writing Score

### Target

- Math Score

## Models Evaluated

- Linear Regression
- Decision Tree Regressor
- Random Forest Regressor
- Gradient Boosting Regressor
- K-Nearest Neighbors Regressor
- XGBoost Regressor
- CatBoost Regressor
- AdaBoost Regressor

The best-performing model is selected automatically using the R² score.

## Example Prediction

### Input

| Feature | Value |
|----------|----------|
| Gender | Male |
| Race/Ethnicity | Group A |
| Parent Education | Bachelor's Degree |
| Lunch | Free/Reduced |
| Test Preparation | Completed |
| Reading Score | 67 |
| Writing Score | 67 |

### Output

```text
Predicted Math Score: 66.00
```

## Running the Project

Install dependencies:

```bash
pip install -r requirements.txt
```

Train the model:

```bash
python src/components/data_ingestion.py
```

Run the Flask application:

```bash
python app.py
```

Open:

```text
http://127.0.0.1:5000
```

## Author

**Kritika Singh**

GitHub: https://github.com/kritikas11