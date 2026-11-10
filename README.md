# FusedRec: Hybrid Recommendation System

FusedRec is a full-stack movie recommendation web application that combines collaborative filtering with content features. It uses **Neural Collaborative Filtering (NCF) with Early Fusion** to learn from the **MovieLens 1M** dataset (1M+ ratings) together with multi-source content features. A Flask REST API serves the recommendations, and a React.js frontend lets users switch between four different recommendation models.

## Features

- **Hybrid recommendations:** NCF with Early Fusion combines user-item interaction data with multi-source content features.
- **Four swappable models:** the modular backend lets users switch between four recommendation models without changing the app.
- **Dynamic movie posters:** posters are retrieved through the TMDb API.
- **Full-stack architecture:** a Flask REST API backend and a React.js frontend.
- **Large dataset:** built on MovieLens 1M, which contains over one million ratings.

## Tech Stack

| Layer | Technologies |
|-------|--------------|
| Backend | Python, Flask (REST APIs) |
| Frontend | React.js, JavaScript, HTML/CSS |
| Machine Learning | Neural Collaborative Filtering, Early Data Fusion, Scikit-learn, Pandas, NumPy |
| External API | TMDb API |
| Tools | Git, GitHub, Google Colab |

## Architecture

The project is split into two parts:

- **Backend:** a Flask REST API that exposes the recommendation models. Each model sits behind the same interface, so the frontend can ask for recommendations from any of the four models.
- **Frontend:** a React.js single-page interface that shows recommended movies and lets the user choose the model. Movie posters are loaded from the TMDb API.

## Getting Started

### Prerequisites

- Python 3
- Node.js and npm
- A free [TMDb API key](https://www.themoviedb.org/settings/api)
- The [MovieLens 1M](https://grouplens.org/datasets/movielens/1m/) dataset from GroupLens

### Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/pyaaztechx2/FusedRec.git
   cd FusedRec
   ```

2. Install the Python dependencies for the backend and the npm packages for the frontend.
3. Add your TMDb API key so the backend can fetch movie posters.
4. Start the Flask server, then start the React development server, and open the app in your browser.

## Dataset

This project uses the [MovieLens 1M dataset](https://grouplens.org/datasets/movielens/1m/), published by GroupLens Research, which contains over one million movie ratings. Please follow GroupLens's terms when using or redistributing it.

## Acknowledgements

- [GroupLens](https://grouplens.org/) for the MovieLens dataset.
- [TMDb](https://www.themoviedb.org/) for movie posters. This product uses the TMDb API but is not endorsed or certified by TMDb.

## Author

**Yash Chaugule**
[LinkedIn](https://linkedin.com/in/yashchaugule) | chaugule.yash4@gmail.com
