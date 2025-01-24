# Weather-App

*COMPANY*: CODTECH IT SOLUTIONS
*NAME*: GAUTAM PATIDAR
*INTERN ID*: CT08NXL
*DOMAIN*: REACT JS
*DURATION*: 4 WEEKS
*MENTOR*: NEELA SANTHOSH KUMAR



#Movie Search App
This is a simple movie search app built using React.js and the OMDb API. The app allows users to search for movies by title, displaying relevant information like the movie's year, poster, type (e.g., movie, series), and title. Below is a breakdown of the two primary components of the app: App.js and MovieCard.js.

#App.js
This is the main component that manages the state and search functionality.

#State Management:

1. movies: Stores the list of movies fetched from the OMDb API.
searchTerm: Stores the current search input from the user.
API Call:

2. searchMovies: An asynchronous function that takes the movie title, constructs a query URL, and fetches data from the OMDb API. It then updates the movies state with the search results.
3. Effect Hook (useEffect):

On initial render, the app automatically searches for the term "Batman". This is done by calling the searchMovies function inside the useEffect hook with an empty dependency array, ensuring it only runs once after the first render.
Rendering:

The app consists of a search bar where users can input a movie title, and a search icon that triggers the searchMovies function when clicked.
If movies are found, they are displayed using the MovieCard component. If no movies are found, a "No Movies Found" message is shown.



# MovieCard.js
This is a functional component that displays individual movie details.

Props:

The component receives a movie object as a prop, destructuring it to extract:
1. imdbID: Unique identifier for each movie.
2. Year: Year of release.
3. Poster: URL of the movie's poster.
4. Title: Title of the movie.
5. Type: Type of media (movie, series, etc.).
Rendering:

Displays the Year, Type, and Title of the movie.
The poster is conditionally rendered: If the Poster field is not available, a placeholder image is shown instead.
Conclusion
The app provides a simple interface for searching and displaying movies, utilizing React's state management and hooks. The App.js component handles fetching data from the API and rendering results, while MovieCard.js is responsible for displaying individual movie details. The app is lightweight and user-friendly, offering a good foundation for further enhancements or features.
