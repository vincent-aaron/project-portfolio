# Project Portfolio

The personal portfolio website of **Vincent Aaron B. Vicente**, a developer from Bulacan, Philippines. It is a single responsive page that introduces me, lists my skills, showcases my projects with screenshots and links, and makes it easy to get in touch or download my resume.

## Sections

- **Home** – introduction and a "Let's Work Together" email call-to-action
- **About Me** – background, profile photo, and key highlights
- **Skills & Expertise** – frontend, backend, and tools
- **Projects** – cards with a screenshot, short description, tech stack, and links to the GitHub repo, README, and live demo (when available)
- **Get In Touch** – email, phone, and location
- **Resume** – downloadable PDF resume

## Featured Projects

| Project | Stack | Repository |
| --- | --- | --- |
| Tech IMS | Python, Django, PostgreSQL | [tech-ims](https://github.com/vincent-aaron/tech-ims) |
| Barangay Adjudication MIS | PHP, MySQL, JavaScript | [barangay-adjudication-mis](https://github.com/vincent-aaron/barangay-adjudication-mis) |
| Runebound | Unity, C# | [runebound](https://github.com/vincent-aaron/runebound) |
| Titan Cruise | Java, Swing, Maven | [titan-cruise](https://github.com/vincent-aaron/titan-cruise) |
| Elevating IQ | Java, Swing | [elevating-iq](https://github.com/vincent-aaron/elevating-iq) |
| Simple Calc | Java, Swing | [simple-calc](https://github.com/vincent-aaron/simple-calc) |

## Tech Stack

| Layer | Technology |
| --- | --- |
| Markup | HTML5 |
| Styling | Tailwind CSS (Play CDN) |
| Hosting | Any static host (e.g. GitHub Pages) |

No build step or dependencies are required.

## Project Structure

```
project-portfolio/
├── index.html                      # The whole site
├── Profile.png                     # Profile photo
├── BPAMIS.png                      # Barangay Adjudication MIS screenshot
├── Vicente_Vincent_Aaron_Resume.pdf
├── elevatingiq/                    # Elevating IQ screenshots
├── runebound/                      # Runebound screenshots
├── simple-calc/                    # Simple Calc screenshot
└── titan cruise/                   # Titan Cruise screenshots
```

## Running Locally

Open `index.html` in any browser, or serve the folder:

```bash
npx serve .
# or
python -m http.server 8000
```

## Deploying to GitHub Pages

1. Push the repository to GitHub.
2. Go to **Settings → Pages**.
3. Set **Source** to *Deploy from a branch*, branch `main`, folder `/ (root)`.
4. The site will be published at `https://vincent-aaron.github.io/project-portfolio/`.

## Contact

- Email: [vincent4aron@gmail.com](mailto:vincent4aron@gmail.com)
- GitHub: [vincent-aaron](https://github.com/vincent-aaron)
