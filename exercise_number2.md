## Exercise number 2 in getting to know GIT and GitHub (.com or .fmi.fi)

### Aims

1. **Create your very own repository.** Use some set of your own codes or other suitable files. 1b. *(Bonus)* Add `README.md` and `.gitignore` files to complete the repository.
2. **Share the repository** on GitHub (.com or .fmi.fi).
3. **Invite a collaborator** to the repository (a colleague working on the same code, a fellow doing these exercises, or me – `siirias` on both GitHubs).\
   3b. *(Bonus)* Make at least one commit in addition to the initial one, to build some history for your repository.
4. **Announce your repository.** Edit the list at the end of this file (as in Exercise 1) with your name and a link to your new repository.

Having accomplished all these, you should be ready to apply Git version control on your own codes and collaborate with others.

---

### Useful Commands and Notes

All commands are to be run in **Git Bash**, opened in the folder where your codebase is located.

```bash
git status  # Always a good command to see the current status of your repository
```

---

### Part 1: Local Setup

1. Locate or create the folder where your target codes are.

2. *(Bonus)* Add:

   - `.gitignore` to exclude unwanted files (e.g., `*.jpg`, `*.png`, temporary outputs)
   - `README.md` to describe the purpose and contents of the repository

```bash
git init  # Initialize a new Git repository locally
```

If this is your first Git repository on this computer, configure your identity:

```bash
git config --global user.name "Your Name"
git config --global user.email "your@email.com"
```

*To set a different identity per project, omit **``**.*

```bash
git add .
git commit -m "Initial commit"
git branch -M main  # Rename branch to 'main' (sometimes Git defaults to 'master')
```

---

### Part 2: Upload to GitHub

Most of this part is done on GitHub (.com or .fmi.fi). Make sure you have a GitHub account and SSH keys set up. Ask Simo or Henry for help if needed.

#### Create a New Repository

- Go to your GitHub account and find "Repositories"
- Click the green **NEW** button
- Choose repository **name**, **visibility** (public/private), and create it

GitHub will then show instructions for pushing an existing repo.

> **NOTE:** GitHub provides both HTTPS and SSH URLs:
>
> - **HTTPS** (`https://...`) is fine for downloading only
> - **SSH** (`git@github...`) is preferred for pushing changes (and requires SSH keys)

Make sure you’re using the SSH version:

```bash
git remote add origin git@github.com:yourname/yourrepo.git
git push -u origin main
```

Now your repository is live!

---

### Part 3: Collaboration

If your repo is **public**, others can view and clone it without needing access. For **collaborators** (edit access):

- Go to your repository settings (not your account settings)
- Find **"Collaborators"**
- Click **"Add People"** and enter their GitHub username (e.g., `siirias`)
- They must accept the invitation via GitHub or email

#### Bonus (3b): Make additional changes

```bash
git pull               # In case someone else or another machine made changes
git add .
git commit -m "Describe what you changed"
git push
```

---

### Part 4: Report Your Work

As in Exercise 1, navigate back to the shared repository and open Git Bash:

```bash
git pull  # Get the latest version
```

Edit the text file (likely this one), and add your name and repository link at the end. Then:

```bash
git add .
git commit -m "added name"
git push
```

Or if you're curious about GitHub’s web interface, try clicking the **"Edit"** button on this file in GitHub and make the commit directly from the browser.

---

### Newly Created Repositories

(Add your name and repository link here)

---

