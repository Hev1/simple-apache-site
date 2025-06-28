# How to Use This Project with GitHub

## Step 1: Create a GitHub Repository
1. Go to [https://github.com](https://github.com) and log in.
2. Click the ➕ icon in the top right and choose **New repository**.
3. Name your repository (e.g., `simple-apache-site`).
4. ✅ Tick **Add a README file**
5. ❌ Do **not** add a `.gitignore` or license.
6. Click **Create repository**.

## Step 2: Push Local Files to GitHub

**IMPORTANT**: Make sure you've created the repository on GitHub first (Step 1)!

1. **Open Terminal in VS Code**:
   - In VS Code, go to `Terminal` → `New Terminal`
   - Make sure you're in the project folder: `/Users/heatherwilliams/Downloads/simple-apache-site 4`
   - You can verify by running: `pwd` (should show the full path above)
   
2. **Initialize Git and add files**:
   
   **Step 2a - Initialize Git repository:**
   ```bash
   git init
   ```
   This creates a new Git repository in your current folder.

   **Step 2b - Add all files to staging:**
   ```bash
   git add .
   ```
   The `.` means "add all files in this directory and subdirectories"

   **Step 2c - Check what files will be committed (optional):**
   ```bash
   git status
   ```
   You should see all your files listed in green (ready to commit)

   **Step 2d - Commit the files:**
   ```bash
   git commit -m "Initial commit with GitHub Actions workflows"
   ```
   This saves a snapshot of your files with a descriptive message.

3. **Connect to your GitHub repository**:
   ```bash
   git remote add origin https://github.com/hev1/simple-apache-site.git
   git branch -M main
   ```

4. **Push to GitHub**:
   ```bash
   git push -u origin main
   ```

   **Note**: You may be prompted to enter your GitHub credentials or use a personal access token.

## Step 3: Verify GitHub Actions
After pushing, your GitHub Actions workflows will automatically start running:

1. Go to your repository: `https://github.com/hev1/simple-apache-site`
2. Click the **Actions** tab
3. You should see the workflows running:
   - `Development Workflow` (runs on all pushes)
   - `Deploy Apache Site` (runs on main branch)
   - `Advanced Apache CI/CD` (runs on main branch)

## What's Already Included
✅ **GitHub Actions workflows are already created**:
- `.github/workflows/apache-deploy.yml` - Basic deployment
- `.github/workflows/advanced-deploy.yml` - Production CI/CD
- `.github/workflows/dev-workflow.yml` - Development QA

✅ **Project files**:
- `public-html/index.html` - Main page
- `public-html/about.html` - About page
- Updated `README.md` with workflow documentation
