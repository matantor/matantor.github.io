# matanspector.com

Personal website and blog for Matan Spector, built with Jekyll and hosted on GitHub Pages.

**Live site:** [matanspector.com](https://matanspector.com)

## Tech Stack

- **Jekyll** - Static site generator (GitHub Pages default)
- **Tailwind CSS** - Styling via CDN (no build step required)
- **GitHub Pages** - Hosting

## Project Structure

```
.
├── _config.yml          # Jekyll configuration
├── _layouts/            # HTML templates
│   ├── default.html     # Base layout with nav and footer
│   ├── home.html        # Home/About page layout
│   └── post.html        # Blog post layout
├── _posts/              # Published blog posts (empty by default)
├── _drafts/             # Draft posts (not published)
├── index.md             # Home page content
├── blog.html            # Blog index page
├── tags.html            # Tags index page
├── CNAME                # Custom domain configuration
└── README.md            # This file
```

## Adding a New Blog Post

1. Create a new file in the `_posts/` directory with the naming format:
   ```
   YYYY-MM-DD-title-with-dashes.md
   ```
   Example: `2025-01-15-my-first-post.md`

2. Add the required front matter at the top of the file:
   ```yaml
   ---
   layout: post
   title: "My Post Title"
   date: 2025-01-15
   tags: [crypto, investing]
   ---
   ```

3. Write your post content in Markdown below the front matter.

4. Commit and push to GitHub:
   ```bash
   git add .
   git commit -m "Add new blog post: My Post Title"
   git push
   ```

GitHub Pages will automatically build and deploy your changes.

### Available Tags

Suggested tags (you can use any tags you want):
- `crypto` - Blockchain and cryptocurrency topics
- `investing` - Markets and investment ideas
- `ai` - Artificial intelligence and machine learning
- `environment` - Sustainability and climate
- `general` - General thoughts and observations

### Front Matter Template

```yaml
---
layout: post
title: "Your Post Title Here"
date: YYYY-MM-DD
tags: [tag1, tag2]
---
```

## Working with Drafts

Files in the `_drafts/` folder are **not published** by GitHub Pages. Use drafts to work on posts that aren't ready for publication.

### Creating a Draft

1. Create a file in `_drafts/` (no date prefix needed):
   ```
   _drafts/my-upcoming-post.md
   ```

2. When ready to publish, move it to `_posts/` and add the date prefix:
   ```
   _posts/2025-01-15-my-upcoming-post.md
   ```

### Previewing Drafts Locally

To see drafts when running Jekyll locally:
```bash
jekyll serve --drafts
```

## Local Development

To run the site locally:

1. Install Jekyll: https://jekyllrb.com/docs/installation/
2. Run the development server:
   ```bash
   bundle exec jekyll serve
   ```
3. Open http://localhost:4000 in your browser

## License

Content is copyright Matan Spector. All rights reserved.
