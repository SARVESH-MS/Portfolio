# Portfolio Website

This is a single-page personal portfolio website.

The project uses a small React setup for local development and build commands, but the visible portfolio content is currently managed as a static page in `public/index.html`.

## Tech Used

- HTML5, CSS3, and vanilla JavaScript for the portfolio page
- React 17 and React Scripts 5 for local development and production builds
- Manrope and DM Mono via Google Fonts

## Project Structure

Main files you will use:

- `public/index.html`  
  Main portfolio content: headings, skills, projects, contact section, links, and page structure.

- `public/assets/css/style.css`  
  Main styling for the portfolio.

- The mobile menu and scroll-scrub hero timeline are small inline scripts in `public/index.html`.

- `public/assets/sarvesh-profile-optimized.webp`: Compressed portrait used in the About card and as the reduced-motion hero fallback.
- `public/assets/sarvesh-rotation-fastseek.mp4` and `public/assets/sarvesh-rotation-poster.jpg`: Optimized scroll-scrubbed hero animation and its opening frame.

- `public/assets/resume/My Resume.pdf`  
  Resume file used by the download button.

- `src/index.js` and `src/App.js`  
  Minimal React entry used so the project can run with `react-scripts`.

## How To Run

Make sure Node.js and npm are installed.

### 1. Install dependencies

```bash
npm install
```

### 2. Start the development server

```bash
npm start
```

By default, the site opens at `http://localhost:3000`.

If port `3000` is already in use, React automatically starts on another port such as `3001`.

### 3. Build for production

```bash
npm run build
```

This creates a generated `build/` folder for deployment.

## GitHub Pages Deployment

This project is configured for GitHub Pages as a project site.

After deployment, the site opens at `https://sarvesh-ms.github.io/Portfolio/`.

Important setup already added in this repo:

- `package.json` has the correct `homepage`
- GitHub Actions workflow is added at `.github/workflows/deploy-pages.yml`

To finish enabling GitHub Pages on GitHub:

1. Open the repository on GitHub
2. Go to `Settings`
3. Open `Pages`
4. Under `Build and deployment`, choose `GitHub Actions`

After that, every push to `main` can deploy the site automatically.

## What To Edit

### Change portfolio content

Edit:

```text
public/index.html
```

Use this file for:

- name
- about text
- education
- skills
- projects
- contact links
- social links

### Change styling

Edit:

```text
public/assets/css/style.css
```

### Change JavaScript interactions

Edit the small inline script near the end of `public/index.html`.

### Change image or resume

- `public/assets/sarvesh-profile-optimized.webp`
- `public/assets/resume/My Resume.pdf`

## Important Notes

- This project now has **one real source page**: `public/index.html`
- Do **not** edit generated build output
- If `build/` appears after running `npm run build`, that is normal
- Always edit the source files in `public/`

## Portfolio Sections

The page currently contains these main sections:

- Home
- About
- Expertise
- Projects
- Education
- Contact

## Quick Workflow

1. Open `public/index.html`
2. Make your content changes
3. Save the file
4. Refresh the browser
5. Use `Ctrl + F5` if the browser shows an older cached version

## Current NPM Scripts

```bash
npm start
npm run build
npm test
```

## Maintenance Tip

If you ever see old tabs in the editor such as deleted `build/...` or backup files, close those tabs and continue working only in the current source files listed above.
