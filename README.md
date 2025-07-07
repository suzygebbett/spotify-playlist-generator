# Spotify Playlist Generator

A web application built with Next.js that allows users to generate Spotify playlists based on natural language prompts using OpenAI's GPT API. Users can log in with their Spotify account, enter a prompt describing the vibe or mood, and the app creates a custom playlist on their Spotify profile.

## Features

- Spotify OAuth 2.0 login for user authentication
- Prompt input to describe the desired playlist theme or mood
- Integration with OpenAI API to generate song suggestions from prompts
- Spotify API integration to create and populate playlists in user accounts
- Modern Next.js 13+ App Router with API routes for backend logic

## Tech Stack

- [Next.js 13+](https://nextjs.org/) with App Router
- React 18
- Spotify Web API
- OpenAI GPT API
- TypeScript
- Tailwind CSS (optional, replace with your styling choice)

## Getting Started

### Prerequisites

- Node.js v18+
- Spotify Developer account and app credentials
- OpenAI API key

### Setup

1. **Clone the repo**

   ```bash
   git clone https://github.com/yourusername/spotify-playlist-generator.git
   cd spotify-playlist-generator
2. **Install dependencies**
    ```bash
    npm install
3. **Create .env.local file**
    ```env
    SPOTIFY_CLIENT_ID=your_spotify_client_id
    SPOTIFY_CLIENT_SECRET=your_spotify_client_secret
    SPOTIFY_REDIRECT_URI=http://localhost:3000/api/auth/callback
    OPENAI_API_KEY=your_openai_api_key
4. **Register redirect URI**
    Go to the Spotify Developer Dashboard, select your app, and add the redirect URI exactly as in .env.local (e.g., http://localhost:3000/api/auth/callback or your local IP URL).
5. **Run development server**
    ```bash
    npm run dev
6. Open http://localhost:3000 in your browser and login with Spotify to get started!

## Folder Structure



## Authentication Flow

1. User clicks **Log in with Spotify** button.  
2. App redirects user to Spotify’s OAuth consent screen.  
3. After successful login, Spotify redirects back to your app’s `/api/auth/callback` endpoint.  
4. Your app exchanges the code for an access token.  
5. Access token is stored (e.g., in a secure cookie) and used for subsequent Spotify API requests.  

## Contact
Created by Suzannah Gebbett (suzannahgebbett@gmail.com). Feel free to open issues or contribute.

If you want, I can help to customise this further - jsut let me know!

