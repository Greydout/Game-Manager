# Game-Manager
<img width="2477" height="1377" alt="image" src="https://github.com/user-attachments/assets/a6a05e0f-365a-4ac2-b538-1bb11f6577ab" />
<img width="2553" height="1309" alt="image" src="https://github.com/user-attachments/assets/6aee7797-f67c-40f2-ad5a-bbd29bde0b77" />
<img width="2487" height="1345" alt="image" src="https://github.com/user-attachments/assets/e5fcafc0-938c-4c3c-b740-8b02ddabfd60" />


A modern Windows game library manager that brings your Steam, Epic Games, GOG, Ubisoft Connect, Battle.net, EA app, and local games together in one place.
My Game Manager enriches your collection with metadata, cover artwork, screenshots, and trailers. Organize your libraries, customize your covers, and use the animated game picker when you can’t decide what to play.
Features
- 🎮 Unified view of seven game libraries
- 🟦 Steam library support
- ⬛ Epic Games library support
- 🟣 GOG library support
- 🔷 Ubisoft Connect library support
- 🔵 Battle.net account integration
- 🔴 EA app account integration and installed-game detection
- 📁 Recursive local game-folder scanning
- 🌐 Support for mapped drives and network locations
- 🔎 Automatic game identification and metadata matching
- 🖼️ Portrait covers, hero artwork, and backgrounds
- 🎨 SteamGridDB artwork integration
- ✨ Animated WebP and GIF covers that play on hover
- ✏️ Custom artwork across every library
- 📸 Game screenshots
- ▶️ Embedded YouTube and compatible provider trailers
- 📝 Descriptions, genres, developers, publishers, scores, and release dates
- 💾 Persistent artwork and metadata caching
- 🧠 Remembered artwork searches to avoid repeated lookups
- 🛠️ Manual game matching, metadata editing, and retry options
- 🚀 Game and launcher shortcuts
- 🎰 Animated “Pick something to play” game picker
- ↕️ Drag-and-drop library ordering with a placement indicator
- 🏷️ Official launcher icons
- 🌗 Midnight and Daylight themes
- 📐 Adjustable game-card sizing
- 🎮 Keyboard and controller navigation
- ⚙️ Configurable library sidebar
- 🔔 GitHub release update checking
- ⚡ Designed to handle large game collections
- 📦 Installer and self-contained portable editions

**How It Works**

My Game Manager reads supported launcher libraries and scans the local folders you choose. Local scanning never executes detected files.
Discovered games can be enriched with:
- Game titles and release information
- Descriptions
- Developers and publishers
- Genres and review scores
- Portrait covers and hero artwork
- Screenshots
- YouTube or provider trailers
  
Metadata and media are cached locally. Existing images are reused, and completed animated-cover searches are remembered—including searches that found no suitable cover.
Local rescans still detect new or removed games while avoiding completed artwork and metadata lookups. Failed or interrupted artwork requests remain eligible for retry.
If automatic matching is uncertain, select the correct game manually or edit its information.

**Supported Libraries**

Library	Support	Library source

Steam	✅	Owned Steam games

Epic Games	✅	Owned Epic games

GOG	✅	GOG account or local Galaxy data

Ubisoft Connect	✅	Ubisoft Connect account cache

Battle.net	✅	Connected account and saved game selection

EA app	✅	Connected EA account and local installation manifests

Local folders	✅	User-selected folders, drives, and network locations



Launcher libraries include uninstalled owned games where account or launcher data makes that information available.
For Battle.net, use Manage games to choose which titles appear in your library. Your selection is preserved when you sync again.
For EA app, select Connect / sync account, sign in on EA’s page, then select Sync library. Regular Refresh updates installed status using the saved ownership library. EA imports owned PC base games; DLC and the complete EA Play subscription catalog are not imported separately.

**Organize Your Libraries**

Drag sidebar library entries into your preferred order. A placement line shows where an entry will land, and your arrangement is saved between launches.
Show or hide supported launcher libraries in Settings. Official launcher icons and a custom local-library controller icon make each collection easy to identify.

**Artwork**

My Game Manager supports provider artwork, SteamGridDB covers, and custom images.
To assign custom artwork:
1. Right-click a game card.
2. Select Change artwork.
3. Choose a PNG, JPEG, or WebP image.
4. Select Reset artwork to restore the original artwork selection.
Custom artwork is copied into the application data directory and remains available after restarting.

To enable animated covers, configure a SteamGridDB token in Settings and enable Prefer animated box art in all libraries. You can also request animated artwork for individual games from their right-click menu.
Supported animated WebP and GIF covers play while you hover over a card. Playback stops when the pointer leaves. Custom artwork takes priority, and static images remain the fallback.
Automatic refreshes reuse existing covers rather than repeatedly searching for replacements. Explicit per-game animation requests can upgrade a static cover.

**Pick Something to Play**

Open Pick something to play from the sidebar for an animated three-reel draw across your saved libraries.
- Choose which libraries participate.
- Use Installed only, enabled by default.
- Reveal a winner with cover artwork.
- Play the game, select a local installer, or open its launcher.
- Spin again to choose a different entry when another eligible game is available.


Hidden Steam, Epic, and GOG games and saved Battle.net selections are respected. Nothing launches automatically.
The picker uses saved library snapshots, so connect or refresh a library first to populate it. Each eligible library entry has equal odds; a title owned on multiple launchers can appear as separate entries.

**Controls**

Keyboard
- Ctrl + F - Focus library search
- F5 - Refresh the current library
- F11 - Toggle full-screen mode
- Escape - Return or exit full-screen mode
Controller
- D-pad or left stick - Navigate
- A - Select
- B - Go back
- X - Play or pause a trailer
- Shoulder buttons - Switch libraries in sidebar order
- Right stick - Scroll
  
**Privacy**

Release packages do not include your personal library, passwords, account sessions, API tokens, browser cookies, logs, or custom artwork.
Account sign-in takes place on the provider’s website through an embedded browser. My Game Manager does not read or store the password entered there. Browser sessions are retained locally in separate provider profiles.
RAWG and SteamGridDB tokens are encrypted using Windows DPAPI for the current Windows account. EA access tokens are held in memory during synchronization and are not written into library snapshots.

**Requirements**

- Windows 10 version 2004 or later, or Windows 11
- 64-bit processor
- Internet access for account synchronization and online content
- Microsoft Edge WebView2 Runtime for embedded account pages and trailers
Official releases are self-contained and include the required .NET runtime. Development requires the .NET 10 SDK.

**Install**

Download the latest setup installer or portable ZIP from the project’s GitHub Releases page.
For the portable edition, extract the ZIP into a writable folder and run MyGameManager.exe. Keep the included files together, including portable.marker. Portable data is stored in the adjacent Data folder.
When updating a portable installation, retain your existing Data folder.
Releases are currently unsigned, so Windows may display an unknown-publisher warning.
