# PasteDrive

Never mistype your car plate again. Tap a saved plate to copy it and open your parking website — just paste and submit.

## Features

- **One-tap workflow** -- tap a plate card to copy the number and open your parking page
- **Multiple plates** -- save as many plates as you need, each with a label
- **Multiple parking locations** -- save different parking websites, tap to switch between them
- **Reorder plates** -- move plates up/down so your most-used is on top
- **Launch animation** -- visual confirmation showing what was copied and where it's opening (can be turned off)
- **Dark / light theme** -- switch in Settings
- **Export / Import** -- backup and restore all your data as a JSON file
- **Erase options** -- erase locations, plates, or all data from Settings
- **Installable** -- add to home screen as a PWA for app-like experience
- **Offline support** -- service worker caches all assets
- **No server, no accounts** -- all data stays in your browser's localStorage on your device
- **No tracking** -- no analytics, no cookies, no telemetry
- **Open source** -- all code is readable, no minification, no hidden logic

## Files

| File | Purpose |
|------|---------|
| `index.html` | The entire app (UI, logic, styles, all inline) |
| `sw.js` | Service worker (caches the page for offline use) |
| `manifest.json` | PWA config (app name, icon, display mode) |
| `icon.svg` | App icon |

## How to Use

1. Tap **+** and add a parking location (label + website URL)
2. Tap **+** and add your license plates (label + plate number)
3. Select which parking location to use (tap to highlight)
4. Tap a plate card -- it copies the number and opens the parking page
5. Paste the plate number into the parking form and submit

## Privacy & Data Handling

**Your data is not stored on any server or cloud.** All data -- plate numbers, parking URLs, preferences -- is saved only in your browser's localStorage on your device. PasteDrive does not send, upload, or store your data anywhere else.

**What PasteDrive does:**
- Saves plate numbers and parking URLs in your browser's localStorage
- Copies a plate number to your clipboard when you tap it
- Opens the parking URL you configured in a new tab

**What PasteDrive does NOT do:**
- Does not send data to any server
- Does not use analytics or tracking
- Does not set or read cookies
- Does not interact with the parking website on your behalf -- you paste and submit manually

**Hosting:** This app is hosted on GitHub Pages. While PasteDrive itself does not collect any data, GitHub may collect standard server access logs (IP address, browser type) as part of operating their hosting service. See [GitHub's Privacy Statement](https://docs.github.com/en/site-policy/privacy-policies/github-general-privacy-statement) for details.

**Third-party parking websites:** When you tap a plate, PasteDrive opens a parking website URL that you configured. That website has its own privacy policy. PasteDrive does not control what those websites do with your data.

**GDPR note:** License plate numbers are considered personal data under GDPR as they can be linked to a vehicle owner. Since PasteDrive processes this data entirely on your device, you remain the sole controller of your data. You can view, edit, delete, export, or erase all data at any time from within the app.

**Data persistence:**
- Your data persists in your browser's localStorage until you clear it
- Use Export (in Settings) to keep a backup

## Tech Stack

- Vanilla HTML / CSS / JS -- no frameworks, no build tools, no external dependencies
- Service Worker for offline caching
- System fonts only (no external font loading)

## License

MIT

