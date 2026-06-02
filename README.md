# MAGIC — Meeting Automotive Liability Challenges through Forensics Soundness

Official website for the MAGIC research project, an FFI-funded Swedish automotive cybersecurity project (Vinnova D-nr: 2024-03687).

**Live site:** https://magic-ffi-project.github.io

## Project overview

MAGIC develops automotive digital forensics (ADF) solutions to support liability investigations in vehicle incidents, enhance cybersecurity resilience, and ensure forensic soundness across the vehicle lifecycle (2025–2028).

**Partners:** Volvo Technology AB (coordinator), Chalmers, Volvo Car Group, RISE, AFRY, Clavister

## Local development

Prerequisites: Ruby 3.x, Bundler

```bash
gem install jekyll bundler   # one-time setup
bundle install               # install dependencies
bundle exec jekyll serve --livereload
```

Open http://localhost:4000 to preview the site.

## Site structure

```
_layouts/       Base and page-specific HTML layouts
_includes/      Header and footer partials
assets/
  css/          SCSS stylesheet (main.scss)
  img/          Images (hero.jpg, partner logos)
  icons/        Favicon and web manifest
about/          Project description, team, regulations
work-packages/  WP1-WP6 details
partners/       Consortium partner profiles
publications/   Deliverables and target venues
news/           Project updates
contact/        Contact information
```

## Deployment

Pushes to `main` are automatically deployed via GitHub Actions to GitHub Pages.
