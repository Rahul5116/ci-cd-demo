# Deploying to GitHub Pages with `gh-pages` Branch

This guide explains how to set up **GitHub Pages** for your repository using a dedicated `gh-pages` branch.

---

## 📌 Step 1: Create the `gh-pages` Branch

Open **Git Bash** and run the following commands in your repository:

```sh
git checkout --orphan gh-pages
git rm -rf .
```

- `git checkout --orphan gh-pages` → Creates a new branch without any history.
- `git rm -rf .` → Removes all tracked files to start fresh.

---

## 📌 Step 2: Add an `index.html` File

GitHub Pages requires an `index.html` file. Create one using:

```sh
echo "<h1>Hello, GitHub Pages!</h1>" > index.html
```

Then, add and commit the file:

```sh
git add index.html
git commit -m "Initial GitHub Pages setup"
```

---

## 📌 Step 3: Push the `gh-pages` Branch

Push the newly created branch to GitHub:

```sh
git push origin gh-pages
```

This makes the `gh-pages` branch available in your GitHub repository.

---

## 📌 Step 4: Enable GitHub Pages

1. **Go to your GitHub repository**  
2. Click on **Settings** → **Pages**  
3. Under **"Source"**, select `gh-pages` as the branch  
4. Click **Save**

After a few minutes, your site will be available at:

```
https://<your-username>.github.io/<repo-name>/
```

---

## 🎉 Done!

Now, whenever you update your `gh-pages` branch, your website will be automatically updated.
