# Xiaobin Wu — Personal Academic Website

Personal academic homepage for **Xiaobin Wu (吴晓斌)**, Research Supervisor at the Pediatric Research Institute, Guangzhou Women and Children's Medical Center.

## Tech Stack

- Pure HTML5 + CSS3 + Vanilla JavaScript
- No build tools, no dependencies
- Deployable on **GitHub Pages** directly

## Directory Structure

```
个人网站/
├── index.html          # Main page
├── css/
│   └── style.css       # Stylesheet
├── js/
│   └── main.js         # Interactions & animations
├── images/             # Images (add your photo here)
└── README.md           # This file
```

## How to Deploy on GitHub Pages

### Step 1: Create a GitHub repository

1. Go to [github.com](https://github.com) and sign in
2. Click **New repository**
3. Name it `<your-username>.github.io` (e.g., `wuxiaobin.github.io`) — this makes it your root domain
   - OR name it anything (e.g., `academic-site`) — it will be at `<your-username>.github.io/academic-site`
4. Set to **Public**
5. Do NOT initialize with README (we already have one)

### Step 2: Push the website to GitHub

```bash
cd D:\Agents\个人网站

git init
git add .
git commit -m "Initial commit: personal academic website"

git remote add origin https://github.com/<your-username>/<repo-name>.git
git branch -M main
git push -u origin main
```

### Step 3: Enable GitHub Pages

1. Go to your repository on GitHub → **Settings** → **Pages**
2. Under "Branch", select `main` (or `master`) and `/ (root)`
3. Click **Save**
4. Wait 1-2 minutes. Your site will be live at:
   - `https://<your-username>.github.io` (if repo is `<username>.github.io`)
   - `https://<your-username>.github.io/<repo-name>` (otherwise)

### Step 4: Add a custom domain (optional)

1. In Settings → Pages, enter your custom domain (e.g., `wuxiaobin.com`)
2. Add a CNAME record at your DNS provider pointing to `<your-username>.github.io`
3. Check "Enforce HTTPS"

## How to Update

Edit the files locally, then:

```bash
git add .
git commit -m "Update: <describe changes>"
git push
```

Changes go live automatically within 1-2 minutes.

## Customization

- **Profile photo**: Add your photo as `images/photo.jpg` and uncomment the `<img>` tag in `index.html`
- **Colors**: Edit CSS variables in `css/style.css` (look for `:root` at the top)
- **Content**: Edit `index.html` - all text is in English with Chinese summaries
- **Add new publications**: Copy a `.pub-item` block in `index.html`

## License

Feel free to use this template for your own academic website. MIT License.
