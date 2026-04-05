# WrestleFlixx Website

A clean, professional wrestling streaming site built for GitHub Pages.

## File Structure

```
wrestleflixx/
├── index.html              ← Homepage
├── events.html             ← Events library
├── promotions.html         ← Promotions page
├── about.html              ← About page
├── css/
│   ├── style.css           ← Main styles
│   └── reader.css          ← Episode reader styles
├── js/
│   └── main.js             ← Navigation + animations
├── episodes/
│   ├── episode-1.html      ← Sample episode 1
│   ├── episode-2.html      ← Sample episode 2
│   └── (add more here)
└── README.md
```

---

## How to Deploy on GitHub Pages (Free, No Banner)

1. Create a GitHub Organization named `WrestleFlixx`
2. Create a repo named exactly: `wrestleflixx.github.io`
3. Upload ALL files (keep folder structure intact)
4. Settings → Pages → Source: main branch → Save
5. Live at: `https://wrestleflixx.github.io`

---

## How to Add a New Episode

1. Copy `episodes/episode-1.html`, rename to `episodes/episode-3.html`
2. Edit the title, banner image, synopsis, and body content
3. Add your text using the elements below
4. Update the prev/next nav links at the bottom
5. Add a card for it in `events.html`
6. Upload both files to GitHub

### Content elements you can use inside episode-body:

**Heading:** `<h2>Section Title</h2>`

**Paragraph:** `<p>Your text here.</p>`

**Full-width image:**
```html
<figure class="episode-figure">
  <img src="IMAGE-URL" alt="Description" />
  <figcaption>Optional caption.</figcaption>
</figure>
```

**Right-floated image (text wraps):** add class `episode-figure-right`
**Left-floated image:** add class `episode-figure-left`

**Pull quote:**
```html
<blockquote class="episode-pullquote">
  "Your quote here."
</blockquote>
```

**Match results:**
```html
<div class="episode-results">
  <h3>Match Results</h3>
  <ul>
    <li><span class="result-match">Tag Match</span><span class="result-winner">Team A def. Team B (12:00)</span></li>
    <li><span class="result-match result-title">Main Event ★</span><span class="result-winner">Champ def. Challenger (25:00)</span></li>
  </ul>
</div>
```
