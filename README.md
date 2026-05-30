# 🎬 Movie Recommendation System

A content-based movie recommendation system built using **Python**, **TF-IDF Vectorization**, **Cosine Similarity**, **FastAPI**, and **Streamlit**.

The application recommends movies based on plot descriptions and metadata, allowing users to discover similar movies through an interactive web interface.

---

## 🚀 Features

- Search movies by title
- Content-based recommendations using NLP
- TF-IDF vectorization of movie descriptions
- Cosine similarity-based matching
- Movie details page
- Poster and backdrop display
- Genre-based recommendations
- FastAPI backend
- Streamlit frontend
- Responsive grid layout

---

## 🧠 Recommendation Engine

The recommendation system uses:

### 1. Data Processing

Movie metadata is cleaned and processed to create a combined text representation using features such as:

- Genres
- Overview
- Tagline
- Production Companies
- Original Language

### 2. TF-IDF Vectorization

Movies are converted into numerical vectors using TF-IDF Vectorization. This helps identify the importance of words in a movie description while reducing the impact of commonly occurring words.

### 3. Cosine Similarity

The similarity between movies is calculated using Cosine Similarity. Movies with the highest similarity scores are recommended to users.

---

## 🛠️ Tech Stack

### Backend
- FastAPI
- Pandas
- NumPy
- Scikit-learn

### Frontend
- Streamlit

### Machine Learning
- TF-IDF Vectorization
- Cosine Similarity

### External API
- TMDB (The Movie Database)

---

## 📁 Project Structure

```text
movie-recommendation-system/
│
├── app.py                 # Streamlit frontend
├── main.py                # FastAPI backend
├── requirements.txt
│
├── df.pkl                 # Movie dataset
├── indices.pkl            # Title-index mapping
├── tfidf.pkl              # Trained TF-IDF vectorizer
├── tfidf_matrix.pkl       # TF-IDF feature matrix
│
├── .gitignore
└── README.md
```

---

## ⚙️ Installation

### Clone the Repository

```bash
git clone https://github.com/AyushiSoni01/movie-recommendation-system.git
cd movie-recommendation-system
```

### Create Virtual Environment

#### Windows

```bash
python -m venv .venv
.\.venv\Scripts\Activate
```

#### Linux/macOS

```bash
python -m venv .venv
source .venv/bin/activate
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

---

## ▶️ Running the Backend

```bash
uvicorn main:app --reload
```

Backend will be available at:

```text
http://127.0.0.1:8000
```

---

## ▶️ Running the Frontend

```bash
streamlit run app.py
```

Frontend will be available at:

```text
http://localhost:8501
```

---

## 📊 How It Works

1. User searches for a movie.
2. The application retrieves movie metadata.
3. TF-IDF vectors are generated from movie descriptions.
4. Cosine similarity is calculated between movies.
5. The most similar movies are selected.
6. Recommendations are displayed with posters and details.

---

## 📸 Screenshots

Add screenshots of:

- Home Page
- Search Results
- Movie Details Page
- Recommendation Section

Example:

```text
screenshots/
├── home.png
├── search.png
├── details.png
└── recommendations.png
```

---

## 🔮 Future Improvements

- Hybrid recommendation system
- Collaborative filtering
- User ratings and reviews
- Personalized recommendations
- User authentication
- Watchlist functionality
- Deep learning embeddings
- BERT/Sentence Transformer recommendations
- Recommendation analytics dashboard

---

## 🎓 Learning Outcomes

This project demonstrates:

- Natural Language Processing (NLP)
- Recommendation Systems
- Feature Engineering
- Information Retrieval
- REST API Development
- Frontend and Backend Integration
- Machine Learning Model Deployment

---

## 👩‍💻 Author

**Ayushi Soni**

---

## 📜 License

This project is intended for educational and portfolio purposes.
