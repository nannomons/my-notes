---
tags:
  - ChatGPT
---
Yes — **it's 100% free** if you go the route of **GitHub Pages + a digital garden setup like Quartz**. No need to pay for Obsidian Publish or hosting fees.

---

## ✅ What You'll Be Setting Up

You'll turn your Obsidian vault (or a subset of notes) into a **public website** using:

- **[[Quartz]]** – a free static site template built for Obsidian-like notes
    
- **[[GitHub]]** – to host your website for free via **GitHub Pages**
    

This combo gives you something that _looks and feels like Obsidian Publish_, without the cost.

---

## 🧠 What You Need

### Prereqs:

- A GitHub account (free)
    
- A basic terminal (Mac/Linux: Terminal; Windows: Git Bash or WSL)
    
- Obsidian installed
    
- Some Markdown notes you'd like to publish
    

---

## 🚀 Step-by-Step Guide to Set Up Quartz for Your Obsidian Vault

### 🔹 Step 1: Create a GitHub Repo

1. Go to [github.com](https://github.com) → Sign in or sign up.
    
2. Create a **new public repository** (e.g., `my-digital-garden`).
    
    - Don’t initialize with a README or license yet.
        

---

### 🔹 Step 2: Clone Quartz Template

You’ll use Quartz as your base. You have two options:

#### Option A: Use GitHub’s “Use This Template” Feature

1. Visit the [Quartz GitHub Repo](https://github.com/jackyzha0/quartz)
    
2. Click the green **“Use this template”** → **Create a new repository**
    

OR

#### Option B: Clone it via terminal

```bash
git clone https://github.com/jackyzha0/quartz.git my-digital-garden
cd my-digital-garden
```

---

### 🔹 Step 3: Replace Sample Content with Your Notes

1. Inside the `content` folder of the cloned Quartz repo, delete the sample notes.
    
2. Copy your selected Obsidian notes into the `content` folder.
    
    - Stick to `.md` files.
        
    - You can keep Obsidian-style `[[wikilinks]]`—Quartz supports them!
        

---

### 🔹 Step 4: Preview Locally (optional but useful)

If you want to preview your site before uploading:

1. Make sure you have [Node.js installed](https://nodejs.org/en/download/).
    
2. Run:
    
    ```bash
    npm install
    npm run dev
    ```
    
    This starts a local server at `http://localhost:3000`.
    

---

### 🔹 Step 5: Push to GitHub

```bash
# If you used git clone:
git remote set-url origin https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git

# Then push everything
git add .
git commit -m "Initial commit"
git push -u origin main
```

---

### 🔹 Step 6: Enable GitHub Pages

1. Go to your repo on GitHub
    
2. Settings → “Pages” tab on the left
    
3. Under **“Source”**, choose `Deploy from a branch`, then select the `gh-pages` branch (or `/docs` folder if that's the setup).
    
4. Save and wait a few minutes. Your site will be available at:
    

```
https://yourusername.github.io/your-repo-name
```

---

## 🌱 Optional: Customize Your Digital Garden

- Edit `quartz.config.ts` to change your site title, author, theme, etc.
    
- Add a `README.md` for project context
    
- Add frontmatter (`---` at the top of your notes) to tag or hide files from the site
    

---

## ✅ Summary of What You Get

| Feature              | Obsidian Publish | Quartz + GitHub |
| -------------------- | ---------------- | --------------- |
| Share via URL        | ✅                | ✅               |
| Cost                 | 💸 ~$8/mo        | 🟢 Free         |
| Obsidian-style links | ✅                | ✅               |
| Custom domain        | ✅                | ✅ (optional)    |
| Looks clean/modern   | ✅                | ✅               |

---

Would you like me to help you set up a sample repo based on your vault structure? Or walk you through Git/GitHub if that’s still new to you?