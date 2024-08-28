Movie Explorer is a React-based web application that allows users to search for movies, view details, and manage a list of favorite movies. The application interacts with The Movie Database (TMDB) API to fetch and display movie data, including popular movies, movie details, and search results. Users can sign up, log in, and explore various movie categories, adding their favorite movies to a personalized list.

Features
User Authentication: Users can sign up and log in to access the application.
Search Movies: Users can search for movies by name and view the results.
Popular Movies: A list of popular movies is fetched from the TMDB API and displayed.
Movie Details: Detailed information about a selected movie, including its title, genres, overview, and runtime.
Favorites Management: Users can add movies to their favorites and view their favorite movies.
Responsive Design: The application is responsive and works on various screen sizes


Setup Instructions

Clone the Repository:
    git clone https://github.com/srinivasvarmadatla/movie-explorer.git
    cd movie-explorer


Install Dependencies:npm install

Create a .env File: Create a .env file in the root of the project and add your TMDB API key:
    
    REACT_APP_API_KEY=your_tmdb_api_key


Run the Application: npm start

The application will be available at http://localhost:3000.


The application uses The Movie Database (TMDB) API to fetch movie data. The API key should be stored in a .env file as REACT_APP_API_KEY. The following endpoints are utilized:

1>Popular Movies:https://api.themoviedb.org/3/movie/popular?api_key=your_api_key
2>Search Movies:https://api.themoviedb.org/3/search/movie?api_key=your_api_key&query=movie_name
3>Movie Details:https://api.themoviedb.org/3/movie/movie_id?api_key=your_api_key


PROJECT STRUCTURE
Context: context/favouriteContext.js - Manages favorite movies across the application.
Components:
Card.jsx - Displays movie information.
Card2.jsx - Displays favorite movies.
Pages:
Login.jsx - User login page.
Signup.jsx - User signup page.
Search.jsx - Movie search page.
Movies.jsx - Displays a list of movies based on search or popular movies.
Details.jsx - Shows detailed information about a specific movie.
Popular.jsx - Displays popular movies fetched from the API.
Favorites.jsx - Displays the user's favorite movies.

Approach
The project was built with a focus on modularity and reusability of components. React Router was utilized for client-side routing, ensuring a seamless navigation experience. State management for favorite movies was handled through React's Context API, allowing for easy access and updates across different components. The integration with TMDB's API was done using fetch, with error handling implemented to ensure a robust user experience.