# Getting this onto GitHub Pages (for JustinTS2022)

You don't need git or the command line for this — GitHub's web UI supports drag-and-drop uploads.

## 1. Create the repo

1. Go to https://github.com/new while signed in as **JustinTS2022**.
2. Repository name: `hebron-stats` (or whatever you want — it becomes part of the URL).
3. Set it to **Public** (GitHub Pages on the free tier needs a public repo).
4. Leave "Add a README" unchecked. Click **Create repository**.

## 2. Upload the site files

1. On the new (empty) repo page, click **uploading an existing file**.
2. Drag in everything from this `hebron-site` folder — `index.html`, `player-ratings.html`, `draft-board.html`, `game-log.html`, `DEPLOY.md`, and the whole `assets` folder (drag the folder itself; GitHub preserves the structure).
3. Scroll down, click **Commit changes**.

## 3. Turn on Pages

1. In the repo, go to **Settings** → **Pages** (left sidebar).
2. Under "Build and deployment" → **Source**, choose **Deploy from a branch**.
3. Branch: `main`, folder: `/ (root)`. Click **Save**.
4. Wait a minute or two — GitHub will show a banner with your live URL, something like:

   `https://justints2022.github.io/hebron-stats/`

That's the link to share with the league.

## Updating the site later

- **Data changes** (new games, updated ratings, draft board edits): nothing to do here — the site reads live from the Google Sheet every time someone loads a page.
- **Site changes** (new pages, style tweaks, bug fixes): edit the files and re-upload through the same "uploading an existing file" flow, or ask me to make the changes and re-deliver the files.

## If a page shows "Couldn't load live data"

Almost always means the Google Sheet's sharing got changed back to private. Fix: open the Sheet → **Share** (top right) → **General access** → set to **Anyone with the link** (Viewer).
