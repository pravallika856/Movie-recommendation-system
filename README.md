# 🎬 Content-Based Movie Recommendation System

![Python](https://img.shields.io/badge/Python-3.10-fcba03)
![Frontend](https://img.shields.io/badge/Frontend-Streamlit-red)
![Machine Learning](https://img.shields.io/badge/ML-Scikit--learn-blue)
![NLP](https://img.shields.io/badge/NLP-CountVectorizer-green)
![Similarity](https://img.shields.io/badge/Similarity-Cosine%20Similarity-orange)

A **content-based movie recommendation system** that recommends movies based on user preferences using **Cosine Similarity**.

The recommendation engine analyzes movie metadata and suggests similar movies by identifying patterns in genres, cast members, directors, and plot descriptions.

---

## 🚀 Features

* 🎥 Recommends movies based on user preferences
* 🧠 Uses **Content-Based Filtering**
* 📊 Built using **Count Vectorization** and **Cosine Similarity**
* 🇮🇳 Supports recommendations from a dataset containing **2,850 Indian regional films**
* 📱 Interactive web application built with **Streamlit**
* ⚡ Generates recommendations in real time

---

## 📌 Project Overview

The model was developed using a dataset containing over **7,500 movies**.

For each movie, relevant attributes such as:

* 🎭 Genres
* 🎬 Movie Title
* 👨‍🎤 Top Cast
* 🎥 Director
* 📝 Movie Overview

are combined to create a single textual representation called **tags**.

These tags are transformed into vectors using **Count Vectorizer**, after which a **Cosine Similarity Matrix** is generated.

When a user searches for a movie, the system identifies movies with the highest similarity scores and recommends them.

---

# 🏗️ System Architecture

The recommendation pipeline follows the workflow shown below:

```mermaid
flowchart LR
    A[Movie Dataset] --> B[Data Preprocessing]
    B --> C[Feature Extraction]
    C --> D[Tag Generation]
    D --> E[Count Vectorization]
    E --> F[Cosine Similarity Matrix]
    F --> G[Recommendation Engine]
    G --> H[Streamlit Web Application]
    H --> I[User Selects Movie]
    I --> G
```

---

# 📐 How Cosine Similarity Works

Cosine Similarity measures how similar two vectors are by calculating the cosine of the angle between them.

Unlike Euclidean distance, cosine similarity focuses on the **orientation** of vectors rather than their magnitude, making it highly effective for recommendation systems.

The **smaller the angle**, the **higher the similarity**.

<p align="center">
  <img src="https://user-images.githubusercontent.com/36665975/70401457-a7530680-1a55-11ea-9158-97d4e8515ca4.png" width="500">
</p>

---

# 🎯 Similarity Score

Similarity scores determine how closely related two movies are.

### Characteristics:

* Scores range from **0 to 1**
* Higher scores indicate stronger similarity
* Movies are ranked based on these scores
* Top-ranked movies are recommended to users

These scores are computed using **Cosine Similarity** on vectorized movie representations.

---

# 🛠️ Technologies Used

| Category             | Technologies      |
| -------------------- | ----------------- |
| Programming Language | Python            |
| Data Processing      | Pandas, NumPy     |
| Machine Learning     | Scikit-learn      |
| NLP                  | Count Vectorizer  |
| Similarity Metric    | Cosine Similarity |
| Frontend             | Streamlit         |
| External API         | TMDB API          |

---

# 📂 Project Structure

```text
Movie-Recommendation-System/
│
├── data/
│   └── pkl_data/
│
├── image/
│
├── app.py
├── requirements.txt
├── README.md
└── .env
```

---

# 🚀 Getting Started

## Clone the Repository

```bash
git clone https://github.com/pravallika856/movie-recommendation-system.git
cd movie-recommendation-system
```

---

## Create a Virtual Environment

```bash
python -m venv venv
```

---

## Activate the Environment

### Windows

```bash
venv\Scripts\activate
```

### Linux/macOS

```bash
source venv/bin/activate
```

---

## Install Dependencies

```bash
pip install -r requirements.txt
```

---

## Configure TMDB API Key

Obtain your API key from:

https://www.themoviedb.org/settings/api

Create a `.env` file in the project directory:

```env
API_KEY=YOUR_API_KEY
```

---

## Run the Application

```bash
streamlit run app.py
```

The application will launch at:

```text
Local URL: http://localhost:8501
```

---

# 🧠 Machine Learning Concepts Used

* Content-Based Filtering
* Feature Engineering
* Natural Language Processing
* Count Vectorization
* Cosine Similarity
* Recommendation Systems

---

# 🔮 Future Enhancements

* Implement Collaborative Filtering
* Build a Hybrid Recommendation System
* Deploy using Streamlit Cloud
* Add User Authentication
* Enable Personalized Watchlists
* Improve Recommendations using Deep Learning

---

# 📚 Learning Outcomes

Through this project, I gained practical experience in:

* Designing recommendation systems
* Applying machine learning techniques to real-world datasets
* Understanding similarity metrics
* Building interactive applications with Streamlit
* Working with external APIs

---

# 👩‍💻 Author

**Lakshmi Pravallika Polineni**

* GitHub: https://github.com/pravallika856

---


