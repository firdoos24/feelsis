# Feelystic - Arabic Sentiment Analysis Platform

## Overview
Feelystic is a Flask-based web application for Arabic sentiment analysis. It analyzes CSV files, social media comments (Facebook, Instagram, YouTube), and integrates with Google Gemini API for chatbot functionality.

## Project Structure
```
feelystic/
├── app/
│   ├── __init__.py
│   └── routes.py
├── static/
│   └── ... (CSS, JS, assets)
├── templates/
│   └── ... (HTML templates)
├── logistic_regression_model.pkl
├── tfidf_vectorizer.pkl
├── run.py
├── requirements.txt
├── .gitignore
└── README.md
```

## Getting Started

1. **Clone the repository**  
   ```bash
   git clone <repo_url>
   cd feelystic
   ```

2. **Create virtual environment**  
   ```bash
   python3 -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install dependencies**  
   ```bash
   pip install -r requirements.txt
   ```

4. **Set up environment variables**  
   Create a `.env` file in the project root and add necessary configuration, e.g.:  
   ```
   FLASK_APP=run.py
   FLASK_ENV=development
   MONGO_URI="mongodb://localhost:27017/asa"
   SECRET_KEY="your-secret-key"
   OPENAI_API_KEY="your-openai-key"
   ```

5. **Run the application**  
   ```bash
   flask run
   ```

6. **Access the app**  
   Open your browser and go to `http://127.0.0.1:5000/`.

## License
This project is licensed under the MIT License.
