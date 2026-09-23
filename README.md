# Portfolio site

## Files
- `index.html` — the main one-page portfolio
- `project-template.html` — duplicate this for each project's detail page (e.g. `project-frostbound.html`)
- `images/` — put your screenshots, gifs, and thumbnails here

## Deploying with GitHub Pages
1. Create a new repository on GitHub (e.g. `your-username.github.io`, or any name you like).
2. Upload the contents of this folder to the root of that repository (not inside a subfolder), so `index.html` sits at the top level.
3. In the repository, go to **Settings → Pages**.
4. Under "Build and deployment", set **Source** to "Deploy from a branch", pick the `main` branch and `/ (root)` folder, then save.
5. GitHub will give you a URL (usually `https://your-username.github.io/repo-name/` — or just `https://your-username.github.io/` if you named the repo `your-username.github.io`). It can take a minute or two to go live.

## Adding real project images
1. Drop your image/gif files into the `images/` folder.
2. In `index.html`, find the project you want to update and replace:
   ```html
   <div class="thumb placeholder"><span>Add screenshot / gif</span></div>
   ```
   with:
   ```html
   <div class="thumb"><img src="images/your-image.jpg" alt="Project Name screenshot"></div>
   ```
3. Do the same in each project's detail page (`hero-media` and `gallery-item` placeholders work the same way).

## Adding a new project page
1. Duplicate `project-template.html` and rename it, e.g. `project-frostbound.html`.
2. Fill in that file's content (title, tags, overview, role, gallery, etc).
3. In `index.html`, find that project's "View project →" link and change its `href` to your new file name.
