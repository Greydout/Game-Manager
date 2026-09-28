# Game-Manager
A modern Windows game library manager that brings your Steam, Epic Games, GOG and local game libraries into one place, automatically enriching titles with metadata, artwork, screenshots and YouTube trailers while giving you a clean, unified view of your entire PC game collection.


## Features

- 🎮 Unified game library
- 🟦 Steam library support
- ⬛ Epic Games library support
- 🟣 GOG library support
- 📁 Local game folder scanning
- 🔎 Automatic game identification and metadata matching
- 🖼️ Automatic cover artwork
- 🌄 Hero/background artwork
- 📸 Game screenshots
- ▶️ YouTube trailers
- 📝 Game descriptions, genres, developers, publishers and release dates
- 💾 Local artwork and metadata caching
- 🔄 Automatic metadata refresh and retry
- 🛠️ Manual game matching when automatic matching is not possible
- ▶️ Launch games directly from your library
- 🎨 Modern Windows interface
- 📐 Adjustable game card sizing
- ⚡ Designed to handle large game libraries

## How It Works

GAME MANAGER scans supported game libraries and configured folders to discover installed games.

Once a game is discovered, the application attempts to identify the title and automatically enrich the library with:

- Game title and release information
- Description
- Developer and publisher
- Genres
- Cover artwork
- Hero artwork
- Screenshots
- YouTube trailer

Metadata and media are cached locally so the library remains fast and does not need to download the same assets every time the application starts.

If metadata cannot be retrieved during the first attempt, the application can retry incomplete games without requiring the entire library to be rebuilt.

## Supported Libraries

| Library | Support |
| --- | --- |
| Steam | ✅ |
| Epic Games | ✅ |
| GOG | ✅ |
| Local folders | ✅ |

Additional launchers and libraries may be added in future releases.

## Requirements

- Windows 10 or Windows 11
- .NET 10 Desktop Runtime
- Internet connection for metadata, artwork, screenshots and trailers

