# FEELIO ✨
> *"Whatever you feel, we feelio."*

An animated mood-based recommendation platform delivering instant personalized music, movies (with verified OTT streaming platforms), literature, and emergency booster vibes across Tamil Kollywood & Global culture.

![GitHub Actions Workflow](https://img.shields.io/badge/deployment-GitHub%20Pages-success?style=flat&logo=github)
![Vite](https://img.shields.io/badge/Vite-6.x-646CFF?style=flat&logo=vite&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-5.x-3178C6?style=flat&logo=typescript&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-4.x-38B2AC?style=flat&logo=tailwind-css&logoColor=white)

---

## 🌟 Key Features

1. **Member Sign In First**
   - Clean, secure email and password authentication screen.
   - Quick-fill demo option for testing (`madhusree644@gmail.com`).
   - "Remember Me" session persistence and direct logout control.

2. **10 Dynamic Mood Dimensions**
   - Happy 😊, Stressed 🤯, Heartbroken 💔, Energetic ⚡, Nostalgic 📼, Overwhelmed 🌊, Motivated 🎯, Lonely 🌧️, Creative 🎨, and Chill ☕.
   - Reactive ambient backgrounds, floating emoji particles, and expressive gradients.

3. **Authentic OTT Movie & Series Streaming Links**
   - Direct links to confirmed platforms: **Disney+ Hotstar**, **Netflix**, **Prime Video**, **Sun NXT**, **Aha**, **SonyLIV**, and **Zee5**.
   - Language filtering for **Tamil / Kollywood** and **Global / Hollywood** cinema.

4. **Curated Music & Audio Playlists**
   - Kollywood gems (Anirudh, A.R. Rahman, Yuvan Shankar Raja, Ilaiyaraaja, Harris Jayaraj) and global hits.
   - 1-click launch to Spotify search and playlists.

5. **Book & Reading Recommendations**
   - Tamil classics (Kalki's *Ponniyin Selvan*, Sujatha, Jayakanthan) paired alongside global bestsellers with direct Goodreads links.

6. **Interactive Boosters & Mood Timeline**
   - Emergency mood booster carousel with interactive 4-7-8 breathing pacer.
   - Saved mood journey timeline with date, time, and trend logging.

---

## 🚀 Quick Start (Local Development)

### Prerequisites
- [Node.js](https://nodejs.org/) (version 18 or higher recommended)
- `npm`, `pnpm`, or `yarn`

### Installation & Run

```bash
# 1. Clone the repository
git clone https://github.com/<your-username>/feelio.git
cd feelio

# 2. Install dependencies
npm install

# 3. Start local development server
npm run dev
```

Visit `http://localhost:3000` in your browser.

### Build for Production

```bash
# Create an optimized production bundle in dist/
npm run build

# Preview the production build locally
npm run preview
```

---

## 📦 Deploying to GitHub Pages (Automated CI/CD)

This repository includes a pre-configured GitHub Actions workflow in [`.github/workflows/deploy.yml`](.github/workflows/deploy.yml).

### Step-by-Step GitHub Setup:

1. **Create a GitHub Repository**:
   - Go to [github.com/new](https://github.com/new) and create a new repository (e.g., `feelio`).

2. **Push Your Code**:
   ```bash
   git init
   git add .
   git commit -m "feat: initial commit ready for GitHub deployment"
   git branch -M main
   git remote add origin https://github.com/<your-username>/feelio.git
   git push -u origin main
   ```

3. **Enable GitHub Pages**:
   - In your GitHub repository, go to **Settings** → **Pages** (in the left sidebar).
   - Under **Build and deployment** → **Source**, select **GitHub Actions**.
   - Save the setting.

4. **Automatic Deployment**:
   - Every push to the `main` branch automatically triggers the workflow.
   - You can monitor the deployment progress in the **Actions** tab.
   - Once completed, your live URL will be:
     `https://<your-username>/feelio/`

> **Note on relative paths:** `vite.config.ts` is configured with `base: './'`, ensuring all scripts and stylesheets load properly on both custom domains and GitHub Pages subpaths.

---

## 🌐 Alternative Deployments

### Vercel
1. Install Vercel CLI: `npm i -g vercel` or connect via [vercel.com](https://vercel.com).
2. Framework Preset: **Vite**
3. Build Command: `npm run build`
4. Output Directory: `dist`

### Netlify
1. Drag and drop the `dist/` directory into [Netlify Drop](https://app.netlify.com/drop), or link your GitHub repo.
2. Build command: `npm run build`
3. Publish directory: `dist`

---

## 📁 Project Architecture

```
feelio/
├── .github/
│   └── workflows/
│       └── deploy.yml      # Automated GitHub Actions workflow for Pages
├── public/                 # Static assets
├── src/
│   ├── data/
│   │   └── moodData.ts     # Mood recommendations, OTT platforms & metadata
│   ├── types/
│   │   └── index.ts        # TypeScript interfaces & types
│   ├── index.css           # Tailwind CSS styles & animations
│   └── main.ts             # Application controller & state machine
├── index.html              # Single-page HTML entry point & views
├── vite.config.ts          # Vite configuration with relative base path
├── tsconfig.json           # TypeScript configuration
├── package.json            # Project manifest & build scripts
└── README.md               # Documentation & deployment guide
```

---

## 📄 License
MIT License. Feel free to use, modify, and distribute.
