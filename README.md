# Task Manager — CI/CD Practice

A beginner-friendly task manager built with HTML, CSS and JavaScript. Tasks are saved in your browser using `localStorage`.

## Run locally

Open `index.html` in your browser.

## Deploy with GitHub Actions

1. Create a new **public** repository on GitHub, for example `task-manager-cicd`.
2. Extract this ZIP file and upload the project files and folders to the repository root.
3. Make sure the default branch is named `main`.
4. Open **Settings → Pages** in your repository.
5. Under **Build and deployment → Source**, choose **GitHub Actions**.
6. Open the **Actions** tab. The workflow should start after you push to `main`.
7. Wait for both jobs, `validate` and `deploy`, to finish successfully.
8. Open **Settings → Pages** to find your published website URL.

## What the pipeline does

- **CI:** On pushes and pull requests to `main`, GitHub Actions checks that the app files exist and validates JavaScript syntax.
- **CD:** On pushes to `main` (and manual workflow runs), the workflow publishes the website to GitHub Pages after validation succeeds.

## Practice exercises

1. Change the page title in `index.html`, commit and push. Watch the Actions run.
2. Change a color in `style.css`, commit and push. Refresh the live website.
3. Open a branch, make a change and create a pull request. Observe that validation runs but deployment does not.
4. Introduce a JavaScript syntax error in a test branch. Observe the failed validation job, then fix it.
5. Merge a pull request into `main`. Observe the deployment run.

## Important

GitHub Pages publishes static websites. This project does not need a server or database. Task data is stored separately in each visitor's browser.
