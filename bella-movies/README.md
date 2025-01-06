Bella Movie App

A React-based movie search and management app that allows users to explore popular movies, search for specific movies, and manage their favorite list. The app is built using React, React Router, and Context API, and styled using modular CSS.

Features
	•	Browse Popular Movies: View a list of trending movies fetched from the TMDB API.
	•	Search Movies: Search for movies by entering keywords in the search bar.
	•	Manage Favorites: Add movies to your favorites list and view them on a dedicated page.
	•	Responsive UI: Optimized for both desktop and mobile devices.
	•	Persistent Favorites: Favorites are stored in local storage, ensuring data is preserved across sessions.

Tech Stack
	•	Frontend: React, JavaScript, HTML, CSS
	•	Routing: React Router
	•	State Management: Context API
	•	Styling: Modular CSS

Folder Structure

src/  
│  
├── components/          # Reusable UI components (e.g., NavBar, MovieCard)  
├── contexts/            # Context API for managing global state (e.g., MovieContext.jsx)  
├── pages/               # Page components (e.g., Home, Favorites)  
├── services/            # API services (e.g., api.js for TMDB API calls)  
├── css/                 # CSS files for styling components  
├── App.jsx              # Root application component  
├── main.jsx             # Application entry point  
└── index.html           # Base HTML file  

How to Run the App
	1.	Clone the repository:

git clone https://github.com/AbelEwnetu/Webstack-Portfolio-Project-Movie-App.git  
cd /Webstack-Portfolio-Project-Movie-App/bella-movies  


	2.	Install dependencies:

npm install  


	3.	Set up your API key:
	•	Create a free account on The Movie Database (TMDB).
	•	Get your API key from your TMDB account.
	•	Open /src/services/api.js and add your API key:

const API_KEY = "your_api_key_here";  


	4.	Start the app:

npm run dev  

The app will run at http://localhost:3000.

Project Structure Breakdown

Components
	1.	NavBar: Provides navigation links to the Home and Favorites pages.
	2.	MovieCard: Displays movie details such as the title, release year, and poster, with functionality to add/remove favorites.

Pages
	1.	Home: Displays popular movies and provides a search bar to look for movies by keywords.
	2.	Favorites: Shows all movies marked as favorites and stored in local storage.

Context
	•	MovieContext: Manages global state for favorites, including adding, removing, and checking favorite movies.

Services
	•	api.js: Handles API calls to fetch popular movies and search movies using TMDB API.

CSS
	•	Each component and page has a corresponding CSS file in the css/ folder to ensure modular and maintainable styling.
Examples:
	•	NavBar.css: Styles for the navigation bar.
	•	MovieCard.css: Styles for the movie card component.
	•	Home.css and Favorites.css: Page-specific styles.

Key Highlights
	•	Responsive Design: Ensures a consistent user experience across different devices.
	•	Local Storage: Preserves the user’s favorites list even after refreshing the page.
	•	API Integration: Fetches real-time movie data using TMDB’s API.


License

This project is open-source and available under the MIT License.

Feel free to contribute or reach out with suggestions for improvement!

# React + Vite

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react/README.md) uses [Babel](https://babeljs.io/) for Fast Refresh
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react-swc) uses [SWC](https://swc.rs/) for Fast Refresh
