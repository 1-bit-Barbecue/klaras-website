# klaras-website

Portfolio website of Klara Brabec Wagnerova - A multilingual Jekyll site showcasing poetry and novel collections.

## Overview

This is a static website built with Jekyll, featuring a clean, professional design with support for multiple languages (English and Czech). The site includes portfolio sections for poems and novels, along with about and contact pages.

## How to Edit the Website

### Editing Pages

The main pages (About, Contact, etc.) are located in language-specific directories:

- **English pages**: `/en/` directory
  - `/en/about.md` - Edit the About page
  - `/en/contact.md` - Edit the Contact page
  - `/en/portfolio-novels.md` - Novel portfolio page
  - `/en/portfolio-poems.md` - Poetry portfolio page

- **Czech pages**: `/cz/` directory
  - `/cz/about.md` - O mně page
  - `/cz/contact.md` - Kontakt page
  - `/cz/portfolio-novels.md` - Romány page
  - `/cz/portfolio-poems.md` - Básně page

Simply edit the markdown files to update page content. Changes will be reflected when the site is commited. GitHub automatically builds and publishes a new version within a couple of minutes.

### Adding New Poems

Poems are stored in collections in the `/_poems/` directory, organized by language.

**To add a new poem:**

1. Create a new markdown file in the appropriate language folder:
   - English: `/_poems/en/your-poem-name.md`
   - Czech: `/_poems/cz/your-poem-name.md`

2. Add front matter at the top of the file:
   ```yaml
   ---
   language: en
   name: "Your Poem Title"
   ---
   ```

3. Add your poem content below the front matter:
   ```markdown
   ---
   language: en
   name: "My Beautiful Poem"
   ---
   
   Your poem text goes here...
   ```

The poem will automatically appear in the poems portfolio grid.

### Adding New Novels

Novels are stored in the `/_novels/` directory, organized by language.

**To add a new novel:**

1. Create a new markdown file in the appropriate language folder:
   - English: `/_novels/en/your-novel-name.md`
   - Czech: `/_novels/cz/your-novel-name.md`

2. Add front matter at the top of the file:
   ```yaml
   ---
   language: en
   name: "Your Novel Title"
   ---
   ```

3. Add your novel description or content:
   ```markdown
   ---
   language: en
   name: "My Epic Novel"
   ---
   
   Your novel description or content goes here...
   ```

The novel will automatically appear in the novels portfolio grid.

## File Structure

```
/en/                 # English language pages
/cz/                 # Czech language pages
/_novels/            # Novel collection
  /en/               # English novels
  /cz/               # Czech novels
/_poems/             # Poetry collection
  /en/               # English poems
  /cz/               # Czech poems
/_layouts/           # Page templates
/_includes/          # Reusable page components
/_sass/              # Styling
/_data/              # Configuration data
```

## Building and Running Locally

Local build and testing requires Jekyll to be installed on the system and available in the CLI, [official guide](https://jekyllrb.com/docs/installation/).

To build and serve the site locally:

```bash
npm run serve
```

The site will be available at `http://localhost:4000`

## Customization

### Navigation
Edit `_data/navigation.yaml` to modify the main navigation menu for each language.

### Footer
Edit `_includes/footer.html` and `_data/footer.yaml` to update footer content.

### Styling
The site uses SCSS for styling. Main styles are in `_sass/main.scss`.

## Languages

The site supports multiple languages (English and Czech). Language-specific content is organized in separate directories and collections, allowing for a fully multilingual experience.

TODO
- missing social media links