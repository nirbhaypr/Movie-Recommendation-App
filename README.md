# Movie-Recommendation-App

Welcome to the Movie Recommender App! This application is built using Python and Streamlit, and it allows users to get personalized movie recommendations based on their selected movie. The app leverages movie data, user ratings, and The Movie Database (TMDb) API to provide detailed recommendations, movie posters, summaries, and cast information. This webapp is now [live](https://movies-recmnd.streamlit.app).

## Features
- Movie Search: Type and select a movie from a dropdown list to search for similar movies.
-Personalized Recommendations: Get up to 20 movie recommendations based on user ratings.
-Movie Details: View movie posters, summaries, and main cast information for each recommendation.
-Customizable UI: Slider to choose the number of recommendations.
-User-Friendly Interface: Built with Streamlit for an interactive and responsive experience.

## How It Works
1. Input: Users can type the name of a movie in the search bar, and select it from the dropdown list.
2. Recommendation Engine: The app cleans the movie title and uses a combination of TF-IDF Vectorizer and Cosine Similarity to find movies with similar titles. It also uses user rating data to refine recommendations.
3. Movie Details Fetching: For each recommended movie, the app fetches the poster, summary, and cast details from the TMDb API.
4. Output: The recommended movies are displayed with their posters, summaries, and cast information in a clean, user-friendly format.

## Installation
To run this app locally, follow these steps:

1. Clone this repository:


```git clone https://github.com/yourusername/movie-recommender-app.git```

```cd movie-recommender-app```

Install the required packages:

```pip install -r requirements.txt```

Run the Streamlit app:

```streamlit run app.py```

## Dataset
The app uses the following datasets:

- **movies.csv**: Contains movie titles, genres, and other metadata.
- **ratings.csv**: Contains user ratings for movies.
Make sure these CSV files are in the same directory as your app.py file.

## API Key
This app uses the TMDb API to fetch movie details. You will need to obtain an API key from The Movie Database (TMDb) and replace the placeholder in the code with your API key:

```api_key = 'your_tmdb_api_key_here'```

## Usage
1. Start the app using the command streamlit run app.py.
2. Type a movie name into the search box and select it from the dropdown.
3. Adjust the number of recommendations using the slider.
4. Click the "Recommend" button to get personalized movie recommendations.
5. View the recommended movies with posters, summaries, and cast information.

## Contributing
Contributions are welcome! If you have any ideas, suggestions, or find any bugs, feel free to open an issue or submit a pull request.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

## Acknowledgments
- The Movie Database (TMDb) for providing the movie data and API.
- The open-source community for the amazing libraries and tools that make this project possible.
