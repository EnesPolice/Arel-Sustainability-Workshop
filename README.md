# 🌊 Arel Koleji Climate & Sustainability Workshop

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](./LICENSE)
[![Website](https://img.shields.io/website?url=https%3A%2F%2Farelcalistay.org&label=website)](https://arelcalistay.org)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)
![Deployed on Vercel](https://img.shields.io/badge/Deployed%20on-Vercel-000000?logo=vercel&logoColor=white)

Website of the **Arel Koleji İklim ve Sürdürülebilirlik Çalıştayı** (Climate & Sustainability Workshop), held on October 10–11, 2026 in Istanbul.

🔗 **Live site:** [arelcalistay.org](https://arelcalistay.org)

## About

A one-page event website with an animated hero, live countdown, interactive committee cards, a two-day program, and a team section. It is a lightweight static site with no framework and no build step.

## Features

- Responsive design (desktop, tablet, mobile)
- Animated hero section with a live countdown that switches to "in progress" and "completed" states after the event starts and ends
- Committee cards with modal detail views (keyboard accessible)
- Day-by-day program timeline
- Team and speaker sections
- SEO-ready: Open Graph tags, JSON-LD event schema, sitemap, favicon set
- Zero dependencies: pure HTML, CSS, and JavaScript

## Tech Stack

- HTML5 / CSS3 (vanilla, no framework)
- Vanilla JavaScript (no libraries)
- Deployed via [Vercel](https://vercel.com) (Root Directory: `site`)

## Project Structure

```
site/
├── index.html        # whole page (styles and scripts included)
├── assets/           # logo, favicons, og-image, web manifest
├── robots.txt
└── sitemap.xml
```

## Run Locally

```bash
cd site
python3 -m http.server 8000   # then open http://localhost:8000
```

## Customizing

Personal details (team names, speaker, contact email) are replaced with placeholders in this repository:

- **Team:** `team-card` blocks in `index.html` (`data-name` and `<h4>`). To add a photo, set `data-photo="assets/team/name.jpg"`.
- **Speaker:** the `speaker-card` block.
- **Contact email:** replace `iletisim@example.com`.
- **Dates:** `EVENT_DATE` / `EVENT_END` in the countdown script, and `startDate` / `endDate` in the JSON-LD block.
- **Domain:** `canonical`, `og:url`, `og:image`, `robots.txt`, and `sitemap.xml`.

## Development Notes

This site was built with the help of AI coding assistants as part of the development process:

- **Initial structure, layout, and core components**: built with **Claude** (Anthropic), using the free tier with the Sonnet model
- **Smaller fixes and refinements**: done with **Gemini Pro** (Google)
- **Some sections and adjustments**: written and customized manually

This is disclosed transparently for anyone curious about the workflow behind the project.

## License

The source code is licensed under the [MIT License](./LICENSE). The Arel Koleji name, logo, and other brand assets in `site/assets/` are **not** covered by the MIT License and belong to their owners.

## Author

**Enes Poliçe**
