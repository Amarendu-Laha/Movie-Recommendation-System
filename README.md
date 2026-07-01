# 🎬 Movie Recommendation System

An end-to-end **Content-Based Movie Recommendation System** built using **Python, Natural Language Processing (NLP), Machine Learning, and Streamlit**. The application recommends movies similar to a user's selected movie by analyzing movie metadata such as genres, overviews, and taglines using **TF-IDF Vectorization** and **Cosine Similarity**.

The project also includes an interactive **Streamlit web application** that displays movie recommendations along with their posters fetched from the **TMDB API**.

---

## 📌 Project Overview

Finding movies that match a user's interests can be challenging due to the vast amount of content available across streaming platforms. This project addresses that problem by developing a **Content-Based Recommendation System** that suggests movies based on textual similarity rather than popularity or user ratings.

The complete solution includes:

- Data Cleaning & Preprocessing
- Feature Engineering
- Natural Language Processing (NLP)
- TF-IDF Vectorization
- Cosine Similarity Calculation
- Streamlit Web Application
- TMDB API Integration for Movie Posters

---

## 🚀 Features

- 🎥 Content-Based Movie Recommendation
- 🔍 Search movies using a dropdown menu
- 🖼️ Displays movie posters using TMDB API
- ⚡ Fast recommendations using pre-computed similarity matrix
- 🎨 Modern Netflix-inspired Streamlit interface
- 💾 Serialized models using Pickle for faster loading
- 📱 Responsive and user-friendly web application

---

## 🛠️ Technologies Used

| Technology | Purpose |
|------------|---------|
| Python | Programming Language |
| Pandas | Data Manipulation |
| NumPy | Numerical Computation |
| NLTK | Text Preprocessing |
| Scikit-learn | Machine Learning |
| TF-IDF Vectorizer | Feature Extraction |
| Cosine Similarity | Recommendation Engine |
| Pickle | Model Serialization |
| Streamlit | Web Application |
| TMDB API | Fetch Movie Posters |
| Jupyter Notebook | Model Development |

---

## 📂 Project Structure

```text
Movie-Recommendation-System/
│
├── app.py                     # Streamlit application
├── main.py                    # Backend logic
├── Movie_Recommendation_System.ipynb
├── movies.pkl
├── similarity.pkl
├── requirements.txt
├── assets/
│   └── screenshots/
├── README.md
└── LICENSE
```

---

## ⚙️ Project Workflow

```text
Movie Dataset
      │
      ▼
Data Cleaning
      │
      ▼
Feature Selection
      │
      ▼
Text Preprocessing (NLP)
      │
      ▼
TF-IDF Vectorization
      │
      ▼
Cosine Similarity Matrix
      │
      ▼
Recommendation Engine
      │
      ▼
Pickle Model Files
      │
      ▼
Streamlit Web Application
```

---

## 📖 How It Works

### 1. Data Collection

The movie dataset contains metadata such as:

- Movie Title
- Genres
- Overview
- Tagline
- Popularity
- Average Rating

---

### 2. Data Preprocessing

The dataset is cleaned by:

- Removing duplicate records
- Handling missing values
- Selecting relevant features
- Combining important text columns

A new **Tags** feature is created using:

- Overview
- Genres
- Tagline

---

### 3. Natural Language Processing (NLP)

The combined text is processed by:

- Converting text to lowercase
- Removing punctuation
- Removing stopwords
- Performing lemmatization

This improves the quality of feature extraction.

---

### 4. TF-IDF Vectorization

The processed text is converted into numerical vectors using **TF-IDF (Term Frequency–Inverse Document Frequency)**.

Configuration:

- Maximum Features: **50,000**
- N-Grams: **Unigrams & Bigrams**
- English Stopwords Removed

---

### 5. Cosine Similarity

Cosine Similarity calculates the similarity between movies based on their TF-IDF vectors.

Movies with the highest similarity scores are recommended to the user.

---

### 6. Recommendation Engine

The recommendation function:

- Accepts a movie title
- Finds its corresponding index
- Calculates similarity scores
- Sorts similar movies
- Returns the **Top 10 Recommendations**

---

### 7. Streamlit Application

The recommendation engine is deployed using **Streamlit** with features such as:

- Interactive UI
- Movie selection dropdown
- One-click recommendation generation
- Movie posters fetched from TMDB API
- Fast loading using serialized models

---

## 📊 Results

The system successfully:

- Cleans and preprocesses movie data
- Applies NLP techniques for feature extraction
- Converts text into numerical vectors
- Computes movie similarity efficiently
- Recommends highly relevant movies
- Displays recommendations with movie posters in a responsive Streamlit interface

---

## 📸 Application Screenshots

> Add screenshots of your application here.

### Home Page

```
assets/screenshots/home.png
```

### Recommendation Results

```
assets/screenshots/recommendations.png
```

---

## 💻 Installation

### Clone the Repository

```bash
git clone https://github.com/yourusername/Movie-Recommendation-System.git

cd Movie-Recommendation-System
```

### Create Virtual Environment

```bash
python -m venv .venv
```

### Activate Virtual Environment

**Windows**

```bash
.venv\Scripts\activate
```

**Linux / macOS**

```bash
source .venv/bin/activate
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

### Run the Application

```bash
streamlit run app.py
```

---

## 📈 Future Enhancements

- Hybrid Recommendation System
- Collaborative Filtering
- Deep Learning Models (BERT/Sentence Transformers)
- User Authentication
- Watch History
- Personalized Recommendations
- Movie Trailers
- Cloud Deployment (AWS / Streamlit Cloud)

---

## 🎯 Key Learning Outcomes

- Natural Language Processing (NLP)
- Feature Engineering
- TF-IDF Vectorization
- Cosine Similarity
- Machine Learning Pipelines
- Model Serialization with Pickle
- Streamlit Deployment
- API Integration (TMDB)
- End-to-End Project Development

---

## 🤝 Contributing

Contributions are welcome!

If you have ideas for improving the project, feel free to fork the repository, create a feature branch, and submit a pull request.

---

## 📜 License

This project is licensed under the MIT License.

---

## 👨‍💻 Author

**Amarendu Laha**

- GitHub: https://github.com/Amarendu-Laha
- LinkedIn: www.linkedin.com/in/amarendu1

If you found this project helpful, don't forget to ⭐ star the repository!

## Important

Create a .env file in vscode which will have TMDB_API_KEY=yourapikey.
You will get your api key from tmdb website.
After that create a virtual environment and then continue.(.venv)
