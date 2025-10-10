# Codex File Store

This repository contains step-by-step instructions for creating a GitHub project that you can use to store configuration files (for example JSON, YAML, or plain text). Once the repository is online, you will be able to access the files from anywhere with an internet connection.

## 1. Prepare your environment

1. [Create a GitHub account](https://github.com/join) if you do not already have one.
2. [Install Git](https://git-scm.com/downloads) on the computer that will upload the files.
3. Configure your Git identity the first time you use Git on a machine:

   ```bash
   git config --global user.name "Your Name"
   git config --global user.email "you@example.com"
   ```

## 2. Create the GitHub repository

1. Sign in to GitHub and click the **New** repository button.
2. Give the project a descriptive name such as `config-file-store` and an optional description.
3. Choose whether the repository should be **Public** (anyone can read it) or **Private** (only invited collaborators can see it).
4. Decide whether to initialize the repository with a README; you can leave the other checkboxes (like adding a `.gitignore`) unchecked for now.
5. Click **Create repository**.

## 3. Clone the repository locally

Back on your computer run:

```bash
git clone https://github.com/<your-username>/<repo-name>.git
cd <repo-name>
```

Replace `<your-username>` and `<repo-name>` with the values you used when creating the repository.

## 4. Add configuration files

1. Create or copy the JSON/TXT files you want to store into the cloned repository directory.
2. If you want to organize the files into folders (for example, by application), create directories as needed.

## 5. Commit and push the files

```bash
git add .
git commit -m "Add initial configuration files"
git push origin main
```

If your repository uses a different default branch name, replace `main` with that branch name.

## 6. Access the files online

1. Visit `https://github.com/<your-username>/<repo-name>` to see the files in the GitHub web interface.
2. Click any file to view, download, or copy its raw contents. You can also use GitHub's **Download ZIP** button to grab the whole repository.

## 7. Keep the repository up to date

Whenever you change or add configuration files:

```bash
git add <file>
git commit -m "Describe the change"
git push
```

You can repeat these steps from any machine. If you are working on another computer, remember to clone the repository first or pull the latest changes with `git pull` before editing files.
