Here’s a full list of Git commands you'll typically use to **pull from a remote repository, make changes, and push back to Git**:

---

### 1. Clone the repository (only needed the first time)

```bash
git clone <repository-url>
```

Example:

```bash
git clone https://github.com/username/repo.git
```

---

### 2. Pull the latest changes

```bash
git pull origin <branch-name>
```

Example:

```bash
git pull origin main
```

---

### 3. Check the current branch (optional)

```bash
git branch
```

---

### 4. Make changes to files

Edit or create files in your editor.

---

### 5. Add the changes

```bash
git add .
```

Or add specific files:

```bash
git add file1.txt file2.js
```

---

### 6. Commit the changes

```bash
git commit -m "Your commit message"
```

---

### 7. Push the changes to the remote repository

```bash
git push origin <branch-name>
```

Example:

```bash
git push origin main
```

---

### Optional: Helpful Extras

#### Check status of changes

```bash
git status
```

#### View commit history

```bash
git log --oneline
```

#### Create and switch to a new branch

```bash
git checkout -b new-branch-name
```
