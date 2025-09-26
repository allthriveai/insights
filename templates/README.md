# All Thrive AI - Insights

This repository contains insight articles and content for All Thrive AI, managed as both an Obsidian vault and a git subtree.

## Repository Structure

This repository is managed as a git subtree of the main [allthriveai/allthriveai](https://github.com/allthriveai/allthriveai) repository, allowing for:

- **Obsidian Integration**: Can be linked directly to Obsidian as a vault
- **Content Management**: Independent versioning of insight articles
- **Main Project Integration**: Automatically synced with the main website

## Usage

### For Content Authors
1. Clone or link this repository to Obsidian
2. Use `insight-article-template.md` as a starting point for new articles
3. Follow the markdown guidelines and frontmatter structure
4. Commit and push changes to sync with the main website

### For Developers
Changes made in the main repository's `/insights` folder automatically sync here via git subtree operations.

## Article Template

Use `insight-article-template.md` for creating new insight articles. It includes:
- Complete frontmatter structure
- Markdown reference with help text
- Obsidian-specific elements
- SEO and accessibility guidelines

## Frontmatter Fields

Required fields for all articles:
```yaml
title: "Article Title"
author: "Author Name"
date: "YYYY-MM-DD"
categories: ["Category 1", "Category 2"]
featured_image: "/insights/images/image.png"
excerpt: "Brief description for SEO"
featured_on_homepage: true/false
priority: 1-100 (lower = higher priority)
draft: false
```

## Git Subtree Operations

This repository is managed via git subtree. Common operations:

```bash
# Push changes from main repo to insights repo
git subtree push --prefix=insights insights main

# Pull changes from insights repo to main repo
git subtree pull --prefix=insights insights main
```

---

*This repository is part of the All Thrive AI ecosystem. Visit [allthriveai.com](https://allthriveai.com) for more information.*