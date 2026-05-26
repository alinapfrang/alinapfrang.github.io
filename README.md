# Alina Pfrang — Personal Website

A simple, clean personal academic website built in HTML and CSS.

## Folder structure

```
alina-pfrang-website/
├── index.html          ← homepage
├── research.html       ← publications and working papers
├── teaching.html       ← courses and supervision
├── style.css           ← shared styling for all pages
├── assets/
│   ├── photo.jpg       ← headshot
│   └── CV_AlinaPfrang.pdf
└── README.md           ← this file
```

## Previewing locally

Just double-click `index.html` and it will open in your web browser. That's it — you can edit the HTML files in any text editor (TextEdit, VS Code, Sublime, etc.) and refresh the browser to see changes.

## Editing tips

**To update text:** Open the relevant `.html` file in a text editor and edit the words between the HTML tags. The structure looks like:

```html
<p class="about-text">
  Your bio text goes here.
</p>
```

**To add a new paper to the Research page:** Copy one of the existing `<div class="paper">...</div>` blocks and edit the title, authors, and status.

**To change colors or fonts:** Edit `style.css`. The main color values are at the top under `:root`.

---

## Publishing online with GitHub Pages

This is the easiest free way to put your site online with a permanent URL.

### Step 1 — Create a GitHub account
Go to https://github.com and sign up (free).

### Step 2 — Create a new repository
1. Click the **+** icon (top right) → **New repository**
2. Name it **`yourusername.github.io`** (replace `yourusername` with your actual GitHub username — this exact name is what makes GitHub serve it as a website)
3. Set it to **Public**
4. Click **Create repository**

### Step 3 — Upload your files
On the new empty repository page:
1. Click **"uploading an existing file"**
2. Drag and drop all the files and the `assets` folder from this website folder
3. Scroll down and click **Commit changes**

### Step 4 — Visit your site
Wait 1–2 minutes, then go to:
`https://yourusername.github.io`

Your site is live! 🎉

### Step 5 (optional) — Use a custom domain like `alinapfrang.com`
1. Buy a domain from a registrar like Namecheap (~$12/year) or Cloudflare Registrar (cheapest, no markup)
2. In your GitHub repo, go to **Settings → Pages**
3. Under "Custom domain", enter your domain and save
4. In your domain registrar's DNS settings, add a CNAME record pointing to `yourusername.github.io`
5. Wait a few hours for DNS to propagate

GitHub has good docs on this: https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site

---

## Alternative: Netlify drag-and-drop (even easier, no account customization)

1. Go to https://app.netlify.com/drop
2. Drag the entire `alina-pfrang-website` folder onto the page
3. Your site is live at a random URL like `random-words-1234.netlify.app`
4. You can sign up for free to claim a nicer subdomain or connect a custom domain

---

## Things to keep updated

- **CV** — replace `assets/CV_AlinaPfrang.pdf` when you have a new version (keep the filename the same so links don't break)
- **Photo** — replace `assets/photo.jpg` if needed (keep filename the same)
- **Research page** — add new papers as they come out
- **Footer year** — currently shows 2026; update annually

---

## Questions while editing?

The HTML is intentionally simple and well-commented. If you want to add a new page (e.g. a "Policy" page, or a "CV" page that shows the CV inline rather than linking to the PDF), just copy `teaching.html`, rename it, and edit the content — then add a link to it in the `<nav>` section of every page.
