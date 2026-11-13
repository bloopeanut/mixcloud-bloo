# The Blue Bus — Shuffle Radio

A single-page player that plays episodes from https://www.mixcloud.com/thebluebus/uploads/
in a fixed shuffled order, back to back, and recovers on its own after network dropouts.

## Publish on GitHub Pages
1. Create a new repository on GitHub (e.g. `bluebus-radio`). Public is required for free Pages.
2. Upload `index.html`, `.nojekyll` and this README to the repository root
   (Add file → Upload files, then Commit).
3. Settings → Pages → Build and deployment → Source: **Deploy from a branch**,
   Branch: **main**, folder **/ (root)** → Save.
4. After a minute the site is live at `https://<your-username>.github.io/bluebus-radio/`.

## Using it
- Press **▶ Start** once per browser (browsers require a click before playing sound).
- The shuffle order is the same in every browser and only changes when you click **Reshuffle** (twice).
- Your episode and position are saved in the browser and in the address bar.
  To continue in another browser, click **🔗 Copy resume link** and open that link there.
- If the connection drops, it resumes at the same spot when the connection returns.
  An episode that fails to load 5 times in a row is skipped.

## Notes
- No accounts, keys or tokens are used: the episode list comes from Mixcloud's public API,
  and audio plays through Mixcloud's official embedded player.
- Updating: replace `index.html` in the repo; Pages redeploys automatically.
