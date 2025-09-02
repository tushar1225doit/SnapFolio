### Step 1: Create a New Git Repository

1. **Open your terminal (Command Prompt, PowerShell, or Git Bash)**.
2. **Navigate to the directory** where your `index.html` file is located. For example:
   ```bash
   cd "C:\Users\Kshipra\Downloads\SnapFolio\SnapFolio"
   ```

3. **Initialize a new Git repository**:
   ```bash
   git init
   ```

4. **Add your HTML file to the repository**:
   ```bash
   git add index.html
   ```

5. **Commit your changes**:
   ```bash
   git commit -m "Initial commit with index.html"
   ```

### Step 2: Create a Remote Repository on GitHub

1. **Go to [GitHub](https://github.com)** and log in to your account.
2. **Click on the "+" icon** in the top right corner and select "New repository".
3. **Fill in the repository details**:
   - Repository name (e.g., `SnapFolio`)
   - Description (optional)
   - Choose "Public" or "Private"
   - Do not initialize with a README (since you already have files to push)
4. **Click on "Create repository"**.

### Step 3: Link Your Local Repository to GitHub

1. **Copy the repository URL** (HTTPS or SSH).
2. **In your terminal**, link your local repository to the remote one:
   ```bash
   git remote add origin <repository-url>
   ```
   Replace `<repository-url>` with the URL you copied from GitHub.

3. **Push your changes to GitHub**:
   ```bash
   git push -u origin master
   ```

### Step 4: Create a Static Web App

You can use various platforms to host your static web app. Here, I'll show you how to do it using GitHub Pages:

#### Using GitHub Pages

1. **Go to your GitHub repository**.
2. **Click on the "Settings" tab**.
3. **Scroll down to the "Pages" section**.
4. **Under "Source," select the branch you want to use (usually `master` or `main`)** and click "Save".
5. **After a few moments**, GitHub will provide you with a link to your live site.

### Step 5: Access Your Static Web App

- After setting up GitHub Pages, you can access your static web app at the URL provided in the "Pages" section of your repository settings. It will typically be in the format:
  ```
  https://<username>.github.io/<repository-name>/
  ```

### Additional Notes

- Make sure your `index.html` file is in the root of your repository for GitHub Pages to serve it correctly.
- If you have additional assets (like CSS, JS, or images), make sure to add them to your repository as well.

That's it! You have successfully created a Git repository, pushed your HTML code, and deployed it as a static web app.