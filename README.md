# Game-Manager
<img width="2477" height="1377" alt="image" src="https://github.com/user-attachments/assets/a6a05e0f-365a-4ac2-b538-1bb11f6577ab" />
<img width="2553" height="1309" alt="image" src="https://github.com/user-attachments/assets/6aee7797-f67c-40f2-ad5a-bbd29bde0b77" />
<img width="2487" height="1345" alt="image" src="https://github.com/user-attachments/assets/e5fcafc0-938c-4c3c-b740-8b02ddabfd60" />


A modern Windows game library manager that brings your Steam, Epic Games, GOG, Ubisoft Connect, Battle.net, and local game libraries together in one place.

My Game Manager automatically enriches your collection with metadata, artwork, screenshots, and YouTube trailers while providing a clean, unified view of your PC game library.

## Features

- 🎮 Unified game library
- 🟦 Steam library support
- ⬛ Epic Games library support
- 🟣 GOG library support
- 🔷 Ubisoft Connect library support
- 🔵 Battle.net library support
- 📁 Recursive local game-folder scanning
- 🌐 Support for mapped drives and network locations
- 🔎 Automatic game identification and metadata matching
- 🖼️ Automatic portrait cover artwork
- 🎨 SteamGridDB artwork integration
- ✏️ Custom artwork for every game library
- 🌄 Hero and background artwork
- 📸 Game screenshots
- ▶️ Embedded YouTube trailers
- 📝 Descriptions, genres, developers, publishers, scores, and release dates
- 💾 Local artwork and metadata caching
- 🔄 Automatic metadata refresh and retry
- 🛠️ Manual game matching and metadata editing
- 🚀 Launch games directly from your library
- 🎨 Modern Windows interface
- 📐 Adjustable game-card sizing
- 🎮 Keyboard and controller navigation
- ⚙️ Configurable library sidebar
- 🔔 GitHub release update checking
- ⚡ Designed to handle large game libraries

## How It Works

My Game Manager reads supported launcher libraries and scans the local folders you choose.

Local scanning never executes detected files.

Once a game is discovered, the application can automatically enrich it with:

- Game title and release information
- Description
- Developer and publisher
- Genres and review score
- Portrait cover artwork
- Hero artwork
- Screenshots
- YouTube or provider trailers

Metadata and media are cached locally so the library remains responsive and does not need to download the same assets every time the application starts.

If metadata cannot be retrieved during the first attempt, incomplete games can be retried without rebuilding the entire library.

If automatic matching is uncertain, you can manually select the correct game or edit its information.

Right-click any game card to choose custom PNG, JPEG, or WebP artwork. Select **Reset artwork** to return to the original provider image.

## Supported Libraries

| Library | Support | Library Source |
| --- | :---: | --- |
| Steam | ✅ | Owned Steam games |
| Epic Games | ✅ | Owned Epic Games |
| GOG | ✅ | Owned GOG games |
| Ubisoft Connect | ✅ | Ubisoft Connect account cache |
| Battle.net | ✅ | Connected Battle.net account |
| Local folders | ✅ | User-selected folders and drives |

Launcher libraries include owned games that are not currently installed when the launcher or account makes that information available.

Additional launchers may be added in future releases.

## Artwork

My Game Manager supports artwork from game providers and SteamGridDB.

You can also assign custom artwork to any game:

1. Right-click the game card.
2. Select **Change artwork**.
3. Choose a PNG, JPEG, or WebP image.
4. Use **Reset artwork** to restore the provider image.

Custom artwork is copied into the application data directory and remains available after restarting the app.

## Controls

### Keyboard

- `Ctrl + F` — Focus library search
- `F5` — Refresh the current library
- `F11` — Toggle full-screen mode
- `Escape` — Return or exit full-screen mode

### Controller

- D-pad or left stick — Navigate
- `A` — Select
- `B` — Go back
- `X` — Play or pause a trailer
- Left and right shoulder buttons — Switch libraries
- Right stick — Scroll

## Privacy

My Game Manager does not include your personal library, passwords, account sessions, API tokens, browser cookies, logs, or custom artwork in its release packages.

Account sign-in occurs on the launcher provider’s real website. My Game Manager does not read or store the password entered there.

RAWG and SteamGridDB tokens are encrypted using Windows DPAPI for the current Windows account and are never stored as plaintext.

## Requirements

- Windows 10 version 2004 or later, or Windows 11
- 64-bit processor
- Internet connection for account synchronization, metadata, artwork, screenshots, trailers, and update checks
- Microsoft Edge WebView2 Runtime for embedded account pages and trailers

Official releases are self-contained and include the required .NET runtime.

Development requires the .NET 10 SDK.

## Install

Download the latest installer from the GitHub Releases page:
A portable package is also available:


The releases are currently unsigned, so Windows may display an unknown-publisher warning.

