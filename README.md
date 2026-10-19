# Cat Breed Search

A web application for browsing cat breeds using The Cat API. Select a breed to see its photo, description, and temperament.

## Features

- Fetches the list of cat breeds from The Cat API
- Breed selection via a searchable dropdown (SlimSelect)
- Displays breed image, description, and temperament
- Loading indicator while fetching data
- Error notifications on failed requests (iziToast)

## Technology

- Vanilla JavaScript (ES modules) with HTML partial injection
- Vite build tooling
- SlimSelect for the breed dropdown
- iziToast for notifications
- The Cat API
- GitHub Actions workflow deploying the production build to GitHub Pages

## Project structure

```
src/
  css/        Stylesheets
  js/
    cat-api.js   The Cat API request functions
    main.js      Breed dropdown, cat info rendering, loading/error states
  index.html
```

## Commands

```
npm install   # install dependencies
npm run dev   # start the Vite dev server
npm run build # build for production (GitHub Pages base path)
npm run preview # preview the production build
```

## Deployment

Pushes to `main` trigger a GitHub Actions workflow that builds the project and deploys the `dist` output to the `gh-pages` branch for GitHub Pages.
