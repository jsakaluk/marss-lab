# MARSS Lab Website

The **Methodology and Relationship/Sexual Science (MARSS) Lab** website, built with [Quarto](https://quarto.org/) and hosted on GitHub Pages.

## Quick Start

```bash
# Preview locally
quarto preview

# Render the full site
quarto render
```

## Structure

| Path | Purpose |
|------|---------|
| `index.qmd` | Homepage |
| `philosophy.qmd` | Lab Philosophy page |
| `join.qmd` | Join the Lab page |
| `people/` | Lab member profiles |
| `projects/` | Research projects and software |
| `papers/` | Publications (from BibTeX + YAML) |
| `blog/` | Blog posts |
| `images/` | Site-wide images and logos |
| `custom.scss` | Light mode styling |
| `custom-dark.scss` | Dark mode styling |
| `news.yml` | Lab news feed data |

## Adding Content

### New Lab Member

1. Copy `people/_template.qmd` to `people/your-name/index.qmd`
2. Add a profile photo as `people/your-name/avatar.jpg`
3. Edit the YAML front matter (`title`, `subtitle`, `description`, `group`, `order`)
4. Fill in the profile sections

### New Blog Post

1. Create `blog/posts/YYYY-MM-DD-slug/index.qmd`
2. Fill in the YAML front matter and write your post

### Updating Publications

1. Export your library from Zotero in BibTeX format
2. Replace `papers/references.bib`
3. Edit `papers/links.yml` to add tags and supplementary links for each entry

## Deployment

Push to the `main` branch. GitHub Actions will build and deploy automatically.

## AI Assistance

The creation of this site was greatly expedited through the use of Cursor + Opus 4.6. I feel perfectly fine about this decision: I understand how markdown and YAMLs work, but I had put this revamp off for *years* because of the time commitment it was going to require. 
