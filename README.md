# 🎬 Movie Recommendation System  

A **content-based movie recommendation system** built using **Count Vectorization** and **K-Nearest Neighbors (KNN)**. The system suggests similar movies based on genres and allows interactive user input to fetch top recommendations with genres and similarity scores.  

---

## 🚀 Project Overview  

- **Algorithm:** Content-Based Filtering (CountVectorizer + KNN)  
- **Language:** Python  
- **Libraries:** Pandas, NumPy, Scikit-learn  
- **Goal:** Deliver highly relevant and personalized movie suggestions  

---

## 🛠 Features  

- ✅ **Content-Based Filtering:** Uses movie genres to find similarity between movies  
- ✅ **Feature Engineering:** Converts genres into numerical feature vectors for similarity analysis  
- ✅ **Interactive Input:** Users can search for a movie title and get top recommended movies  
- ✅ **Similarity Scores:** Recommendations include genres and similarity scores for transparency  
- ✅ **Efficient Data Processing:** Built using Python data science stack  

---

## 📊 Workflow  

1. **Data Loading:** Load movies dataset (title, genres, IDs)  
2. **Feature Extraction:** Transform genres using `CountVectorizer`  
3. **Modeling:** Apply `NearestNeighbors` to calculate similarity  
4. **User Input:** Search for a movie, get recommended titles with genres & similarity score  
5. **Output:** Display top `N` recommendations  

---

## 🖥 Sample Code  

```python
user_input = "Interstellar"
print("Here are similar movies: ")
for i in range(5):
    print(i, ": ", search_by_title(user_input)['title'].iloc[i])

title = 0
print("Recommendation Results: ")
print(recommendation_results(user_input))
