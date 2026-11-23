# 📌 Leads Tracker – Chrome Extension
 
A simple Chrome extension to save and keep track of leads (links) — either by typing them in or by saving the URL of the current browser tab in one click.
 
This project was built as part of the **Scrimba Fullstack Developer Path**, while learning the fundamentals of JavaScript and building my first browser extension.
 
## ✨ Features
 
- **Save input** – type any link or text and save it to your list
- **Save tab** – save the URL of the currently active tab with one click
- **Persistent storage** – leads are kept in `localStorage`, so they're still there after closing the popup or the browser
- **Clickable links** – each lead opens in a new tab
- **Delete all** – double-click the delete button to clear the whole list (double-click helps avoid accidental deletion)
## 🛠️ Built With
 
- **HTML5** – popup structure
- **CSS3** – styling
- **JavaScript** – DOM manipulation, event listeners, `localStorage`
- **Chrome Extensions API** (Manifest V3) – `chrome.tabs` to get the current tab's URL
- **Vite** – local development server
## 🚀 Getting Started
 
### Run it as a Chrome extension
 
1. Clone the repository:
```bash
git clone https://github.com/IzumiGo/leads-tracker.git
```
2. Open Chrome and go to `chrome://extensions`
3. Enable **Developer mode** (top-right corner)
4. Click **Load unpacked** and select the project folder
5. Pin the extension and click its icon to open the popup
### Run it locally in the browser
 
```bash
npm install
npm start
```
 
> Note: the **Save tab** button only works when the project runs as an extension, since it relies on the `chrome.tabs` API.
 
## 📁 Project Structure
 
```
leads-tracker/
├── index.html       # Popup structure
├── index.css        # Styles
├── index.js         # App logic (saving, rendering, storage)
├── manifest.json    # Chrome extension configuration (Manifest V3)
├── icon.png         # Extension icon
├── package.json     # Scripts and dependencies (Vite)
└── vite.config.js   # Vite configuration
```
 
## 📚 What I Learned
 
- Using `let` and `const` and working with arrays
- Selecting elements and listening to events with `addEventListener` (`click`, `dblclick`)
- Rendering lists dynamically with `innerHTML` and template strings
- Storing and retrieving data with `localStorage`, `JSON.stringify()` and `JSON.parse()`
- Handling truthy/falsy values to load saved data on startup
- Creating a Chrome extension with a `manifest.json` and using the `chrome.tabs` API
## 🔮 Possible Improvements
 
- Delete a single lead instead of the whole list
- Prevent saving empty inputs or duplicate leads
- Use `chrome.storage` to sync leads across devices
- Escape user input before rendering to avoid HTML injection
## 🙌 Acknowledgments
 
Project from [Scrimba](https://scrimba.com)'s Fullstack Developer Path.
 
