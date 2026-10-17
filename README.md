# Sustainable Drainage for New Developments

CEG3001 · Design of Sustainable Engineering Systems · Newcastle University

Interactive, white-and-blue lecture website for students. Includes site analysis, CityCAT imagery, drainage design concepts, an interactive runoff/storage calculator, links to the original permeable paving and Newcastle Helix videos, and Vevox activity prompts.

## Publish to GitHub Pages

1. Create a new **public GitHub repository** (for example `sustainable-drainage-lecture`). If you use a private repository, confirm that your GitHub plan supports the requested Pages visibility.
2. Upload **all the contents of this folder to the repository root**, including `index.html`, the entire `media/` folder, `poll_assets/` if you want the poll reference image, and `.nojekyll`. Do **not** upload only `index.html` — it would leave pictures missing.
3. In GitHub, open **Settings → Pages**. Under **Build and deployment**, select **Deploy from a branch**, then the **main** branch and **/(root)**. Save.
4. Wait for GitHub to publish and display your Pages link (typically `https://YOUR-USERNAME.github.io/sustainable-drainage-lecture/`). Share the actual URL with students through Canvas. Do not assume the example URL is live.

Everything needed to view the lecture content and use the calculator is static. No npm, build process, Python server, database, external CSS, or third-party JavaScript is required.

## Vevox

The website has three Vevox-ready participation prompts but does **not** host a Vevox poll itself. Create/activate polls in your university Vevox account and show results using Vevox. The poll image is at `poll_assets/Arthurs_Hill_Vevox_Pin_on_Image.jpg`.

To show the **same session ID to every student on GitHub Pages**, edit `index.html` and change the single JavaScript line:

```js
const PUBLISHED_VEVOX_SESSION = '';
```

to your real 9-digit ID, for example `const PUBLISHED_VEVOX_SESSION = '123456789';` (example ID only). Commit and push the change **before class**. If left blank, use the Vevox session join details shown during the lecture. The Vevox dialog also supports local per-device saving; a local save does not update the public website for other users.

Student app: https://vevox.app/ · Newcastle SSO: https://ncl.vevox.com/

## Using and editing

- Open `index.html` to view locally, or open the GitHub Pages URL.
- Navigate with ←/→ or the chapter list. `F` enables focus mode. `N` opens brief **student explanation notes**. `V` opens Vevox details.
- Main content is freely navigable; there are no fixed lecture timings.
- All images are in `media/`, referenced by relative paths so that GitHub Pages can serve them in a project repository.
- Videos, Google Earth, official policy documents, BGS mapping, and Vevox require internet access. The main website, photos, maps, and live calculator work without it after the site has loaded or when viewing a local copy.

## Source links restored from the course presentation

- Permeable paving demonstration: https://youtu.be/14cQLPZDuV0
- Newcastle Helix / Google Earth Studio video: https://youtu.be/pzz0SRLLclc
- Interactive Google Earth site: https://earth.google.com/earth/d/1mXv4cmR-HZ-YSKhRC4HYpymxA5BWHmlo?usp=sharing

These were recovered from the original PowerPoint hyperlinks. External destinations may change over time and should be checked before class.

## Before making the repo public

Some maps, photographs, and figures were sourced from the existing lecture presentation and may carry third-party copyright or redistribution restrictions. Verify licences and permissions before placing the repository on a public GitHub Pages site; public Pages usually makes the repository content publicly accessible. If necessary, replace non-redistributable images with openly licensed equivalents. Any Newcastle University branding is used here only as part of course material, not as an implied institutional endorsement of an open-source distribution.

## Technical information

- Entry point: `index.html`
- Optimised local assets: `media/` (WebP)
- Reference image for Vevox pin-on-image poll: `poll_assets/`
- No external dependencies or secrets.
