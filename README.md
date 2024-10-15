# 🚀 Git Training

Welcome to the **Git Training** repository! 🎉 This space is designed for you to learn and practice Git and GitHub commands. Let's dive into the world of version control together! 🌟

## 📚 Purpose

In this repository, you will:

- Learn basic Git commands: `add`, `commit`, `push`, `pull`, `clone`, and more. 💻
- Practice branching, merging, and resolving conflicts. 🔀
- Get familiar with pull requests and collaborating with others. 🤝

## 🛠️ Getting Started

### 1. **Clone the Repository:**

Start by cloning the repository to your local machine:

```bash
git clone https://github.com/KhaledKammoun/git-training.git
```

### 2. **Navigate to the Repository:**

Move into your newly cloned repository:

```bash
cd git-training
```

### 3. **Create a New Branch for Your Changes:**

To avoid conflicts, it's recommended to create a new branch for each feature or bug fix:

```bash
git checkout -b feature/your-feature-name
```

### 4. **Make Your Changes and Commit Them:**

Once you've made your changes, add them to the staging area and commit:

```bash
git add .
git commit -m "Your commit message"
```

🔔 **Note:** You can also use the command below to add and commit changes in one step, but remember, this only works for files that have already been tracked by Git (i.e., files previously added to the repository):

```bash
git commit -am "Your commit message"
```

### 5. **Reset a Previous Commit (if needed):**

If you want to reset your branch to a previous commit, you can use:

```bash
git reset --soft HEAD~1
```

🔍 **Note:**

- **`--soft`**: Keeps the changes in the staging area.
- **`--hard`**: Discards all changes in the working directory and staging area, permanently losing any changes made since that commit.

Alternatively, reset using a specific commit hash:

```bash
git reset --soft <commit_hash>
```

### 6. **Push Your Changes to the Remote Repository:**

Once you're satisfied with your changes, push them to the remote repository:

```bash
git push origin feature/your-feature-name
```

### 7. **Checkout to the Main Branch:**

Switch back to the main branch:

```bash
git checkout main
```

### 8. **Create a Pull Request:**

Before creating a pull request, ensure your local branch is up to date. If there have been changes in the remote main branch, update your local copy:

```bash
git pull origin main
```

OR

```bash
git fetch origin main
git merge origin/main
```

### 9. **Merge the Feature Branch with Main:**

To merge your feature branch into the main branch:

```bash
git merge feature/your-feature-name
```

### 10. **Delete the Feature Branch Locally:**

After merging, you can safely delete the local feature branch:

```bash
git branch -d feature/your-feature-name
```

### 11. **Delete the Remote Branch:**

If you pushed your feature branch to the remote repository and want to delete it, use:

```bash
git push origin --delete feature/your-feature-name
```

---

Happy coding! 🎊 Remember, practice makes perfect. Don’t hesitate to experiment in this repository and deepen your understanding of Git and GitHub! If you have any questions, feel free to ask. 🤗
