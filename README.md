# Jekyll Portfolio Site Generator

**Live Site:** [kristofer.site](https://kristofer.site/site.html)  
**Deployed Repository:** [maanum.github.io](https://github.com/Maanum/maanum.github.io)

## Overview

This is the Jekyll source code for my personal portfolio website. The site showcases my experience in digital product discovery and delivery, providing a more engaging overview of projects and skills than traditional resume formats.

## Architecture

This repository contains the Jekyll source code that generates static files deployed to the separate `maanum.github.io` repository via Git submodules:

```
jekyll-site/
├── _site/          # Built files (submodule → maanum.github.io)
├── _data/          # Project and tool data files
├── _includes/      # Reusable components (project cards, icons)
├── _layouts/       # Page templates
├── _sass/          # CSS styling
└── *.md            # Content pages
```

## Key Features

- **Data-Driven Content**: Projects and tools managed in YAML data files
- **Component System**: Reusable project cards and icon components
- **Template-Based**: Consistent layouts with Markdown content
- **Minimal JavaScript**: Focus on raw HTML/CSS implementation
- **Responsive Design**: Clean, professional presentation

## Development

### Prerequisites
- Ruby
- Jekyll (`gem install jekyll bundler`)

### Local Development
```bash
git clone https://github.com/Maanum/jekyll-site.git
cd jekyll-site
bundle install
jekyll serve --watch
```

### Adding Content
- **New Projects**: Add entries to `_data/projects.yml`
- **New Tools**: Add entries to `_data/tools.yml`
- **Project Pages**: Create new `.md` files using existing templates

### Deployment
The `_site` directory is a Git submodule pointing to the live site repository. Changes are automatically deployed when the submodule is updated.

---

*The built site files are served from the [maanum.github.io](https://github.com/Maanum/maanum.github.io) repository.*
