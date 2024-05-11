# Spotify-Playlist-Generator(Popular Tracks Analyzer)

## Project Overview
Welcome to the Spotify Playlist Generator(Popular Tracks Analyzer) project! This open-source project is aimed at analyzing and curating playlists based on the popularity of tracks from a user's Spotify account. Leveraging the Spotify API, Python programming language, and PKCE(Proof Key for Code Exchange), this project offers valuable insights into music preferences and trends. Additionally, as part of future development plans, I aim to incorporate the MusicMatch API to analyze the genres of the liked songs fetched from Spotify. While the Spotify API provides robust music data, to the best of my knowledge, it lacks a direct genre API endpoint. Therefore I plan to integrate the MusicMatch API for more comprehensive genre analysis and playlist curation, enhancing the accuracy and relevance of curated playlists not only on popularity but also on the genres that resonate with the user's preferences. Stay tuned for updates on this exciting enhancement to the project!

## Key Features
- Fetch liked songs from Spotify using the Spotify API.
- Extract essential track details such as name, artist, album, popularity, and date added
- Dynamilcally sorts tracks based on popularity scores.
- Creates a new playlist on Spotify, adding the top 100 popular tracks.

## Project Structure
- README.md: Detailed project overview, usage instructions, and technology used.
- main.py: The Python script orchestrating the project, handling everything from API credentials setup to token exchange using PKCE for fetching liked songs, extracting data, and creating the playlist.
- index.html: Landing page for user interaction

## Getting Started
1. Access your Spotify for Developers dashboard using your Spotify account
2. Create an App: Provides you with the client ID and client secret needed to request an access token by implementing any of the authorization flows.
The OAuth2 standard for Spotify defines four grant types or flows to request and get the access token that we need to get our Spotify data. You can follow the Authorization tutorial on the Spotify for Developers page to learn more about the OAuth flows.
This project uses the authorization code with PKCE(proof key ), as it provides protection against attacks where the authorization code may be intercepted since it does not require our secret key. You can read more on the full guide for the implementation of the PKCE extension under the Authorization code with PKCE Flow.
3. Develop an HTML file to serve as landing page using GitHub pages to facilitate user interaction.
To create an HTML file, follow these steps:
   a. Navigate to the Cloned Repository Directory: Open your terminal (Command Prompt, Terminal, or equivalent).
   Use the cd command to navigate to the directory where your cloned repository is located.
   (For example:cd ~/Documents/repository-name).
   Replace Documents with the name of the directory where your cloned repository is located, and repository-name with the actual name of your cloned repository directory.
   b. Create the HTML File: Once you're in the correct directory, use a text editor or code editor in the terminal to create the index.html file. For example, you can use the nano text editor:
   (nano index.html)
   This command will open a new file named index.html in the nano editor within the terminal.
   c. Add HTML Content: In the nano editor (or any other editor you make use of), add your HTML content for the landing page. You can use the HTML code provided in this repository or create your own content.
5. Move the HTML file to your GitHub repository. Then configure your GitHub pages to access your GitHub pages url where your landing page is hosted. You can follow the Getting started tutorial on GitHub pages.
6. Make a request authorization from user's Spotify account to retrieve the authorization code, this redirects the user to Spotify for authorization by visiting the URL provided.
After authorization, Spotify will redirect back to the redirect URI with the authorization code. Then use the access token to fetch data from the Spotify Web API.
7. Run the Python script to authenticate with Spotify, fetch liked tracks, and create the playlist.

## Usage
1. Run the script to fetch liked songs and create the playlist.
2. Follow the authorzation prompt to link the application with your Spotify account.
3. After authorization, the script generates a new playlist comprising the top 100 songs by popularity.

## Technologies Used
- Python
- Request library for HTTP requests.
- Spotify API for music data access.

## Contributing
Feel free to contribute to this project by forking the repository, making changes, and creating pull requests.

## Contact
For further inquiries or collaboration oppprtunities, please reach out to [Segun Bakare](segunbakare.d@gmail.com).
