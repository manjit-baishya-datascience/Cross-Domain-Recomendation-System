# **Cross-Domain Recommendation System**

## **Overview**
This project implements a cross-domain recommendation system using datasets from multiple domains (movies, music, and books). The goal is to leverage user interactions across these domains to improve recommendation accuracy.

## **Project Structure**
This project is organized into several key components:

- **Data**: User-item interaction datasets for movies, music, and books.
- **Preprocessing**: Cleaning and structuring data for recommendation modeling.
- **Modeling**: Applying collaborative filtering techniques.
- **Evaluation**: Assessing the performance of the recommendation system.
- **Pipeline**: The complete workflow from data preparation to recommendation generation.

## **Data**
The dataset consists of user interaction data across three domains:

- **Movies**: User ratings for different movies.
- **Music**: User ratings for music items.
- **Books**: User ratings for books.

### **Data Loading**
Data is loaded from text files with tab-separated values. The key attributes include:

- **user_id**: Unique identifier for each user.
- **item_id**: Unique identifier for each movie, music, or book.
- **rating**: User-provided rating for the item.

## **Data Preprocessing**
Preprocessing steps include:

- **Filtering relevant columns** (user_id, item_id, rating).
- **Handling missing values** to ensure data consistency.
- **Merging datasets** to prepare cross-domain interactions.

## **Modeling**
A collaborative filtering approach is used for recommendations. The key steps include:

- **Building interaction matrices** to represent user-item relationships.
- **Applying matrix factorization techniques** such as Singular Value Decomposition (SVD).
- **Generating recommendations** based on learned user and item embeddings.

## **Evaluation**
The performance of the recommendation system is assessed using:

- **User interaction validation** to check recommendation relevance.
- **Comparing rating predictions** with actual user ratings.

## **Pipeline**
The end-to-end pipeline follows these steps:

1. Load and preprocess data from multiple domains.
2. Train a collaborative filtering model.
3. Generate and evaluate recommendations.

## **Testing the Model**
The trained model is tested with various user interactions to demonstrate its effectiveness.

### **Example Recommendations:**

- **User 1**: Recommended Movies - [Movie A, Movie B, Movie C]
- **User 2**: Recommended Music - [Song X, Song Y, Song Z]
- **User 3**: Recommended Books - [Book P, Book Q, Book R]

## **Requirements**
To run this project, install the following Python libraries:

```bash
pip install pandas numpy scikit-learn
```
