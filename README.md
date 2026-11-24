# Umesh Patil — professional portfolio

React 19, Vite 6, Tailwind CSS 4 and Lucide React. Static site; no backend or paid services required.

## Local development
Install Node.js 22 LTS and Git. Extract this archive and open the umesh-portfolio directory in VS Code. In its terminal:

```sh
npm install
npm run dev
```
Open the localhost URL printed by Vite. To test the production build:

```sh
npm run build
npm run preview
```

## Free GitHub Pages deployment
1. Review all content before making it public. The original resume PDF contains a phone number and email; replace `public/resume.pdf` with a public-safe version if desired. Both supplied portraits are included; check that you have permission to publish them, especially the workplace branding. The main portrait is the studio photo, with the workplace-themed image in About.
2. Sign in as `patilumesh-code` and create a **public** repository named `patilumesh-code.github.io`. If it already exists, do not overwrite it blindly; integrate these files into the existing repository or choose a different repository name.
3. For a new empty repository, run the following from this project directory after `npm install` (commit the generated package-lock.json):

```sh
git init
git add .
git commit -m "Build professional analytics portfolio"
git branch -M main
git remote add origin https://github.com/patilumesh-code/patilumesh-code.github.io.git
git push -u origin main
```
4. Open the repository Settings > Pages. Under Build and deployment, choose GitHub Actions as Source.
5. Open Actions > Deploy portfolio to GitHub Pages > Run workflow > main > Run workflow. The included workflow installs packages, builds the site and publishes dist. Subsequent pushes to main trigger deployment automatically.
6. When the deployment succeeds, open https://patilumesh-code.github.io/. If you used a different repository name, the URL will include that repository name as a path.

## Customize
- `src/data.js`: social links, experience, skills, projects and credentials.
- `src/main.jsx`: layout, education, interactive chart examples and contact links.
- `src/style.css`: theme colors, layout and responsive rules.
- `public/`: resume, optimized photos and favicon.
- `index.html`: title, description and social metadata.
- `.github/workflows/deploy.yml`: deployment automation.

Project charts are illustrative synthetic data, not actual company records or model evaluation outputs. No project repository links, certificate images or verified numerical business outcomes were supplied; add only genuine evidence. The PL-300 entry follows the resume's CloudThat wording and does not independently establish a Microsoft certification. Contact uses mailto and requires the visitor's email app. Theme preference is stored locally. No tracking or backend is included.

## Validation status
Source syntax checked with the local TypeScript transpiler. The npm registry was unreachable in the authoring environment; dependencies could not be installed and the production build/browser behavior has not been verified. Run the build locally or use GitHub Actions before publishing.
