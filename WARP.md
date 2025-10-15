# WARP.md

This file provides guidance to WARP (warp.dev) when working with code in this repository.

## Project Overview

This is a **WDD 130: Web Fundamentals** coursework repository for Akamunyereka Kevin at BYU-Idaho. This course teaches HTML and CSS fundamentals through hands-on learning activities and projects. The repository contains weekly HTML/CSS exercises, a student portfolio homepage, and a comprehensive white water rafting website project.

## Development Environment

The project uses VS Code with the following setup:
- **Five Server** extension for local development server (port 5501)
- **Live Server** as backup (port 5503)  
- Auto-formatting enabled for HTML/CSS
- Spell checker configured with custom dictionary

## Commands

### Development Server
```bash
# Start Five Server (preferred, port 5501)
# Use VS Code extension: right-click HTML file → "Open with Five Server"

# Alternative: Start Live Server (port 5503)
# Use VS Code extension: right-click HTML file → "Open with Live Server"
```

### Validation and Testing
```bash
# Use W3C Validator for HTML validation
# Visit: https://validator.w3.org/

# Use W3C CSS Validator for CSS validation  
# Visit: https://jigsaw.w3.org/css-validator/

# Check contrast ratios for accessibility
# Visit: https://contrast-ratio.com/
```

### File Operations
```bash
# View file structure
Get-ChildItem -Recurse -Name

# Find specific file types
Get-ChildItem -Recurse -Include *.html, *.css

# Check git status
git status --porcelain

# Commit and sync workflow (as per course instructions)
git add .
git commit -m "Week ## activity completion"
git push origin main
```

## Repository Structure

### Main Components
- **`index.html`** - Student portfolio homepage with personal information and course links
- **`styles/styles.css`** - Main styling for the homepage
- **`wwr/`** - White Water Rafting website project (Rapids Edge Rafting company)
- **`week##/`** - Weekly learning exercises and assignments

### White Water Rafting Site (`wwr/`)
The main course project is a multi-page website for "Rapids Edge Rafting":
- **`about.html`** - Company history, mission, and adventure gallery
- **`contact.html`** - Contact information, team profiles, and contact form
- **`styles/rafting.css`** - Complete styling for the rafting site
- **`images/`** - All images for the rafting site (logos, photos, social media icons)

### Weekly Exercises (`week##/`)
Learning exercises are organized chronologically with specific focus areas:
- **Week 01** - File paths and basic HTML document structure
- **Week 02** - HTML semantic elements, CSS fundamentals, box model, block vs inline elements
- **Week 03** - CSS classes, IDs, floating elements, and advanced selectors
- **Week 04** - Flexbox layouts, responsive design, and layout exercises
- **Week 05** - HTML tables, advanced styling, and form elements
- **Week 06-07** - Advanced topics and project completion

## Architecture Patterns

### HTML Best Practices (Course Standards)
- **Semantic HTML5 elements** - Use `<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<aside>`, `<footer>` instead of generic `<div>` elements
- **Proper heading hierarchy** - Use h1-h6 tags in correct order without skipping levels
- **Required meta elements** - Every page must include:
  - `<meta name="description" content="...">`
  - `<meta name="author" content="...">`
  - `<meta name="viewport" content="width=device-width, initial-scale=1.0">`
- **Accessibility focus** - Alt text for all images, proper form labels, semantic markup
- **Image optimization** - All images must be under 100kB file size

### CSS Organization Patterns
- **Box model mastery** - Understanding content, padding, border, margin relationships
- **CSS shorthand notation** - Preferred for conciseness (e.g., `margin: 10px 20px;`)
- **Color specification methods** - Support for keywords, hex, RGB/RGBA, HSLA formats
- **Responsive units** - Mix of absolute (px) and relative (%, em, rem) units
- **Block vs inline elements** - Proper understanding and application of display types

### Course-Specific Requirements
- **W3C validation** - All HTML and CSS must validate without errors
- **Contrast ratio compliance** - All text/background combinations must meet accessibility standards
- **GitHub Pages deployment** - All work must be accessible via GitHub Pages URLs
- **Consistent file structure** - CSS files in `styles/` subfolder, images in `images/` subfolder

## Development Notes

### VS Code Configuration
The `.vscode/settings.json` file is configured for beginner web development:
- **Auto-formatting** enabled for HTML/CSS on save and paste
- **Five Server** extension recommended (port 5501) with Live Server backup (port 5503)
- **Smart Git workflow** - Auto-staging, simplified sync process
- **Spell checking** with custom dictionary for student names
- **Simplified UI** - minimized panels for focus on coding fundamentals

### Course Learning Progression
**Week 02 Focus Areas:**
- HTML semantic elements vs non-semantic (`<div>`, `<span>`)
- CSS Box Model understanding (content, padding, border, margin)
- Block vs inline element behavior
- CSS units of measurement (absolute vs relative)
- Proper meta tag implementation
- W3C validation requirements

### Assignment Workflow
1. **Local Development** - Use Live/Five Server for testing
2. **Git Operations** - Commit with descriptive messages, sync to GitHub
3. **Validation** - Check HTML/CSS with W3C validators
4. **GitHub Pages Testing** - Verify live deployment
5. **Accessibility Check** - Ensure contrast ratios meet standards

### File Naming Conventions
- HTML files: `kebab-case.html` (e.g., `basic-layout.html`)
- CSS files: `kebab-case.css` in `styles/` subfolder
- Images: Descriptive names, optimized under 100kB
- Weekly structure: `week##/` folders with consistent organization

### Common Validation Issues
- Missing `alt` attributes on images
- Incorrect heading hierarchy (skipping h2 to h4)
- Invalid HTML structure (unclosed tags, improper nesting)
- CSS syntax errors (missing semicolons, invalid values)
- Poor color contrast ratios
