# From The Beginning - Website

Website for https://fromthebeginning.xyz - supporting site and SEO companion for the YouTube channel [From The Beginning](https://www.youtube.com/@FromTheBeginning9).

Built with Jekyll on GitHub Pages. No build step needed: push Markdown, GitHub publishes.

## Add a new story

1. Copy `episode-template.md` into `_posts/`
2. Rename: `YYYY-MM-DD-slug.md` (slug = permalink from the FTB blog file)
3. Fill in title, description, tags and the real `youtube_id`
4. Paste the story content below the front matter
5. Commit and push. The homepage, /stories/ and sitemap.xml update automatically.

## Do not delete

- `CNAME` - connects the site to fromthebeginning.xyz
- `_config.yml`, `_layouts/` - site settings and templates
