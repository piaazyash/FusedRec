# FusedRec: Hybrid Recommendation System

A full-stack movie recommendation web app that combines collaborative filtering with content features. It uses **Neural Collaborative Filtering (NCF) with Early Fusion** to learn from the **MovieLens 1M** dataset (1M+ ratings) together with multi-source content features. A Flask REST API serves the models, and a React.js frontend lets users explore recommendations and switch between four different recommendation models.

<!-- TODO: add a screenshot or demo GIF here, e.g. ![FusedRec demo](docs/demo.gif) -->

## Features

- **Hybrid recommendations:** NCF with Early Fusion merges user-item interaction data with multi-source content features before the model learns from them.
- **Swappable models:** a modular backend lets users switch between four recommendation models from the UI.
- **Rich movie cards:** posters are fetched dynamically from the [TMDb API](https://www.themoviedb.org/documentation/api).
- **Full-stack architecture:** Flask REST API backend with a React.js frontend.
- **Large-scale training data:** built and evaluated on MovieLens 1M (1M+ records).

## Tech Stack

| Layer | Tools |
|-------|-------|
| Backend | Python, Flask (REST APIs) |
| Frontend | React.js, JavaScript, HTML/CSS |
| ML / Data | Neural Collaborative Filtering, Early Data Fusion, Scikit-learn, Pandas, NumPy |
| External API | TMDb API (movie posters) |
| Tools | Git, GitHub, Google Colab |

## How It Works

1. **Data:** MovieLens 1M ratings are combined with additional content features from multiple sources.
2. **Early Fusion:** the interaction and content features are fused at the input stage, and the fused representation is fed into the NCF model.
3. **Serving:** the Flask backend loads the trained models and exposes recommendations through a REST API.
4. **Model selection:** the frontend sends the user's chosen model to the API, so any of the four models can be used without changing the app.
5. **Presentation:** movie metadata and posters come from TMDb and are shown as cards in the React UI.

## Recommendation Models

| # | Model | Description |
|---|-------|-------------|
| 1 | NCF with Early Fusion | TODO: one-line description |
| 2 | TODO: model name | TODO: one-line description |
| 3 | TODO: model name | TODO: one-line description |
| 4 | TODO: model name | TODO: one-line description |

## Project Structure

```text
TODO: paste the output of `tree -L 2` here (or list the main folders)
```

## Getting Started

### Prerequisites

- Python 3.x
- Node.js and npm
- A free [TMDb API key](https://www.themoviedb.org/settings/api)

### 1. Clone the repository

```bash
git clone https://github.com/pyaaztechx2/FusedRec.git
cd FusedRec
```

### 2. Set up the backend

```bash
# TODO: add your real commands, for example:
# create a virtual environment
# pip install -r requirements.txt
# set your TMDb key (name the environment variable your code actually reads)
# start the Flask server
```

### 3. Set up the frontend

```bash
# TODO: add your real commands, for example:
# cd <frontend folder>
# npm install
# npm start
```

### 4. Dataset and trained models

Download [MovieLens 1M](https://grouplens.org/datasets/movielens/1m/) from GroupLens.

<!-- TODO: say where to place the dataset, and whether trained model files are included in the repo or must be generated (for example, by running a notebook in Google Colab) -->

## API

<!-- TODO: list your main endpoints, for example:

| Method | Endpoint | Description |
|--------|----------|-------------|
| GET | /api/... | ... |
-->

## Evaluation

<!-- TODO: add your results, for example RMSE, Hit Rate@10 or NDCG for each of the four models. Concrete numbers make this section the most valuable part of the README. -->

## Roadmap

- [ ] TODO: ideas for future work (for example, deployment, new models, user accounts)

## Acknowledgements

- [GroupLens](https://grouplens.org/datasets/movielens/1m/) for the MovieLens 1M dataset
- [TMDb](https://www.themoviedb.org/) for movie metadata and posters. This product uses the TMDb API but is not endorsed or certified by TMDb.

## Author

**Yash Chaugule**
[LinkedIn](https://linkedin.com/in/yashchaugule) | chaugule.yash4@gmail.com

## License

<!-- TODO: add a LICENSE file (for example MIT) and name it here -->
