# Movie Recommendation System

## Getting Started

This project is a content-based movie recommendation system that suggests similar movies based on user input. It utilizes **natural language processing (NLP)** and **machine learning techniques** to analyze movie metadata and compute similarity scores.

## Features

- **Data Preprocessing:**
  - Merging movie and credits datasets.
  - Extracting relevant features (genres, keywords, cast, crew, and overview).
  - Handling missing values.
- **Feature Engineering:**
  - Text processing using `ast.literal_eval` to convert stringified lists.
  - Creating a `tags` column by combining important metadata.
- **Vectorization & Similarity Computation:**
  - Using **CountVectorizer** to convert movie tags into feature vectors.
  - Computing **cosine similarity** between movies.
- **Movie Recommendation:**
  - Fetching the top 5 similar movies based on similarity scores.
- **Serialization:**
  - Saving preprocessed data and similarity matrix using `pickle` for future use.

## Installation

Ensure you have Python installed, then install dependencies:

```sh
pip install numpy pandas scikit-learn
```

## Usage

Run the script to generate movie recommendations:

```python
recommend('Gandhi')
```

### Example Output:

```
Gandhi, My Father
The Wind That Shakes the Barley
A Passage to India
Guiana 1838
Ramanujan
```

## Files

- `tmdb_5000_movies.csv` - Movie metadata.
- `tmdb_5000_credits.csv` - Cast and crew details.
- `movie_list.pkl` - Serialized movie data.
- `similarity.pkl` - Serialized similarity matrix.

## Contributing

We welcome contributions! Please follow these steps:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Commit your changes (`git commit -m 'Add a new feature'`).
4. Push to the branch (`git push origin feature-branch`).
5. Create a pull request.

## Authors & Acknowledgments

This project was developed with inspiration from various machine learning techniques and datasets available publicly.

## License

This project is open-source and available under the MIT License.

## Project Status

This project is actively maintained, and new features are being explored.





