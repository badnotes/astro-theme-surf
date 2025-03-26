# Astro Blog

A modern blog built with Astro, TailwindCSS, and MDX.

## Features

- 📝 MDX for writing blog posts
- 🎨 TailwindCSS for styling
- 📱 Responsive design
- ⚡️ Fast performance
- 🔍 SEO optimized
  - Meta tags and Open Graph support
  - Automatic sitemap generation
  - RSS feed
  - Structured data for better search results

## Getting Started

1. Install dependencies:
```bash
npm install
```

2. Start the development server:
```bash
npm run dev
```

3. Build for production:
```bash
npm run build
```

## Writing Posts

Create new blog posts by adding `.mdx` files in the `src/pages/posts` directory. Each post should include frontmatter with the following fields:

```yaml
---
layout: ../../layouts/Layout.astro
title: Your Post Title
date: YYYY-MM-DD
description: A brief description of your post
categories: ["Category1", "Category2"]  # Optional: Add categories for your post
tags: ["tag1", "tag2", "tag3"]         # Optional: Add tags for your post
image: "/path/to/image.jpg"            # Optional: Featured image for social sharing
author: "Author Name"                   # Optional: Post author
---
```

## SEO Configuration

The blog comes with built-in SEO features:

1. **Meta Tags**: Each page automatically generates proper meta tags based on your content
2. **Open Graph**: Social media sharing is optimized with Open Graph tags
3. **Sitemap**: Automatically generated at `/sitemap.xml`
4. **RSS Feed**: Available at `/rss.xml`
5. **Structured Data**: JSON-LD for better search engine understanding

To customize site-wide SEO settings, edit `src/config.ts`:

```ts
export const SITE = {
  title: 'Your Site Title',
  description: 'Your site description',
  defaultLanguage: 'en-us',
  website: 'https://your-domain.com',
  author: 'Your Name',
  twitter: '@yourhandle'  // Optional
}
```

