# Vincent Aaron B. Vicente — Portfolio

Personal portfolio site of **Vincent Aaron B. Vicente**, a full-stack and AI automation developer and BSIT graduate (Cum Laude) from Bulacan, Philippines.

**Live site:** https://vincent-aaron.github.io/project-portfolio/

A single `index.html` with no build step. It has light and dark themes, works on phones and desktops, is keyboard-accessible, and respects reduced-motion settings.

## Sections

Hero (résumé download, GitHub) · tech ticker · 4 featured projects · filterable archive of more projects · experience and education timeline · skills · about · contact.

## Featured projects

| Project | Stack | Live demo | Source |
| --- | --- | --- | --- |
| Vera Frei | Python, LLM agents, Playwright, SQLite | – | [vera-frei](https://github.com/vincent-aaron/vera-frei) |
| Electro Galaxy | Next.js, TypeScript, Supabase | – | [electro-galaxy](https://github.com/vincent-aaron/electro-galaxy) |
| Tech IMS | Python, Django, PostgreSQL | [tech-ims-azure.vercel.app](https://tech-ims-azure.vercel.app) | [tech-ims](https://github.com/vincent-aaron/tech-ims) |
| Barangay Adjudication MIS | PHP, MySQL, JavaScript | – | [barangay-adjudication-mis](https://github.com/vincent-aaron/barangay-adjudication-mis) |

More projects (Auto Apply, RuneBound, LogPose, Elevating IQ, Titan Cruise, CineMax, Simple Calc and others) are in the archive section of the site.

## Editing projects

All project content lives in the `PROJECTS` array near the top of the `<script>` in `index.html`. Each entry has `github`, `live` and `image` fields. A **Live demo** button appears only when `live` is set, and a placeholder tile shows when `image` is empty.

## Files

```
index.html
assets/
  Vicente_Vincent_Aaron_Resume.pdf
  profile.jpg
  one screenshot or cover image per project
ignition/     # Ignition showroom concept, live at /ignition/
otherworld/   # Otherworld Books concept, live at /otherworld/
```

## Run / deploy

Open `index.html` in a browser, or serve the folder (`npx serve .` or `python -m http.server`). It is deployed with GitHub Pages from the `main` branch root.

## Contact

- Email: [vincent4aron@gmail.com](mailto:vincent4aron@gmail.com)
- GitHub: [vincent-aaron](https://github.com/vincent-aaron)
