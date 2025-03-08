# Water Quality Detection System

This Django-based web application allows users to assess water quality by predicting whether it is suitable for irrigation or drinking. It integrates user authentication, profile management, and machine learning models for classification.

## Features

### 1. User Authentication
- Users can log in using their credentials.
- New users can register and create an account with their details.

### 2. Profile Management
- Users can view their registered profiles.

### 3. Water Quality Prediction
- Users enter water parameters such as pH, hardness, solids, sulfate, etc.
- The system applies various machine learning models to classify the water type.
- A Voting Classifier combines multiple models for improved accuracy.

### 4. Data Processing
- The application loads water quality data from a CSV file.
- CountVectorizer is used to convert text data into numerical format.
- Data is split into training and testing sets for model evaluation.

### 5. Machine Learning Implementation
- Multiple classification models are trained and evaluated, including:
  - Naïve Bayes
  - Support Vector Machine (SVM)
  - Decision Tree Classifier
  - Logistic Regression
  - K-Nearest Neighbors (KNN)
  - Stochastic Gradient Descent (SGD)
- Accuracy, classification reports, and confusion matrices are generated.
- The final prediction is stored in the database and displayed to the user.

## Installation

### Prerequisites
- Python 3.x
- Django
- scikit-learn
- Pandas
- OpenPyXL

### Steps
1. Clone the repository:
   ```bash
   git clone https://github.com/your-repo/water-quality-detection.git
   ```
2. Navigate to the project directory:
   ```bash
   cd water-quality-detection
   ```
3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
4. Apply migrations:
   ```bash
   python manage.py migrate
   ```
5. Run the Django server:
   ```bash
   python manage.py runserver
   ```
6. Open your browser and visit:
   ```
   http://127.0.0.1:8000/
   ```

## Usage
1. Register a new account or log in.
2. Enter water quality parameters.
3. Submit the form to get a prediction.
4. View the predicted water quality result.

## Contributing
Feel free to fork the project and submit pull requests for improvements.

## License
This project is licensed under the MIT License.

