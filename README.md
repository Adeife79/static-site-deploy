## Static Website Deployed via GitHub Pages
This project demonstrates how to deploy a static website to GitHub Pages using GitHub Actions. This project is to practice automation of deployments; every push to `main` triggers a workflow that builds and publishes the site with zero manual steps.

## Tech Stack
- HTML 5
- CSS 3
- GitHub Actions (CI/CD)
- GitHub Pages (app host)

## Project Structure

```
static-site-deploy
├──.github
|    └──  workflows
|        └── deploy.yanl
├── website
|    ├── index.html
|    └── styles.css
└── README.md
```


## Local Set Up
1. Create a project folder and navigate to it:
```bash
mkdir static-site
cd static-site
```

2. Create a new folder inside the project folder and create app files (html and css)
```bash
mkdir website
cd website
touch index.html
touch styles.css
```

3. Push to GitHub Repository.
```bash
git init
git add .
git commit -m "initial commit"
git remote add origin <github_repo_url>
git push -u origin main
```

## GitHub Pages Set Up
Here's a guide on how the GitHub pages were setup 
- Go to your repoitory **Settings**  → **Pages** 
- Under **Build and deployment**, set **Source** to `GitHub Actions`
- Push to `main` for the workflow to handle the deployment.

## Static Website Deployment
This project uses a GitHub Actions workflow (/github/workflows/deploy.yaml) to automatically deploy to GitHub Pages whenever changes are pushed to the main branch.

Below is a step on how to get github action workflow for a static website

1. Go to repository GitHub Actions, navigate to **Pages** → **Static HTML**
2. Click on **Configure** in Static HTML.
3. Modify yaml file (optional) and click on **Commit changes**
4. Go to workflows page, you static website url is displayed there if the workflow runs successfully.

## The Preview of the Website

![Website Screenshot](images/webpage.png)

## Contributions
Suggestions are always welcome!. You can fork the repository, or clone it.

