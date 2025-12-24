# Music Recommendation System

An era of digital music growth has made discovering new music tailored to individual preferences a complex task. This project addresses this challenge by developing a machine learning-based music recommendation system capable of proposing songs to users based on their listening history and item popularity.

## 🚀 Overview
The goal of this system is to predict the preference a user would give to a track and provide accurate, personalized recommendations. This project explores multiple recommendation strategies, primarily focusing on:
* **Popularity-Based Recommenders:** Suggesting songs based on global listening counts.
* **Content-Based Filtering:** Leveraging item features to find similarities.
* **Collaborative Filtering:** Predicting user preferences by analyzing the behaviors of similar users (e.g., SVD/Matrix Factorization).

## 📊 Dataset
The project utilizes a subset of the **Million Song Dataset**, specifically the *Taste Profile Subset*.
* **Data Source:** [Million Song Dataset](http://millionsongdataset.com/)
* **Characteristics:** Contains audio features and metadata for contemporary popular music tracks.
* **Key Files:** * `10000.txt`: User listening activity (User ID, Song ID, Play Count).
    * `song_data.csv`: Metadata (Song ID, Title, Artist, Release).

## 🛠️ Tech Stack
* **Language:** Python
* **Libraries:** * `Pandas`, `NumPy` (Data Manipulation)
    * `Matplotlib`, `Seaborn` (Visualization)
    * `Scikit-learn` (Model Building & Evaluation)
    * `Recommenders` (Custom utility classes for recommendation algorithms)

## 📖 Project Workflow
1.  **Data Loading & Merging:** Combining user log files with song metadata to create a unified dataset.
2.  **Exploratory Data Analysis (EDA):** * Analyzing the most popular songs and artists.
    * Understanding user play count distributions.
    * Subsetting data to focus on frequent listeners and popular tracks for computational efficiency.
3.  **Preprocessing:** Cleaning text data, handling duplicates, and aggregating listening history.
4.  **Model Implementation:**
    * **Popularity Model:** A baseline model that recommends the most listened-to songs to all users.
    * **Similarity Model:** Recommending songs similar to a user's previous history based on co-occurrence.
5.  **Evaluation:** Measuring the performance of the system using Precision-Recall metrics.

## 💻 How to Run
1. Clone the repository:
   ```bash
   git clone [https://github.com/prithankurdasgupta30/Song-Recommendation-System.git](https://github.com/prithankurdasgupta30/Song-Recommendation-System.git)
