# Nisarga Xavier — Portfolio Website

A personal portfolio website built with HTML, CSS, and JavaScript. Connected to Firebase Firestore for feedback submissions. Hosted on Render with manual CI/CD via GitHub Actions.

---

## 📁 File Structure

```
Nisarga Xavier/
├── index.html                  ← Main portfolio page
├── Nisarga.jpeg                  ← Your profile photo
├── AWS.png                     ← AWS certification image
├── CSS3.png                    ← CSS3 certification image
├── Digital Engineering.png     ← Digital Engineering cert image
├── README.md                   ← This file
└── .github/
    └── workflows/
        └── deploy.yml          ← GitHub Actions manual deploy workflow
```

---

## 🚀 How to Deploy

### 1. Push to GitHub
```bash
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/nithu-portfolio.git
git push -u origin main
```

### 2. Host on Render
- Go to [render.com](https://render.com) → New → Static Site
- Connect your GitHub repo
- Build Command: *(leave blank)*
- Publish Directory: `.`
- Click **Create Static Site**

### 3. Add Deploy Hook Secret to GitHub
- Render Dashboard → your site → Settings → Deploy Hook → Generate
- Copy the URL
- GitHub repo → Settings → Secrets → Actions → New secret
  - Name: `RENDER_DEPLOY_HOOK`
  - Value: paste the Render URL

### 4. Trigger a Deploy
- GitHub repo → **Actions** tab
- Click **Deploy to Render (Manual)**
- Click **Run workflow** button
- Done! 🎉

---

## 🛠 Tech Stack
- HTML5, CSS3, JavaScript
- Firebase Firestore (feedback form)
- Render (hosting)
- GitHub Actions (CI/CD)
