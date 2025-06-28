# How to Use This Project with GitHub

## Step 1: Create a GitHub Repository
1. Go to [https://github.com](https://github.com) and log in.
2. Click the ➕ icon in the top right and choose **New repository**.
3. Name your repository (e.g., `simple-apache-site`).
4. ✅ Tick **Add a README file**
5. ❌ Do **not** add a `.gitignore` or license.
6. Click **Create repository**.

## Step 2: Push Local Files to GitHub
1. Unzip this project on your computer.
2. Open a terminal inside the unzipped folder.
3. Run the following commands:

```bash
git init
git remote add origin https://github.com/YOUR-USERNAME/simple-apache-site.git
git add .
git commit -m "Initial commit"
git branch -M main
git push -u origin main
```

Replace `YOUR-USERNAME` with your GitHub username.

## Step 3: Follow the Lesson
Now your files are on GitHub, follow the lesson instructions to:
- Create `.github/workflows/apache-deploy.yml`
- Use GitHub Copilot and Copilot Chat in VS Code to scaffold and improve the workflow.
