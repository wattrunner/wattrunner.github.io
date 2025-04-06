# Wattrunner Website

This is the repository for the Wattrunner static website, built with [Astro](https://astro.build/) and [Tailwind CSS](https://tailwindcss.com/). The site is hosted on GitHub Pages.

## Branches

*   `main`: Deployed branch for GitHub Pages.
*   `staging`: Development branch for building and testing new features before merging into `main`.

## Project Setup

1.  **Clone the repository:**
    ```bash
    git clone <repository-url>
    cd wattrunner.github.io
    ```

2.  **Install dependencies:**
    ```bash
    npm install
    ```

## Development

To start the local development server:

```bash
npm run dev
```

This will open the site in your browser, usually at `http://localhost:4321`. The server will automatically reload when you make changes to the code.

## Build

To build the static site for production:

```bash
npm run build
```

This command generates the static files in the `dist/` directory. These are the files that will be deployed to GitHub Pages.

## Deployment (GitHub Pages)

This repository is configured to deploy the contents of the `main` branch to GitHub Pages. Changes pushed or merged to `main` will trigger a GitHub Action (needs to be set up) to build the site and deploy the `dist/` folder.

**Workflow:**

1.  Make changes on the `staging` branch.
2.  Test locally using `npm run dev`.
3.  Commit and push changes to `staging`.
4.  Once ready, create a Pull Request from `staging` to `main`.
5.  After review and approval, merge the Pull Request.
6.  The GitHub Action (when configured) will automatically build and deploy the site from the `main` branch. 