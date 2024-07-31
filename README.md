# 🌟 Discord Bot Music Player 🌟

## 📋 Description

This project aims to create a Discord bot that seamlessly integrates music playback into Discord servers, enhancing the social experience and providing an easy way for users to enjoy music together.

- 🎯 **Music Playback:**  The bot supports common audio formats (MP3, WAV, OGG) and allows users to queue songs, creating a playlist for playback in the order they are added. It provides basic controls like pause, resume, skip, restart, and volume control.
- 🛠️ **Search and Selection:** Users can search for songs by entering song titles or artist names and select a specific song from the displayed search results. The bot integrates with various music sources like YouTube, Spotify, and SoundCloud.
- 🚀 **User Interaction:** The bot uses simple and user-friendly commands for interaction, providing clear feedback and notifications about currently playing songs, queued songs, and any errors.

## 📑 Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [Hosting](#hosting)
- [API Documentation](#api-documentation)
- [License](#license)
- [Authors and Acknowledgments](#authors-and-acknowledgments)

## 💻 Installation

### 🔧 Prerequisites

- Python 3.7 or later
- pip (Python package installer)
- Discord API token

### 🚀 Setup Instructions

1. **Clone the repository:**
   - `git clone https://github.com/your-username/discord-music-bot.git`
2. **Navigate to the project directory:**
   - `cd discord-music-bot`
3. **Create a .env file:**
   - Copy the `.env.example` file to `.env`.
4. **Install dependencies:**
   - `pip install -r requirements.txt`
5. **Set your Discord API token:**
   - Open the `.env` file and set the `DISCORD_TOKEN` variable to your Discord bot's API token.
   - Get your token from the Discord Developer Portal.

## 🏗️ Usage

### 🏃‍♂️ Running the Project

1. **Run the bot:**
   - `python main.py`

### ⚙️ Commands

- **!play [song name/URL]:** Plays a song from the chosen music source.
- **!skip:** Skips to the next song in the queue.
- **!stop:** Stops the current music playback.
- **!queue:** Displays the current song queue.
- **!volume [number]:** Adjusts the playback volume.
- **!pause:** Pauses the current playback.
- **!resume:** Resumes playback.

## 🌐 Hosting

### 🚀 Deployment Instructions

You can host the bot on a cloud platform like Heroku or AWS.

#### Heroku

1. **Create a Heroku app:**
   - `heroku create discord-music-bot`
2. **Set environment variables:**
   - `heroku config:set DISCORD_TOKEN="your_discord_token"`
   - `heroku config:set SPOTIFY_CLIENT_ID="your_spotify_client_id"`
   - `heroku config:set SPOTIFY_CLIENT_SECRET="your_spotify_client_secret"`
   - (Set other necessary environment variables)
3. **Deploy the code:**
   - `git push heroku main`

### 🔑 Environment Variables

- `DISCORD_TOKEN`: Your Discord API token.
- `SPOTIFY_CLIENT_ID`: Your Spotify Client ID (if using Spotify API).
- `SPOTIFY_CLIENT_SECRET`: Your Spotify Client Secret (if using Spotify API).
- `YOUTUBE_API_KEY`: Your YouTube Data API v3 key (if using YouTube API).
- `SOUNDCLOUD_CLIENT_ID`: Your SoundCloud Client ID (if using SoundCloud API).
- `SOUNDCLOUD_CLIENT_SECRET`: Your SoundCloud Client Secret (if using SoundCloud API).

## 📜 API Documentation

### 🔍 Endpoints

- **GET /api/music/search?query=[query]**: Search for songs on the selected music source (YouTube, Spotify, or SoundCloud).
- **GET /api/music/now_playing**: Get information about the currently playing song.
- **POST /api/music/queue**: Add a song to the queue.
- **POST /api/music/skip**: Skip to the next song in the queue.
- **POST /api/music/stop**: Stop the current music playback.
- **POST /api/music/pause**: Pause the current playback.
- **POST /api/music/resume**: Resume playback.
- **POST /api/music/volume**: Adjust the playback volume.

### 🔒 Authentication

The bot uses a simple token-based authentication for its API. You need to provide your Discord bot's API token in the request headers.

### 📝 Examples

- `curl -X GET "http://localhost:5000/api/music/search?query=Imagine Dragons" -H "Authorization: Bearer your_discord_token"`

## 📜 License

This project is licensed under the MIT License.

## 👥 Authors and Acknowledgments

- **Author Name** - Spectra.codes
- **Contributor Name** - DRIX10

Special thanks to:

- [Spectra.codes](https://spectra.codes)
- [DRIX10](https://github.com/Drix10)

## 📚 Additional Resources

- [Project Website](https://example.com)
- [Documentation](https://example.com/docs)
- [Related Project](https://example.com/related)