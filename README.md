# Adding the Blog to Loopwork System

## What's in this folder

```
_config.yml          ← Jekyll configuration (drop in repo root)
_layouts/
  post.html          ← Blog post template (create _layouts folder in repo)
_posts/
  2026-05-30-sample-post.md  ← Example post (create _posts folder in repo)
blog/
  index.html         ← Blog listing page (create blog folder in repo)
  blog.css           ← Blog styles (goes inside blog folder)
```

## Setup (one time, ~5 minutes)

1. **Copy all 5 files into your GitHub repo** in the same folder structure shown above.

2. **Add "Blog" to the nav** on your existing pages (index.html, about.html, publications.html, contact.html). Find this line in each file:

   ```html
   <li><a href="publications.html">Publications</a></li>
   <li><a href="contact.html">Contact</a></li>
   ```

   Add the blog link between Publications and Contact:

   ```html
   <li><a href="publications.html">Publications</a></li>
   <li><a href="/blog/">Blog</a></li>
   <li><a href="contact.html">Contact</a></li>
   ```

3. **Push to GitHub.** That's it. GitHub Pages builds the site automatically with Jekyll.

## Writing a new post

1. Create a new file in `_posts/` named: `YYYY-MM-DD-your-title.md`
2. Add front matter at the top (copy from the sample post)
3. Write your post in markdown below the front matter
4. Push to GitHub

The post will appear on your blog page and be indexed by Google under your domain.

## SEO notes

- The `description` in front matter becomes your Google search snippet
- Tags help with keyword relevance
- Each post gets its own canonical URL at loopworksystem.com/blog/YYYY/MM/title/
- Open Graph and Twitter cards are auto-generated for social sharing
- Set `scholar: true` in front matter for posts you want indexed by Google Scholar

## Cross-posting workflow

1. Write and publish on loopworksystem.com first (this is your canonical source)
2. Wait 1-2 days for Google to index it
3. Cross-post to Substack with a note: "Originally published at loopworksystem.com"
4. Optionally cross-post to Medium using their "import" feature (it respects canonical URLs)

This way Google always treats your site as the original source.
