
## Spylt

Spylt is a small, modern marketing website built with Vite + React. It highlights product flavors, nutrition information, testimonials, and short promo media in a clean, responsive layout.

Why this repo
- Component-driven UI for easy content updates and maintenance
- Lightweight tooling for fast local development and builds

Features
- Flavor slider and highlighted product sections
- Nutrition & ingredient details
- Testimonials and media-rich sections (video/images)
- Reusable components for quick iteration

Tech stack
- Vite (dev server & build)
- React (JSX)
- GSAP (& @gsap/react) for animations
- Tailwind CSS (present in dependencies) and plain CSS

Prerequisites
- Node.js (LTS) and npm

Quick start (PowerShell)
```powershell
npm install
npm run dev
```

Useful scripts (from `package.json`)
- `npm run dev` — start development server (vite)
- `npm run build` — production build
- `npm run preview` — preview production build locally
- `npm run lint` — run ESLint

Project layout (top-level)
- `index.html`, `vite.config.js`, `package.json`
- `public/` — static assets (fonts, images, videos)
- `src/` — application source
  - `App.jsx`, `main.jsx`, `index.css`
  - `components/` — UI components (NavBar, FlavorSlider, ClipPathTitle, etc.)
  - `sections/` — page sections (HeroSection, FlavorSection, NutritionSection, FooterSection, ...)
  - `constants/` — shared values

Development notes
- Vite provides fast HMR — run `npm run dev` and open the local URL it prints.
- Run `npm run lint` before submitting changes.
- Animations are handled with GSAP; look for imports from `gsap` or `@gsap/react` in components.

Deployment
- Build with `npm run build` and deploy the `dist/` folder to any static host (Vercel, Netlify, GitHub Pages, etc.).

Contributing
- Fork, create a feature branch, and submit a PR with a clear description. Small, focused PRs are preferred.