[![Netlify Status](https://api.netlify.com/api/v1/badges/8fd7da5f-0c4d-4a43-9e23-2d1baf0d35cc/deploy-status)](https://app.netlify.com/sites/kavinsood/deploys)

# Portfolio and Blog Website

A port of [Narative](https://www.narative.co/)'s beautiful Gatsby theme [Novela](https://narative.co/design/open/novela/) for Hugo 🚀🚀

## Prerequisites

- Go > 1.12
- Hugo > 0.65.0 

## Content Management System

Use your CMS of choice, or none at all.

## Deploy on Netlify

Import your repository in [Netlify](https://netlify.com)

1. Create a new site in Netlify and import your repository.
2. Set the build command to: `hugo --gc --minify`
3. Set the publish directory to: `public`
4. Set `GO_VERSION` to `1.12` or above
4. Set `HUGO_VERSION` to `0.85.0` or above

That's it, now your site gets deployed automatically on `git push` or when saving documents from Forestry.

## Development

```bash
# clone your repository
# cd in your project directory
# Start local server
hugo server
```

For more information, see [official Hugo documentation](https://gohugo.io/getting-started/).

## Customization

### Logo

Add to your projects layout directory your logo's SVG:
`/layouts/icons/ui/logo.html`

### Socials

In order for the Socials to be surfaced in Forestry, you should copy the theme's `config/_default/social.yaml` to your project.

### Authors

You should register authors as a taxonomy in your project's `config.yaml``

```yaml
taxonomies:
  author: authors
```

#### Creating authors

Add a similar file to your content directory and Front Matter example.

```yaml
# /content/authors/firstname-lastname/_index.md
---
title: Full Name
bio: |
  Written by You. This is where your author bio lives. Share your work, your
  joys and of course, your Twitter handle.
avatar: /images/your-picture.jpg
featured: true
social:
  - title: github
    url: https://github.com
  - title: twitter
    url: https://twitter.com
  - title: instagram
    url: https://instagram.com
  - title: dribbble
    url: https://dribbble.com
  - title: unsplash
    url: https://unsplash.com
---
```

#### Assigning authors to posts.

Add the name of the author to the "authors" field:

```yaml
authors:
  - Your Name
```

## LICENSE

MIT
