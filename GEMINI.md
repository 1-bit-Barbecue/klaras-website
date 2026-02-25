# Klaras Web Page - Contextual Guidance

## Project Overview
This is a personal, bilingual portfolio website for Klara Brabec Wagnerova, a writer, song writer and poet. The site is designed to showcase her work across various mediums, including lyrics, comics, novels, and short stories.

### Core Technologies
- **Jekyll:** Framework used to generate the pages from markdown
- **HTML5:** Jekyll templates
- **CSS:** Site style
- **Markdown:** Site content in a human readable format

### Architecture & Structure
- The project follows standard Jekyll structure
- The site is GitHub pages compatible
- The initial content is in Website.docx
- The site is multilingual, English and Czech
- The file structrure
  - **_templates** - Jekyll templates for the nav bar, footer and the pages
  - **_styles** - CSS styles for the site
  - **_works** - Markdown with the infromation about the authors works
    - **_en** - English versions
      - **_lyrics**
      - **_comics**
      - **_novels**
      - **_shorts**
    - **_cz** - Czech versions
      - **_lyrics**
      - **_comics**
      - **_novels**
      - **_shorts**


## Building and Running
Jekyll build based on the Jekyll config

### Development
Build and test locally using `bundle exec jekyll serve`

## Development Conventions
- **Language Synchronization:** When adding or updating content, ensure that both the `en` and `cz` versions are updated to maintain parity. In case one language is missing, create empty stup with a TODO comment and show a warning message.
- **Styling:** All styling should be managed within the `_styles` directory to ensure visual consistency. Use the defined CSS variables for colors and fonts.
- **Navigation:** Maintain the navigation bar and footer across all pages. The `active-nav` and `active-lang` classes should be correctly applied to indicate the current page and language.
- **Image Placeholders:** Currently, images (like the author's photo) are represented by `image-placeholder` divs. When adding real images, ensure they are optimized for web use.
