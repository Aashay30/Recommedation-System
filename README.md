# 🎬 Movie Recommendation System

This project implements a movie recommendation system using Natural Language Processing (NLP) techniques. By analyzing the TMDB movies and credits data, we can recommend similar movies based on user input.

## 🚀 How to Run

1. **Clone the repository**:
   ```bash
   git clone <repository_url>
   cd movie-recommendation-system

2. **Create a virtual environment**:
   ```bash
   conda create --name env python=3.9

3. **Activate the environment**:
   ```bash
   conda activate env

4. **Install the required dependencies**:
   ```bash
   pip install -r requirements.txt

5. **Run the Streamlit app**:
   ```bash
   streamlit run app.py

That's it! 🎉 You can now enjoy recommending movies!

### 📊 Data Overview

We used the TMDB movies and credits datasets and loaded them into our project. The two datasets were merged into one DataFrame for further operations.

### **Feature Engineering**

We performed feature engineering by selecting only relevant and important features:

We performed feature engineering by selecting only relevant and important features:

```python
movies = movies[['genres', 'id', 'keywords', 'original_language', 'title', 'overview', 'popularity', 'cast', 'crew']]
```

After storing this data, we applied several preprocessing techniques:

- **Stopwords removal**
- **Stemming**
- **Punctuation removal**
- **Lowercasing**

Additionally, we utilized `CountVectorizer` to convert the input data into vectors, which are then fed into the cosine similarity algorithm.

### 🔍 Recommendation Model

We created a model that uses cosine similarity to predict similar movies based on the input movie provided by the user.

### 🌐 Web Interface

An engaging web interface was built using Streamlit, allowing users to input a movie title and receive recommendations for similar movies. This makes the model easy to use and accessible for everyone!

Feel free to explore and enhance the movie recommendation experience! 🍿
