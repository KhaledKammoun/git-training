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
<code>git merge feature/your-feature-name</code>

### 11. Delete the Feature Branch Locally

After merging, you can safely delete the local feature branch:  
<code>git branch -d feature/your-feature-name</code>

### 12. Delete the Remote Branch

If you pushed your feature branch to the remote repository and want to delete it:  
<code>git push origin --delete feature/your-feature-name</code>

### 13. Cherry-Pick a Commit

To apply a specific commit from one branch to another, use:  
<code>git cherry-pick &lt;commit_hash&gt;</code>

### 14. Rebase Your Branch

To keep your feature branch updated with the main branch, use rebase:  
<code>git rebase main</code>

## <span style="color: #33C1FF;">⚠️ Important Notes</span>

- Always ensure you are on the correct branch before making changes.
- Regularly pull changes from the main branch to avoid conflicts.
- Use descriptive commit messages to maintain a clear project history.

## <span style="color: #33C1FF;">🎉 Happy Coding!</span>

Remember, practice makes perfect. Don’t hesitate to experiment in this repository and deepen your understanding of Git and GitHub! If you have any questions, feel free to ask. 🤗
