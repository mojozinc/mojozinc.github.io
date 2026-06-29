# Sandeep Jangra's Personal Site & Writing Platform

A simple, text-centric, zero-friction writing platform styled in the 2000s programmer-essayist aesthetic. It loads lightning fast, supports automatic system-level light/dark mode toggling, and requires no build steps.

## Publishing a New Essay

To write and publish a new article:

1. **Create the file**: Duplicate the template post `posts/my-first-post.html` and rename it (e.g., `posts/my-new-essay.html`).
2. **Write the content**:
   - Update the `<title>` and `<meta name="description">` tags in the `<head>`.
   - Update the `<h1>` title and meta dates/read-time under `<header class="article-header">`.
   - Write your thoughts using standard semantic HTML elements (like `<h2>`, `<p>`, `<code>`, `<pre>`, `<blockquote>`, `<ul>`, etc.).
3. **Register the post**: Add the post to the `<ul class="post-list">` section in `index.html` with its date and title.
4. **Deploy**: Push your changes to GitHub to update your live GitHub Pages site:
   ```bash
   git add .
   git commit -m "Publish: [Title of your post]"
   git push origin main
   ```

## Development & Local Preview

To preview the website locally, you can run any standard local web server in the root of this repository:

```bash
# Using Python 3
python3 -m http.server 8000

# Using Node.js (npx)
npx http-server -p 8000
```
Then visit `http://localhost:8000`.
