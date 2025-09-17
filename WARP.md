# WARP.md

This file provides guidance to WARP (warp.dev) when working with code in this repository.

## Project Overview

This is a **single-page HTML portfolio website** for Samuel Adu, a Finance & Operations leader, Compliance strategist, and Data Science professional. The site is built using vanilla HTML5, CSS3, and JavaScript with a modern dark theme and responsive design.

## Architecture & Structure

### Core Files
- `index.html` - Single-page portfolio site containing all HTML, CSS (embedded), and JavaScript
- `netlify.toml` - Netlify deployment configuration with security headers and caching rules
- `README.md` - Project documentation with customization instructions

### Design System
The site uses CSS custom properties (CSS variables) defined in `:root`:
- Color scheme: Deep navy background (`#0f1724`) with cyan (`#06b6d4`) and purple (`#7c3aed`) accents
- Typography: Inter font family from Google Fonts
- Layout: CSS Grid and Flexbox for responsive design
- Max container width: 1100px

### Section Structure
The single-page layout includes these main sections:
1. **Hero Section** - Introduction with profile image, CTA buttons, and professional tags
2. **About Section** - Bio, core strengths, and three-column value propositions
3. **Portfolio Section** - 3x2 grid of featured projects (currently with placeholder content)
4. **Vision Section** - Mission statement in highlighted container
5. **Contact Section** - Professional info and contact form

## Common Commands

### Local Development
```bash
# Serve locally (using Python's built-in server)
python -m http.server 8000

# Alternative using Node.js http-server (if installed)
npx http-server .
```

### Deployment to Netlify
The site is configured for Netlify deployment:
- Publishes from root directory (`.`)
- Includes security headers and caching configuration
- No build process required (static HTML)

### Version Control
```bash
# Check current changes
git status
git diff

# Commit changes
git add .
git commit -m "Update portfolio content"
git push origin main
```

## Customization Guidelines

### Content Updates
- **Profile Image**: Replace placeholder in `.hero-right .profile-plate img` (line 119)
- **Contact Information**: Update email and LinkedIn URLs in contact section (lines 208-209)
- **Professional Tags**: Modify tags in hero section (lines 104-106)
- **Project Content**: Replace placeholder projects in portfolio grid (lines 171-187)
- **Video Content**: Add embedded video in hero section placeholder (line 112)

### Form Configuration
The contact form (lines 215-227) currently shows a demo alert. To make functional:
- Replace form `action` with form handler endpoint (Netlify Forms, Formspree, etc.)
- Remove demo `onsubmit` handler
- Add proper form processing

### Styling Modifications
All CSS is embedded in `<style>` tags (lines 10-86). Key style sections:
- CSS variables (lines 11-19)
- Hero section styles (lines 29-43)
- Card and grid layouts (lines 46-57)
- Responsive breakpoints (lines 73-80)

### Responsive Behavior
- **Desktop**: Hero uses flex layout with left content and right profile image
- **Mobile** (< 900px): Hero stacks vertically, grids become single column
- Portfolio grid: 3 columns → 1 column on mobile
- Contact section: Side-by-side → stacked on mobile

## Key Features

### Glass Morphism Design
- Semi-transparent containers with backdrop blur effects
- Subtle borders and gradients for depth
- Dark theme optimized for professional presentation

### Accessibility Considerations
- Semantic HTML structure
- Alt text for images
- Proper form labels
- Color contrast meets professional standards

### Performance Optimizations
- Single HTML file reduces HTTP requests
- External dependencies limited to Google Fonts
- Netlify caching headers for static assets
- Minimal JavaScript footprint

## Development Notes

- No build process or package management required
- Direct file editing workflow
- CSS and JavaScript are embedded in HTML for simplicity
- Responsive design uses modern CSS Grid and Flexbox
- Professional color palette suitable for business contexts

## Security Headers (Netlify)
The site includes security headers via `netlify.toml`:
- X-Frame-Options: DENY
- X-XSS-Protection: enabled
- X-Content-Type-Options: nosniff
- Referrer-Policy: strict-origin-when-cross-origin

## Future Enhancements
Common improvements to consider:
- Separate CSS into external stylesheet for maintainability
- Add smooth scroll navigation between sections
- Implement proper form backend integration
- Add loading animations or transitions
- Include SEO meta tags and structured data
