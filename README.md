# 🎬 Movie Recommendation System

A content-based movie recommendation system using Natural Language Processing (NLP) techniques, specifically CountVectorizer, to provide personalized movie suggestions based on movie descriptions, genres, cast, and crew information.

## 📋 Overview

This system analyzes movie content using NLP to generate recommendations by:
- Processing movie descriptions and metadata
- Converting text data into numerical features using CountVectorizer
- Calculating movie similarities using cosine similarity
- Providing personalized movie recommendations

## 🛠️ Tech Stack

- Python 3.8+
- scikit-learn (CountVectorizer, Cosine Similarity)
- pandas
- numpy
- NLTK
- Streamlit (for web interface)

## 🚀 Features

- Content-based movie recommendations
- Text preprocessing and vectorization
- Similarity score calculation
- Interactive web interface
- Real-time recommendations

## 📊 Dataset

The system uses the TMDB movie dataset containing:
- Movie titles and descriptions
- Cast and crew information
- Genres
- Release dates
- User ratings

## 💻 Installation

```bash
# Clone the repository
git clone https://github.com/parthalathiya03/Movie_Recommenadation.git
cd Movie_Recommenadation

# Create virtual environment
python -m venv venv
source venv/bin/activate  # For Linux/Mac
venv\Scripts\activate     # For Windows

# Install required packages
pip install -r requirements.txt
```

## 🎯 Usage

### Running the Web Application
```bash
streamlit run app.py
```

### Using the Python API
```python
from recommender import MovieRecommender

# Initialize recommender
recommender = MovieRecommender()

# Get recommendations
recommendations = recommender.get_recommendations("The Dark Knight")
```

## 🔧 Implementation Details

### Text Processing Pipeline
1. Text cleaning and preprocessing
2. Stop words removal
3. CountVectorizer transformation
4. Cosine similarity calculation

### Recommendation Algorithm
1. Convert movie features to vectors using CountVectorizer
2. Calculate similarity matrix using cosine similarity
3. Rank movies based on similarity scores
4. Return top N similar movies

## 📁 Project Structure
```
Movie_Recommenadation/
├── data/                     # Dataset files
├── models/                   # Trained models
├── src/                      # Source code
│   ├── preprocessing.py      # Data preprocessing
│   ├── vectorizer.py        # Text vectorization
│   ├── recommender.py       # Recommendation logic
│   └── utils.py             # Utility functions
├── notebooks/               # Jupyter notebooks
├── static/                  # Static files
├── templates/              # HTML templates
├── app.py                  # Streamlit application
├── requirements.txt        # Dependencies
└── README.md              # Documentation
```

## 📊 Model Performance

- Average recommendation time: < 1 second
- Similarity score threshold: 0.3
- Top-N recommendations: 5-10 movies

## 🌟 Example

```python
Input: "The Dark Knight"

Output:
1. Batman Begins (Similarity: 0.87)
2. The Dark Knight Rises (Similarity: 0.82)
3. Batman v Superman (Similarity: 0.76)
4. Justice League (Similarity: 0.71)
5. Inception (Similarity: 0.65)
```

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the project
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📜 License

Distributed under the MIT License. See `LICENSE` for more information.

## 👥 Contact

Parth Lathiya - [Your Email]
Project Link: [https://github.com/parthalathiya03/Movie_Recommenadation](https://github.com/parthalathiya03/Movie_Recommenadation)

## 🙏 Acknowledgments

- TMDB for the movie dataset
- scikit-learn community
- Streamlit for the web framework
- Contributors and collaborators

---
⚡️ Powered by NLP & Machine Learning
