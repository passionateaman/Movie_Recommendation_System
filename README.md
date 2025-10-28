#  Movie Recommendation System

A machine learning-based movie recommendation system that suggests similar movies using cosine similarity.

![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)
![Streamlit](https://img.shields.io/badge/Streamlit-1.28+-red.svg)

##  Features

- **Content-Based Filtering**: Recommends movies based on similarity in genres, keywords.
- **Interactive UI**: Built with Streamlit for a smooth user experience
- **Movie Posters**: Fetches real-time movie posters from The Movie Database (TMDb) API
- **10000+ Movies**: Extensive database of movies to choose from
- **Fast Recommendations**: Pre-computed similarity matrix for instant results

##  Demo

Select any movie from the dropdown and get 5 personalized movie recommendations with posters!

##  Prerequisites

Before running this project, make sure you have:

- Python 3.8 or higher
- pip (Python package manager)

##  Installation

### 1. Clone the repository

```bash
git clone https://github.com/passionateaman/Movie-Recommendation-System.git
cd Movie-Recommendation-System
```

### 2. Install required packages

```bash
pip install -r requirements.txt
```

### 3. Run the application

```bash
streamlit run app.py
```

The app will open in your browser at `http://localhost:8501`

##  Project Structure

```
Movie-Recommendation-System/
│
├── app.py                  # Main Streamlit application
├── Main.ipynb             # Jupyter notebook for model training
├── dataset.csv            # Movie dataset
├── movies_list.pkl        # Processed movie data
├── similarity.pkl         # Pre-computed similarity matrix
├── requirements.txt       # Python dependencies
├── frontend/              # Frontend assets (if any)
└── README.md             # Project documentation
```

##  How It Works

1. **Data Processing**: Movies are processed based on genres, keywords, cast, crew, and overview
2. **Vectorization**: Text data is converted to numerical vectors using CountVectorizer
3. **Similarity Calculation**: Cosine similarity is computed between all movies
4. **Recommendation**: When a user selects a movie, the system finds the top 5 most similar movies
5. **Display**: Results are shown with movie posters fetched from TMDb API

##  Technologies Used

- **Python**: Core programming language
- **Streamlit**: Web application framework
- **Pandas**: Data manipulation and analysis
- **NumPy**: Numerical computing
- **Scikit-learn**: Machine learning library for vectorization and similarity
- **Requests**: HTTP library for API calls
- **TMDb API**: Movie posters and metadata

##  Dataset

The dataset contains information about 5000+ movies including:
- Movie titles
- Genres
- Keywords
- Cast and crew
- Overview/plot
- Movie IDs for poster fetching

## Usage

1. Launch the application using `streamlit run app.py`
2. Select a movie from the dropdown menu
3. Click "Show Recommendation" button
4. View 5 similar movie recommendations with posters

##  API Key

The project uses TMDb API for fetching movie posters. The API key is included in the code for demonstration purposes. For production use, please:

1. Get your own API key from [TMDb](https://www.themoviedb.org/settings/api)
2. Replace the API key in `app.py`

##  Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the project
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

##  Acknowledgments

- The Movie Database (TMDb) for providing the API
- Streamlit for the amazing framework
- scikit-learn for machine learning tools

##  Contact

For any queries or suggestions, feel free to reach out!

---

⭐ If you found this project helpful, please give it a star!
