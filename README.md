# DwQ's Personal Blog - Powered by Jekyll

A clean, simple personal blog built with Jekyll and hosted on GitHub Pages.

## What is Jekyll?

Jekyll is a static site generator that GitHub Pages supports natively. It allows you to:
- Write blog posts in simple Markdown instead of HTML
- Automatically generate your homepage with all posts
- Use templates (layouts) to avoid repeating code
- Never manually update your homepage again!

## Current Setup

Your blog is now using Jekyll! Here's the structure:

```
.
├── _config.yml           # Site configuration (title, tagline, etc.)
├── _layouts/             # HTML templates
│   ├── default.html      # Main page template
│   └── post.html         # Blog post template
├── _posts/               # Your blog posts (Markdown files)
│   ├── 2025-01-15-welcome-to-my-blog.md
│   └── 2025-01-20-getting-started-with-github-pages.md
├── assets/
│   └── css/
│       └── style.css     # Styling
├── index.html            # Homepage (auto-generates post list)
├── about.md              # About page
└── README.md             # This file
```

## How to Add a New Blog Post

### Method 1: GitHub Web Interface (No computer needed!)

1. **Go to your repository** on GitHub: `https://github.com/davidwquinlan/davidwquinlan.github.io`

2. **Navigate to the `_posts` folder** and click "Add file" → "Create new file"

3. **Name your file** using this format:
   ```
   _posts/YYYY-MM-DD-your-post-title.md
   ```
   Example: `_posts/2025-02-02-my-third-post.md`
   
   **Important:** 
   - Must start with the date in `YYYY-MM-DD` format
   - Must end with `.md`
   - Use hyphens instead of spaces in the filename

4. **Add the front matter** at the top of the file:
   ```markdown
   ---
   layout: post
   title: "Your Post Title Here"
   date: 2025-02-02
   ---
   ```

5. **Write your post** below the front matter using Markdown:
   ```markdown
   This is my first paragraph. I can write naturally without HTML tags!

   ## This is a heading

   Here are some things I learned:
   - First point
   - Second point
   - Third point

   I can make text **bold** or *italic*.

   [This is a link](https://example.com)
   ```

6. **Commit the file** - Your post will appear on your blog in about 30 seconds!

### Method 2: Mobile (Same as above!)

The GitHub mobile website works the same way. You can write posts from your phone!

## Markdown Quick Reference

Markdown is much simpler than HTML. Here's what you need to know:

```markdown
# Heading 1
## Heading 2
### Heading 3

**Bold text**
*Italic text*

- Bullet point
- Another bullet point

1. Numbered item
2. Another numbered item

[Link text](https://example.com)

> This is a quote

`code text`
```

That's it! No `<p>`, `<strong>`, `<h2>` tags needed.

## Customizing Your Blog

### Change the Title and Tagline

Edit `_config.yml`:
```yaml
title: Your Blog Name
tagline: Your tagline here
description: A brief description
url: "https://davidwquinlan.github.io"
```

After changing `_config.yml`, you need to wait a few minutes for GitHub Pages to rebuild.

### Update Your About Page

Edit `about.md` - it's in Markdown, so easy to update!

### Change Colors

Edit `assets/css/style.css` and look for:
- Header gradient: `background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);`
- Link colors: `#667eea` and `#764ba2`

## How Jekyll Works (Behind the Scenes)

When you push changes to GitHub:

1. GitHub detects you're using Jekyll (because of `_config.yml`)
2. Jekyll reads all your posts from the `_posts` folder
3. Jekyll generates HTML pages from your Markdown
4. Jekyll uses the layouts to wrap your content
5. Your site is published at `https://davidwquinlan.github.io`

**You never see this process - it just works!**

## Troubleshooting

**Post not showing up?**
- Check the filename format: `YYYY-MM-DD-title.md`
- Make sure the date in the front matter matches
- Ensure the front matter has the three dashes `---` at the top and bottom
- Wait 1-2 minutes for GitHub to rebuild

**Site looks broken?**
- Check that `_config.yml` wasn't accidentally modified
- Make sure all layout files are in `_layouts/`
- Check CSS file is at `assets/css/style.css`

**Front matter example (copy this for new posts):**
```markdown
---
layout: post
title: "My Post Title"
date: 2025-02-02
---

Your content starts here...
```

## Tips for Writing Posts

1. **Keep file naming consistent:** Always use `YYYY-MM-DD-title.md`
2. **Write drafts in any text editor** then paste into GitHub
3. **Preview locally (optional):** If you want to see posts before publishing, you can install Jekyll on your computer, but it's not necessary
4. **Use descriptive titles** that work well in URLs (they'll become `/posts/your-title/`)
5. **The newest post (most recent date) appears first** on your homepage automatically

## Examples

**Good filename:**
```
_posts/2025-02-02-learning-javascript.md
```

**Bad filename:**
```
2025-02-02-learning-javascript.md  (missing _posts/)
learning-javascript.md              (missing date)
2025/02/02/post.md                 (wrong format)
```

## Next Steps

1. Delete the old HTML post files if they're still in your repository (not in `_posts`)
2. Start writing new posts in the `_posts` folder
3. Customize the about page
4. Change colors if you want

That's it! Enjoy your new Jekyll-powered blog. Writing posts is now as simple as creating a Markdown file on GitHub!
