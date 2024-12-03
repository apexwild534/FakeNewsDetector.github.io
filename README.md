# Fake News Detection Web Application

This project is a web application that predicts whether a news article is **fake** or **real** using machine learning techniques. The model is built using a **Passive Aggressive Classifier** and is trained on a dataset of real and fake news articles. The web app is powered by **Flask**, and the machine learning model is implemented using **scikit-learn**.

## Features

- **Input Text:** Users can input any news article text to classify it as either **fake** or **real**.
- **Web Interface:** Built using HTML, Bootstrap, and Flask for the backend.
- **API Support:** A simple API endpoint to make predictions programmatically.
- **Model:** The classifier uses a **TF-IDF vectorizer** to convert text into numerical data and a **Passive Aggressive Classifier** for the prediction.

## Tech Stack

- **Backend:** Flask, Python
- **Machine Learning:** scikit-learn, NLTK
- **Frontend:** HTML, Bootstrap, JavaScript
- **Data Processing:** TF-IDF Vectorizer, Stopwords filtering, and stemming using NLTK
- **Model:** Passive Aggressive Classifier
- **Dataset:** Fake and True news articles stored in CSV files (`Fake.csv`, `True.csv`)

## Installation

1. **Clone the repository:**
   ```bash
   git https://github.com/apexwild534/FakeNewsDetector.git
   cd FakeNewsDetector

2. **Install the required Python packages**: Make sure you have Python installed (Python 3.8+ recommended). Then run:
   ```bash
   pip install -r requirements.txt

3. **Download the NLTK stopwords**: In your Python environment, run:
   ```python
   import nltk
   nltk.download('stopwords')
   
4. **Ensure the model and vectorizer are available**: If not already present, train the model by running test.ipynb to generate model2.pkl and tfidfvect2.pkl   

## Usage
1. **Start by running:**
   ```python
   python app.py
   
2. **Access the app**: Open your browser and go to http://127.0.0.1:5000/. You should see the web interface for predicting fake news.

## Dataset
 **True.csv**: Contains real news articles.\
 **Fake.csv**: Contains fake news articles.
### Both datasets are preprocessed using the following techniques:
1. Text cleaning: Removing non-alphabetic characters.
2. Lowercasing and tokenization.
3. Stopwords removal and stemming using NLTK.

## Model
The model is a **Passive Aggressive Classifier**, trained using the following steps:\
1. Convert the news article text into a TF-IDF vector.
2. Train the model on 80% of the data and test on the remaining 20%.
3. Achieve accuracy using scikit-learn metrics.

## Acknowledgments
1. **scikit-learn** for machine learning libraries.
2. **Flask** for building the web application.
3. **NLTK** for natural language processing tools.

## Explanation
For Code Explanation refer to [Expalnation](explanation.md).

## License
This project is licensed under the *MIT License*. See the [LICENSE](mit-license) file for more details.
