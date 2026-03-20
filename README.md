# corbett.ai

Personal website of Justin Corbett — built with Jekyll, hosted on GitHub Pages.

## Running locally

1. Clone the repo
2. Run `bundle install`
3. Run `bundle exec jekyll serve`
4. Open <http://localhost:4000>

## Writing a post

Create a file in `_posts/` named `YYYY-MM-DD-title.md` with front matter:

```yaml
---
title: Your Post Title
description: A short description for SEO and post previews.
tags: [tag1, tag2]
image: /assets/img/your-image.jpg  # optional, used as the card image
---
```

## Adding a project

Create a file in `_projects/` with front matter:

```yaml
---
title: Project Name
description: Short description.
links:
  - title: View Project
    url: https://example.com
---
```

## Stack

- [Jekyll](https://jekyllrb.com) 4.3
- Custom theme — no external CSS framework
- Hosted on [GitHub Pages](https://pages.github.com)
