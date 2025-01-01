Here are the steps to create a repository named **"DevOps"** on GitHub:

### Option 1: Create via GitHub Website

1. **Go to GitHub:**
   - Open your browser and go to [GitHub](https://github.com/).

2. **Sign in:**
   - Log in to your GitHub account.

3. **Create a New Repository:**
   - Click the **"+"** icon in the top-right corner and select **"New repository"**.

4. **Fill in the Repository Details:**
   - **Repository Name:** Enter `DevOps`.
   - **Description (Optional):** You can add a description, such as "Repository for DevOps-related projects."
   - **Public or Private:** Choose whether the repository will be public or private.
   - **Initialize with a README:** You can check this option if you'd like to add a README file automatically.

5. **Create Repository:**
   - Click the **"Create repository"** button.

### Option 2: Create via Git CLI

1. **Set up your GitHub credentials locally (if not already set):**
   ```bash
   git config --global user.name "Your Name"
   git config --global user.email "youremail@example.com"
   ```

2. **Create a new directory for your repository:**
   ```bash
   mkdir DevOps
   cd DevOps
   ```

3. **Initialize the Git repository:**
   ```bash
   git init
   ```

4. **Add your files (optional):**
   ```bash
   echo "# DevOps" >> README.md
   git add README.md
   ```

5. **Commit the changes:**
   ```bash
   git commit -m "Initial commit"
   ```

6. **Create the repository on GitHub using the GitHub CLI:**
   ```bash
   gh repo create DevOps --public
   ```

   If you don’t have the GitHub CLI (`gh`), you can install it by following [these instructions](https://cli.github.com/manual/installation).

7. **Push your local repository to GitHub:**
   ```bash
   git branch -M main
   git remote add origin https://github.com/yourusername/DevOps.git
   git push -u origin main
   ```

Now your `DevOps` repository is created on GitHub and ready to use.
