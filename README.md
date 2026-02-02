# My Personal Blog

A simple, clean personal blog built with HTML and CSS, designed to be hosted on GitHub Pages.

## Features

- Clean, modern design
- Fully responsive (mobile-friendly)
- Easy to customize
- No dependencies or build process required
- Ready for GitHub Pages deployment

## Setup Instructions

### Option 1: Deploy to GitHub Pages

1. **Create a GitHub account** (if you don't have one)
   - Go to [github.com](https://github.com) and sign up

2. **Create a new repository**
   - Click the "+" icon in the top right and select "New repository"
   - Name it `yourusername.github.io` (replace `yourusername` with your actual GitHub username)
   - Make it public
   - Don't initialize with README (we already have files)

3. **Upload your blog files**
   - Download all the files from this blog
   - In your new repository, click "uploading an existing file"
   - Drag and drop all the blog files (index.html, style.css, about.html, and the posts folder)
   - Commit the changes

4. **Enable GitHub Pages**
   - Go to your repository Settings
   - Scroll down to "Pages" section
   - Under "Source", select "main" branch
   - Click Save

5. **Visit your blog!**
   - Your blog will be live at `https://yourusername.github.io`
   - It may take a few minutes for the site to appear

### Option 2: Using Git Command Line

If you're comfortable with Git:

```bash
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/yourusername/yourusername.github.io.git
git push -u origin main
```

## Customization

### Update Your Information

1. **Edit the header** in all HTML files:
   - Change "My Personal Blog" to your blog name
   - Update the tagline

2. **Update About page** (`about.html`):
   - Add your bio
   - Update contact information
   - Add your social media links

3. **Customize colors** in `style.css`:
   - Find the header gradient: `background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);`
   - Change link colors: look for `#667eea` and `#764ba2`

### Adding New Posts

1. Create a new HTML file in the `posts` folder
2. Copy the structure from an existing post
3. Update the content
4. Add a link to your new post on the homepage (`index.html`)

### File Structure

```
.
├── index.html          # Homepage with blog post list
├── about.html          # About page
├── style.css           # All styling
├── posts/
│   ├── first-post.html
│   └── second-post.html
└── README.md           # This file
```

## Adding a Custom Domain (Optional)

1. Buy a domain from a domain registrar (like Namecheap, Google Domains, etc.)
2. In your repository, create a file named `CNAME` with your domain (e.g., `myblog.com`)
3. Configure your domain's DNS settings:
   - Add an A record pointing to GitHub's IPs:
     - 185.199.108.153
     - 185.199.109.153
     - 185.199.110.153
     - 185.199.111.153
   - Or add a CNAME record pointing to `yourusername.github.io`

## Tips

- Write your posts in any text editor
- Keep images in an `images` folder and reference them with relative paths
- Commit regularly to keep a history of your changes
- Preview locally by opening `index.html` in your browser before pushing to GitHub

## Support

If you need help:
- Check [GitHub Pages documentation](https://docs.github.com/en/pages)
- Review [GitHub's guide to setting up Pages](https://pages.github.com/)

## License

Feel free to use this template for your own blog!
