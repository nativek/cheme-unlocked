# How to Add Blog Posts to ChemE Unlocked

This guide explains how to add new blog articles to your ChemE Unlocked website.

## 🎯 Quick Start

Your website is **fully functional** and hosted at: **https://nativek.github.io/cheme-unlocked/**

### Current Structure:
- **Homepage:** `index.html` — displays all categories and recent posts
- **Template:** `_category-template.html` — use this to create category pages
- **Styling:** `style.css` — clean, modern design (green accent, responsive)

---

## Step 1: Create Category Pages

You currently have `_category-template.html` which you can duplicate for each category.

### Categories needed:
1. `fundamentals.html`
2. `transport-ops.html`
3. `reaction-engineering.html`
4. `process-design.html`
5. `ai-cheme.html`
6. `career.html`

### How to create a category page:

1. **Go to GitHub:** https://github.com/nativek/cheme-unlocked
2. **Click "Add file" → "Create new file"**
3. **Copy the content from `_category-template.html`**
4. **Replace the placeholders:**
   - `[CATEGORY NAME]` → e.g., "Fundamentals"
   - `[CATEGORY DESCRIPTION]` → e.g., "Engineering math, thermodynamics, physical chemistry, and mass/energy balances"
   - `[CATEGORY ICON]` → e.g., "⚗️" (use emojis from your index.html)
5. **Save as:** `fundamentals.html` (or whatever category name)
6. **Commit changes**

---

## Step 2: Write Your First Article

### Create a new folder structure:

```
cheme-unlocked/
  ├── index.html
  ├── fundamentals.html
  ├── style.css
  └── posts/
       ├── first-law-thermodynamics.html
       ├── mass-balance-intro.html
       └── bernoulli-equation.html
```

### Article Template:

Create a new file at `posts/your-article-title.html`:

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Your Article Title | ChemE Unlocked</title>
  <link rel="stylesheet" href="../style.css">
</head>
<body>
  <nav>
    <div class="nav-container">
      <a href="../index.html" class="logo">ChemE Unlocked</a>
      <ul class="nav-links">
        <li><a href="../index.html">Home</a></li>
        <li><a href="../fundamentals.html">Fundamentals</a></li>
        <li><a href="../transport-ops.html">Transport & Unit Ops</a></li>
        <li><a href="../reaction-engineering.html">Reaction Engineering</a></li>
        <li><a href="../process-design.html">Process Design</a></li>
        <li><a href="../ai-cheme.html">AI in ChemE</a></li>
        <li><a href="../career.html">Career</a></li>
      </ul>
    </div>
  </nav>

  <article>
    <h1>Your Article Title Here</h1>
    <div class="article-meta">
      📅 February 28, 2026 | ⏱️ 10 min read | 📚 Fundamentals
    </div>

    <p>Write your introduction here. Keep it engaging and explain what the reader will learn.</p>

    <h2>Section 1: Key Concept</h2>
    <p>Explain the concept in detail. You can use:</p>
    <ul>
      <li>Bullet points for lists</li>
      <li>Bold text for <strong>important terms</strong></li>
      <li>Inline code for equations: <code>PV = nRT</code></li>
    </ul>

    <h2>Section 2: Worked Example</h2>
    <p>Show a step-by-step example:</p>
    <pre>
Given: P = 1 atm, V = 22.4 L, T = 273 K
Find: n (moles of gas)

Solution:
PV = nRT
n = PV / RT
n = (1)(22.4) / (0.0821)(273)
n = 1.00 mol
</pre>

    <h2>Key Takeaways</h2>
    <ul>
      <li>Summary point 1</li>
      <li>Summary point 2</li>
      <li>Summary point 3</li>
    </ul>
  </article>

  <footer>
    <p>&copy; 2026 ChemE Unlocked | Built with passion for learning</p>
  </footer>
</body>
</html>
```

---

## Step 3: Add Post Card to Category Page

Once you've written an article, add it to the relevant category page.

### Example for `fundamentals.html`:

Find the empty state section and replace it with:

```html
<div class="post-grid">
  <div class="post-card">
    <div class="post-content">
      <div class="post-meta">
        <span>📅 February 28, 2026</span>
        <span>⏱️ 10 min read</span>
      </div>
      <h3>First Law of Thermodynamics Explained</h3>
      <p>A breakdown of energy conservation in closed systems, with real-world applications and worked examples.</p>
      <a href="posts/first-law-thermodynamics.html" class="read-more">Read more →</a>
    </div>
  </div>

  <!-- Add more post cards as you write articles -->
</div>
```

---

## Step 4: Update Homepage (Optional)

To feature your latest posts on the homepage (`index.html`), find the "Recent Posts" section and replace the empty state with the same post card grid.

---

## ✨ Tips for Writing

1. **Keep it simple:** Write like you're explaining to a friend
2. **Use examples:** Worked problems help readers understand
3. **Break it down:** Use headings (h2, h3) to organize content
4. **Add visuals:** You can add images using `<img src="..." alt="...">`
5. **Be consistent:** Use the same structure across all posts

---

## 🚀 Publishing Workflow

1. **Write locally or in GitHub editor**
2. **Commit to main branch**
3. **GitHub Pages auto-deploys** (takes 1-2 minutes)
4. **Check your site:** https://nativek.github.io/cheme-unlocked/

---

## 🛠️ Need Help?

- **Edit any file:** Go to the file on GitHub → Click the pencil icon → Make changes → Commit
- **Preview before commit:** Use the "Preview" tab in GitHub's editor
- **Delete a file:** Go to the file → Click trash icon → Confirm

**Your blog is ready to grow as you learn!** 🚀
