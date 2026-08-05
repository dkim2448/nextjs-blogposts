# nextjs-blogposts

content repo for my next.js mdx blog. holds the raw `.mdx` posts and images fetched at build/request time by the blog app.

## structure

- `*.mdx` — blog posts, one file per post. filename (minus extension) becomes the post's url slug.
- `images/` — images referenced inside posts.

## frontmatter

each post needs:

```yaml
---
title: post title
date: yyyy-mm-dd
tags: [tag1, tag2]
---
```

## notes

- renaming a `.mdx` file changes its slug/url — old links will 404.
- after editing/pushing a post, revalidate the corresponding path on the blog app to see changes live (see that repo's readme).
