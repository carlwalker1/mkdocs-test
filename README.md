# Hello World Static Site

A simple static website built with Jekyll and Markdown, ready to deploy on GitHub Pages.

## Project Structure

```
hello-world-site/
├── _config.yml      # Jekyll configuration
├── index.md         # Homepage (Markdown)
├── .gitignore       # Git ignore file
└── README.md        # This file
```

## Local Development (Optional)

To preview your site locally before publishing:

1. Install Ruby and Jekyll:
   - Download Ruby from [rubyinstaller.org](https://rubyinstaller.org/)
   - Install Jekyll: `gem install jekyll bundler`

2. Run the local server:
   ```bash
   cd hello-world-site
   jekyll serve
   ```

3. Open your browser to `http://localhost:4000`

## Publishing to GitHub Pages

### Step 1: Create a GitHub Repository

1. Go to [GitHub](https://github.com) and sign in
2. Click the "+" icon in the top right, select "New repository"
3. Name your repository (e.g., `my-website` or `username.github.io`)
4. Choose "Public"
5. Do NOT initialize with README (we already have files)
6. Click "Create repository"

### Step 2: Push Your Code

Run these commands in your terminal:

```bash
cd hello-world-site
git add .
git commit -m "Initial commit: Hello World site"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/YOUR-REPO-NAME.git
git push -u origin main
```

Replace `YOUR-USERNAME` and `YOUR-REPO-NAME` with your actual GitHub username and repository name.

### Step 3: Enable GitHub Pages

1. Go to your repository on GitHub
2. Click "Settings" tab
3. Scroll down to "Pages" in the left sidebar
4. Under "Source", select "main" branch
5. Click "Save"
6. Wait a few minutes for GitHub to build your site
7. Your site will be available at: `https://YOUR-USERNAME.github.io/YOUR-REPO-NAME/`

## Editing Your Site

1. Edit `index.md` to change your homepage content
2. Create new `.md` files for additional pages
3. Update `_config.yml` to change site title and description
4. Commit and push changes:
   ```bash
   git add .
   git commit -m "Update content"
   git push
   ```

## Markdown Tips

Jekyll uses Kramdown for Markdown. You can use:
- Headers: `#`, `##`, `###`
- **Bold** and *italic* text
- Lists (bulleted and numbered)
- Links: `[text](url)`
- Images: `![alt text](image-url)`
- Code blocks with syntax highlighting
- Tables
- And much more!

## Customization

The site uses the "minima" theme by default. You can:
- Change the theme in `_config.yml`
- Browse themes at [jekyllthemes.org](https://jekyllthemes.org)
- Customize layouts by creating `_layouts/` directory
- Add custom CSS in `assets/css/`

## Learn More

- [Jekyll Documentation](https://jekyllrb.com/docs/)
- [GitHub Pages Documentation](https://docs.github.com/en/pages)
- [Markdown Guide](https://www.markdownguide.org/)

---

Happy building! 🚀
