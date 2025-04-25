## Exercise number 3: Actually start using GIT/GitHub

So, this time the exercise is a bit more open-ended:  
Start applying Git/GitHub in your daily workflow,  
gather experiences, possibly problems, hopefully successes.

---

### Tasks

1. **Pick a set of codes** you are working on.  
Create a Git repository from it. (Basically repeat Exercise 2 on it.)

2. **Use Git regularly** while coding.  
The regular workflow should be, after each coding session (or after completing something):

```bash
git add .
git commit -m "what you changed"
git push
```

And if someone else might have worked on your code (or you did, on a different computer), always run:

```bash
git pull
```

Before you start coding — so you get possible new changes first.

3. **Share it** with colleagues who might benefit from the code.  
(Or not, if it's classified or there's another reason not to.)

---

### Handy Commands

| Command                         | Description                           |
|----------------------------------|---------------------------------------|
| `git status`                    | See what’s changed                    |
| `git pull`                      | Fetch and merge changes from remote  |
| `git add .`                     | Stage all changes                     |
| `git commit -m "message"`       | Save a snapshot of your work          |
| `git push`                      | Send your work to GitHub              |

---

### View Changes / Earlier Versions

- Compare changes before committing:
  ```bash
  git diff
  ```
- See commit history:
  ```bash
  git log
  ```
- Check out an earlier commit (safe way):
  ```bash
  git clone git@github.com:yourname/yourrepo.git temp_folder
  cd temp_folder
  git checkout <commit-id>
  ```

- If you want to view just a single file from an earlier commit:
  ```bash
  git show <commit-hash>:<filename>
  ```

- And to save it for comparison or copying parts:
  ```bash
  git show <commit-hash>:<filename> > target_file
  ```

This way, you get a copy of the old file for yourself.  
Not often needed, but sometimes useful when you want to test reverting a change or recover a piece you lost.

---

### (Optional) Use a Branch

```bash
git checkout -b my_new_feature
```

Continue working and pushing like normal. This keeps your original `main` untouched, so you can safely experiment.

When you're done with the branch and happy with it, you can merge it back into main:

```bash
git checkout main
git merge my_new_feature
```

---

### Also explore GitHub itself

It has helpful views to show commit history, file comparisons, differences between branches, etc.  
Play around with it!

---

###  Questions, ideas, problems?

Use the **Issues tab** on the shared practice repository to:

- Ask Git-related questions
- Report problems you ran into
- Suggest improvements to these exercises

👉 https://github.com/siirias/GitDemonstrationQuacamole/issues  
(or use the `.fmi.fi` version inside the internal network)

> When you feel you’ve successfully used Git in your project, create an Issue there and share your experience!

**Good luck, and happy GITting to everyone.**
