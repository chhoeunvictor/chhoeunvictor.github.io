# Victor Chhoeun — Portfolio

Personal portfolio for Victor Chhoeun, Technical Writer & Content Strategist.

## 🚀 Deploying to GitHub Pages

### Step 1 — Create a GitHub repository

1. Go to [github.com](https://github.com) and sign in
2. Click the **+** button → **New repository**
3. Name it exactly: `your-username.github.io`  
   *(Replace `your-username` with your actual GitHub username — this is required for GitHub Pages to work)*
4. Set it to **Public**
5. Click **Create repository**

---

### Step 2 — Upload your files

**Option A — Using GitHub's website (easiest):**

1. Open your new repository
2. Click **Add file → Upload files**
3. Drag and drop all 4 files:
   - `index.html`
   - `style.css`
   - `script.js`
   - `README.md`
4. Scroll down, write a commit message like `Initial portfolio`, click **Commit changes**

**Option B — Using Git (if you have it installed):**

```bash
git init
git add .
git commit -m "Initial portfolio"
git branch -M main
git remote add origin https://github.com/your-username/your-username.github.io.git
git push -u origin main
```

---

### Step 3 — Enable GitHub Pages

1. Go to your repository → **Settings** tab
2. Click **Pages** in the left sidebar
3. Under **Source**, select **Deploy from a branch**
4. Choose **main** branch, **/ (root)** folder
5. Click **Save**

Your site will be live at:
```
https://your-username.github.io
```

> It usually takes 1–3 minutes to go live after the first deploy. Subsequent updates are faster.

---

## ✏️ Customizing your content

### Update your work projects
Open `index.html` and find the `<!-- WORK PORTFOLIO -->` section. Each `<article class="work-card">` is one project. Edit the title, description, tag, year, and link.

### Update your writing samples
Find the `<!-- WRITING SAMPLES -->` section. Each `<a class="writing-item">` is one piece. Update the `href` with your actual URLs.

### Change contact info
Find `<!-- CONTACT -->` and update the email, LinkedIn URL, and phone number.

### Add your photo (optional)
You can add a profile photo in the About section. Add this to `index.html` inside `.about-left`:
```html
<img src="your-photo.jpg" alt="Victor Chhoeun" class="about-photo" />
```
Then add to `style.css`:
```css
.about-photo {
  width: 100%;
  max-width: 320px;
  border-radius: 8px;
  filter: grayscale(20%);
  margin-top: 2rem;
}
```

---

## 📁 File structure

```
your-username.github.io/
├── index.html     ← All page content and structure
├── style.css      ← All styles and responsive design
├── script.js      ← Scroll animations and nav behavior
└── README.md      ← This file
```

---

## 🎨 Colors & fonts

The portfolio uses:
- **DM Serif Display** — headings and display text
- **Syne** — body and navigation
- **DM Mono** — labels, tags, and code-style text

Colors are defined as CSS variables at the top of `style.css` — easy to change.
