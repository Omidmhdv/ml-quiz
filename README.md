# ML Daily Quiz PWA

A Progressive Web App that generates 10 AI-powered machine learning questions every day.
Installs as a native-feeling app icon on your phone's home screen.

## Deploy to GitHub Pages (5 minutes)

### 1. Create a GitHub repo

Go to https://github.com/new and create a **public** repo named `ml-quiz`.

### 2. Upload the files

Upload all files in this folder to the repo root:
```
ml-quiz/
├── index.html
├── manifest.json
├── sw.js
└── icons/
    ├── icon-192.png
    ├── icon-512.png
    └── apple-touch-icon.png
```

You can drag-and-drop the entire folder into the GitHub web interface.

### 3. Enable GitHub Pages

- Go to your repo → **Settings** → **Pages**
- Under "Source", select **Deploy from a branch**
- Branch: `main`, folder: `/ (root)`
- Click **Save**

After ~1 minute your app will be live at:
`https://<your-github-username>.github.io/ml-quiz/`

---

## Add to Home Screen

### iPhone (Safari only)
1. Open the URL in **Safari** (not Chrome)
2. Tap the **Share** button (bottom center)
3. Scroll down → **"Add to Home Screen"**
4. Tap **Add** → done ✓

### Android (Chrome)
1. Open the URL in **Chrome**
2. Tap the **three-dot menu** (top right)
3. Tap **"Add to Home Screen"** or **"Install App"**
4. Confirm → done ✓

---

## Features

- 🤖 AI-generated questions (new every time via Claude API)
- 📊 Score history & streak tracking (stored locally on device)
- ⏱ Timer per quiz
- ✅ Instant feedback + explanations
- 📴 Works offline (app shell cached)
- 📱 Full-screen, no browser chrome

## API Key Note

The app calls `api.anthropic.com` directly from your browser.
This is fine for personal use — your API key is handled by Claude.ai's session.
If you share the URL with others, they'll need their own Claude session or you can
add a personal API key in `index.html` (search for `headers`).
