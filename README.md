## Movie Recommendation System using Collaborative Filtering

This repository contains a movie recommendation system implemented using collaborative filtering techniques. The system leverages user ratings data to suggest movies similar to those that users have already rated positively.

### Dataset

The system utilizes two main datasets:

1. **Movies Dataset**: Contains information about movies including movie ID, title, and genres.
2. **Ratings Dataset**: Consists of user ratings for various movies, including user ID, movie ID, rating, and timestamp.

### Methodology

The recommendation system follows these key steps:

1. **Data Preprocessing**: 
   - The dataset is cleaned and prepared to handle missing values. 
   - Users and movies with insufficient ratings are filtered out.

2. **Building the Model**:
   - The ratings data is transformed into a sparse matrix to handle the large amount of data efficiently.
   - A Nearest Neighbors model is trained using cosine similarity as the metric. This model is used to find movies similar to a given input.

3. **Recommendation Function**:
   - A function is implemented to recommend movies similar to a given input movie.
   - The function identifies movies similar to the input based on user ratings and returns a list of recommended movies.

### Usage

1. Clone the repository to your local machine.
2. Ensure you have the required dependencies installed (Pandas, NumPy, Matplotlib, Seaborn, SciPy, Scikit-learn).
3. Load the movies and ratings datasets into the system.
4. Run the recommendation function with a movie title as input to receive recommendations.

### Example

```python
# Example Usage
movie_recommend('Fight Club')
```

### Results

The system successfully recommends movies based on user ratings and similarity metrics. Users can explore recommended movies based on their preferences and interests.

### Future Improvements

- Incorporate user profiles and preferences for personalized recommendations.
- Implement a more sophisticated algorithm to handle larger datasets efficiently.
- Enhance the user interface for better user experience.

### Contributors

- [Srihari Kamath](https://github.com/SrihariKamath)


Feel free to contribute to the project by submitting bug fixes, feature enhancements, or suggesting improvements to the codebase. Your contributions are highly appreciated!

