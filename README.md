# Personal Portfolio (Vite)

A modern, responsive single-page portfolio built with Vite and vanilla JS/CSS. It includes:

- Sticky header with smooth scrolling and active section highlighting
- Sections: Home, About, Skills, Projects, Contact
- Light/Dark theme with persistence
- Responsive cards and grid
- Contact form wired for Formspree (optional)

## Quickstart

Prerequisites:
- Node.js 18+ recommended

Install and run locally:

```bash
npm install
npm run dev
```

Build for production and preview the build:

```bash
npm run build
npm run preview
```

## Customize Your Portfolio

Update the following placeholders:

- `index.html`:
  - `<title>Your Name — Portfolio</title>` → set your name.
- `src/main.js`:
  - Change all occurrences of `Your Name`, `Your Role`, and `you@example.com`.
  - Update the `projects` array at the top with your real projects:
    - `title`, `description`, `tags`, `link` (live demo), `repo` (source).
  - Update social links in the Contact section (GitHub, LinkedIn, Twitter/X).
  - Update the skills list under the `#skills` section as needed.
  - Replace `action="https://formspree.io/f/yourid"` with your Formspree endpoint ID if you want form submissions to email you.
- `src/style.css`:
  - Tweak colors, spacing, or fonts if desired. Theme variables are defined at the top (e.g., `--primary`).

Optional cleanups (not required):
- Remove unused starter files like `src/counter.js` and `src/javascript.svg` if you don’t need them.

## Contact Form (Formspree)

- Go to https://formspree.io/ and create a new form.
- Copy your endpoint ID, e.g. `https://formspree.io/f/abcdxyz`.
- Replace the `action` attribute in the form in `src/main.js`.

## Deployment Options

- Netlify
  - Drag-and-drop the `frontend/` folder or connect your repo.
  - Build command: `npm run build`
  - Publish directory: `dist`
- GitHub Pages
  - Build locally: `npm run build`
  - Serve `dist/` using GitHub Pages (e.g., `gh-pages` branch or GitHub Actions).

## Troubleshooting

- If you open `index.html` directly in the browser (file://), imports may fail. Use the dev server (`npm run dev`) or a simple static server.
- If ports conflict, Vite will prompt to use another port.

## License

You own your content. Code is MIT licensed by default (feel free to change).
