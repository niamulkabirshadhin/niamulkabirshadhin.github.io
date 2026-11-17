# Md. Niamul Kabir Shadin | Portfolio

A personal portfolio website built with plain HTML, CSS and JavaScript. There is no build step and no dependencies, so it runs on GitHub Pages as it is.

**Live site:** https://niamulkabirshadhin.github.io

## Features

- Animated hero with a typing effect and an interactive dot-network background
- Sections for About, Skills, Projects, Education, Certifications and Contact
- Scroll-reveal animations and animated counters
- Project filters by technology
- Built-in project manager: add projects by hand, fill them in from a GitHub link, or sync your public repositories
- Fully responsive, and respects the reduced-motion setting

## Files

| File | Purpose |
|------|---------|
| `index.html` | The whole website (HTML, CSS and JavaScript) |
| `projects.json` | Projects that every visitor sees, in addition to the built-in ones |
| `README.md` | This file |

## Run it locally

Open `index.html` in a browser. To test loading `projects.json` as well, serve the folder instead:

```bash
python -m http.server 8000
```

Then visit http://localhost:8000.

## Deploy with GitHub Pages

1. Create a public repository named `niamulkabirshadhin.github.io`.
2. Upload `index.html`, `projects.json` and `README.md`.
3. Open **Settings → Pages**, choose **Deploy from a branch**, select `main` and `/ (root)`, then save.
4. The site goes live in about a minute.

## Personalize

Near the top of the `<script>` in `index.html`:

```js
var USER = "niamulkabirshadhin";                          // GitHub username
var LINKEDIN = "https://www.linkedin.com/in/niamul-kabir-shadin/";
```

Skills are in the `SKILLS` object, and the starting projects are in `DEFAULTS`, both in the same script.

## Add a new project

**Option 1: from the website (saved in your browser only)**
1. Open the Projects section and click **+ Add a project**.
2. Paste the GitHub link and click **Fill from GitHub**, or type the details yourself.
3. Click **Add project**.

You can also click **Sync from GitHub** to pull in all your public repositories that aren't listed yet. Remove any you don't want with the × on the card.

**Option 2: make it permanent for every visitor**
1. After adding projects in the browser, click **Copy projects.json**.
2. On GitHub, open `projects.json`, click the pencil icon, and paste the copied content.
3. Commit the change. The site updates within a minute or two.

Each entry in `projects.json` looks like this:

```json
{
  "title": "My New Project",
  "desc": "What it does in one or two sentences.",
  "tech": ["React", "Firebase"],
  "url": "https://github.com/niamulkabirshadhin/my-new-project"
}
```

## Notes

- Projects added in the browser are stored in `localStorage`, so only you see them until you copy them into `projects.json`.
- The GitHub fill and sync features use the public GitHub API, so they only work for public repositories and are subject to GitHub's rate limits.

## Contact

- Email: niamulkabirshadhin@gmail.com
- GitHub: https://github.com/niamulkabirshadhin
- LinkedIn: https://www.linkedin.com/in/niamul-kabir-shadin/
