# 🎬 Movie App

A modern, feature-rich movie search application built with React. Discover movies, save your favorites, and rate them - all with a beautiful, responsive interface.

## ✨ Features

- **🔍 Live Movie Search** - Search for any movie with real-time results
- **⭐ Rating System** - Rate movies with an interactive star rating component
- **💾 Local Storage** - Your watched movies and ratings are saved automatically
- **⌨️ Keyboard Shortcuts** - Press `Enter` to focus search from anywhere
- **📱 Responsive Design** - Works perfectly on desktop, tablet, and mobile
- **🎨 Modern UI** - Clean, dark-themed interface with smooth animations

## 🚀 Demo

[Live Demo](#) *(Add your demo link here)*

## 🛠️ Technologies

- **React 18** - UI Library
- **OMDb API** - Movie database
- **CSS3** - Styling with custom properties
- **LocalStorage API** - Persistent data storage

## 📦 Installation

1. **Clone the repository**
```bash
git clone https://github.com/yourusername/movie-app.git
cd movie-app
Install dependencies

bash
npm install
Get an API Key

Visit OMDb API

Register for a free API key

Configure environment variables

bash
# Create a .env file in the root directory
REACT_APP_OMDB_API_KEY=your_api_key_here
Start the application

bash
npm start
The app will open at http://localhost:3000

🎯 Usage
Searching for Movies
Type at least 3 characters in the search box

Results appear instantly as you type

Click on any movie to see details

Managing Your Watchlist
Add to watched - Click the "+" button on any movie

Rate movies - Use the star rating component (1-5 stars)

Remove from list - Click the "X" button to delete

Keyboard Shortcuts
Enter - Focus the search input from anywhere on the page

Escape - Close movie details modal (if implemented)

📁 Project Structure
text
movie-app/
├── src/
│   ├── components/
│   │   ├── StarRating.js      # Reusable star rating component
│   │   ├── MovieList.js       # Displays movie grid
│   │   ├── MovieDetails.js    # Individual movie view
│   │   └── WatchedList.js     # User's watched movies
│   ├── hooks/
│   │   ├── useLocalStorageState.js  # Persistent state hook
│   │   └── useKey.js               # Keyboard event hook
│   ├── App.js                 # Main application component
│   └── index.js               # Entry point
├── public/
│   └── index.html
├── .env                       # Environment variables
└── package.json
🧩 Key Components
StarRating Component
A fully customizable star rating component:

jsx
<StarRating 
  maxRating={5}
  color="#fcc419"
  size={48}
  messages={["Terrible", "Bad", "OK", "Good", "Amazing"]}
  onSetRating={(rating) => console.log(rating)}
  defaultRating={3}
/>
Custom Hooks
useLocalStorageState

javascript
const [watched, setWatched] = useLocalStorageState([], "watched");
// Automatically syncs with localStorage
useKey

javascript
useKey("Enter", () => {
  searchInput.current.focus();
});
// Listens for keyboard events globally
🔧 Available Scripts
Command	Description
npm start	Runs app in development mode
npm test	Launches test runner
npm run build	Builds for production
npm run eject	Ejects from Create React App
🌟 Features in Detail
Live Search with AbortController
Cancels previous requests while typing

Prevents race conditions

Saves API quota

Persistent Watchlist
Movies stay saved after page refresh

Ratings are preserved

Stores in browser's localStorage

Responsive Design
Desktop: Grid layout with side panel

Tablet: Adjusted spacing and font sizes

Mobile: Stacked layout for better usability

🎨 Color Palette
css
--color-primary: #6741d9    /* Purple - Primary actions */
--color-primary-light: #7950f2  /* Lighter purple for hover */
--color-text: #dee2e6       /* Light gray - Main text */
--color-text-dark: #adb5bd  /* Darker gray - Secondary text */
--color-background-900: #212529 /* Darkest background */
--color-red: #fa5252        /* Red - Delete/Error */
🤝 Contributing
Fork the repository

Create your feature branch (git checkout -b feature/AmazingFeature)

Commit your changes (git commit -m 'Add some AmazingFeature')

Push to the branch (git push origin feature/AmazingFeature)

Open a Pull Request

📝 Future Improvements
Add user authentication

Create custom playlists

Add movie recommendations

Implement movie trailers

Add social sharing features

Create a backend with Node.js

Add movie ratings from other users

🙏 Acknowledgments
OMDb API for providing movie data

React Documentation for excellent guides

Font Awesome for icons inspiration

📄 License
This project is licensed under the MIT License - see the LICENSE file for details.

📧 Contact
Your Name - @yourtwitter - your.email@example.com

Project Link: https://github.com/yourusername/movie-app

⚡ Quick Start Commands
bash
# Clone and install
git clone https://github.com/yourusername/movie-app.git
cd movie-app
npm install

# Create .env file
echo "REACT_APP_OMDB_API_KEY=your_api_key_here" > .env

# Start development server
npm start

# Build for production
npm run build
🐛 Troubleshooting
API Key not working?

Make sure your .env file is in the root directory

Restart the development server after adding the key

Check if your API key is active on OMDb

Movies not saving?

Check if localStorage is enabled in your browser

Clear your browser cache and try again

Search not working?

Minimum 3 characters required

Check your internet connection

Verify API key is correct

Just replace the placeholder text (your name, Twitter, API key instructions, etc.) with your actual information!


Made with ❤️ by Massomeh