## Aim:- Develop and deploy a portfolio Azure static Web App on a custom domain (tushargalhotra.shop) creating and using git repository, In this pursuit I downloaded a web template and customise it then commited to the repository and then using Azure static web app then configure a custom domain


### Step 1: Create a New Git Repository

1. **Open your terminal (Command Prompt, PowerShell, or Git Bash)**.
2. **Navigate to the directory** where your `index.html` file is located. For example:
   ```bash
   cd "C:\Users\Kshipra\Downloads\SnapFolio\SnapFolio"
   ```

3. **Initialize a new Git repository**:

   git init


4. **Add your HTML file to the repository**:
   
   git add index.html


5. **Commit your changes**:
   git commit -m "Initial commit with index.html"

### Step 2: Create a Remote Repository on GitHub

1. **Go to [GitHub](https://github.com)** and log in to your account.
2. **Click on the "+" icon** in the top right corner and select "New repository".
3. **Fill in the repository details**:
   - Repository name (`myportal`)
   - Description (optional)
   - Choose "Public"
   - Do not initialize with a README (since you already have files to push)
4. **Click on "Create repository"**.

### Step 3: Link Your Local Repository to GitHub

1. **Copy the repository URL** (HTTPS or SSH).
2. **In your terminal**, link your local repository to the remote one:

   git remote add origin <repository-url>


3. **Push your changes to GitHub**:
   git push -u origin master

### Step 4: Create a Static Web App

You can use various platforms to host your static web app. Here, I'll show you how to do it using GitHub Pages:



### Step 5: Access Your Static Web App

- After setting up GitHub Pages, you can access your static web app at the URL provided in the "Pages" section of your repository settings. It will typically be in the format:
  ```
  https://<username>.github.io/<repository-name>/
  ```

I have successfully created a Git repository, pushed your HTML code, and deployed it as a static web app