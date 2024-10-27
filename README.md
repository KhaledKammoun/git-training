# 🚀 Git Training

Welcome to the <strong><span style="color: #FF5733;">Git Training</span></strong> repository! 🎉 This space is designed for you to learn and practice Git and GitHub commands without affecting any main projects. Let's dive into the world of version control together! 🌟

## <span style="color: #33C1FF;">📚 Purpose</span>

In this repository, you will:

- Learn basic Git commands: <code>add</code>, <code>commit</code>, <code>push</code>, <code>pull</code>, <code>clone</code>, and more. 💻
- Practice branching, merging, and resolving conflicts. 🔀
- Get familiar with pull requests and collaborating with others. 🤝
- Explore advanced commands: <code>rebase</code>, <code>stash</code>, <code>cherry-pick</code>, and more. 🔍

## <span style="color: #33C1FF;">🛠️ Getting Started</span>

### 1. Clone the Repository

Start by cloning the repository to your local machine:  
<code>git clone https://github.com/your-username/git-training.git</code>

### 2. Navigate to the Repository

Move into your newly cloned repository:  
<code>cd git-training</code>

### 3. Create a New Branch for Your Changes

To avoid conflicts, it's recommended to create a new branch for each feature or bug fix:  
<code>git checkout -b feature/your-feature-name</code>

### 4. Make Your Changes and Commit Them

Once you've made your changes, add them to the staging area and commit:  
<code>git add .</code>  
<code>git commit -m "Your commit message"</code>

> <strong>Note:</strong> You can also use the command below to add and commit changes in one step, but remember, this only works for files that have already been tracked by Git (i.e., files previously added to the repository):  
> <code>git commit -am "Your commit message"</code>

### 5. Working with Stash

If you need to save your changes temporarily, use stash:  
<code>git stash</code>  
To apply your stashed changes later:  
<code>git stash apply</code>

### 6. Reset a Previous Commit (if needed)

If you want to reset your branch to a previous commit, you can use:  
<code>git reset --soft HEAD~1</code>

- <strong>--soft</strong>: Keeps the changes in the staging area.
- <strong>--hard</strong>: Discards all changes in the working directory and staging area, permanently losing any changes made since that commit.  
  Alternatively, reset using a specific commit hash:  
  <code>git reset --soft &lt;commit_hash&gt;</code>

### 7. Push Your Changes to the Remote Repository

Once you're satisfied with your changes, push them to the remote repository:  
<code>git push origin feature/your-feature-name</code>

### 8. Checkout to the Main Branch

Switch back to the main branch:  
<code>git checkout main</code>

### 9. Create a Pull Request

Before creating a pull request, ensure your local branch is up to date. If there have been changes in the remote main branch, update your local copy:  
<code>git pull origin main</code>  
OR  
<code>git fetch origin main</code>  
<code>git merge origin/main</code>

### 10. Merge the Feature Branch with Main

To merge your feature branch into the main branch:

```bash
git merge feature/your-feature-name
```

To push the merged changes to the remote main branch:

```bash
git push origin main
```

### 11. Delete the Feature Branch Locally

After merging, you can safely delete the local feature branch:  
<code>git branch -d feature/your-feature-name</code>

# Git and GitHub Workflow

### 11. Delete the Remote Branch

If you’ve pushed your feature branch to the remote repository and want to delete it, use:

```bash
git push origin --delete feature/your-feature-name
```

### 11.1 Restore a Deleted Branch

In case you want to restore a deleted branch, you can find the commit it pointed to using the following command (this lists all actions, including commits, from the latest to the oldest):

```bash
git reflog
```

#### Steps to Restore the Branch

1. **Find the Target Commit SHA**  
   Use `git reflog` to locate the commit SHA you need (e.g., `ea9d340`).

2. **Recreate the Branch Locally**  
   Replace `your-feature-name` with the name of the branch you want to restore:

   ```bash
   git checkout -b feature/your-feature-name ea9d340
   ```

3. **Push the Branch Back to GitHub (Optional)**  
   Push the restored branch back to the remote repository:

   ```bash
   git push origin feature/your-feature-name
   ```

### 12. Update Branches List in Your Local Repository

To update your local repository with the latest branches from the remote:

```bash
git fetch origin               # Fetch the latest branches from remote
git branch -r                  # List remote branches to verify
git checkout --track origin/your-branch-name   # Create a local copy of the remote branch
git branch                     # List local branches
```

### 13. Synchronize Branches

To keep your branch synchronized with another branch, use:

```bash
git pull origin branch-name
```

---

Happy coding! 🎊 Remember, practice makes perfect. Don’t hesitate to experiment in this repository and deepen your understanding of Git and GitHub! If you have any questions, feel free to ask. 🤗
