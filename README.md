# Mary's Portfolio

A responsive, single-page personal portfolio for a computer science student, built with pure HTML and CSS plus a little JavaScript.

**Live site:** `https://your-username.github.io/portfolio-site/` _(replace after deploying)_

## Overview

This site introduces who I am, what I can do and what I have built, and gives visitors an easy way to get in touch. It was designed mobile first, so it looks good on a phone and scales up to a wide desktop screen.

The project meets a set of technical requirements: organised files, Git history from the start, semantic HTML, a form with varied field types, Grid, Flexbox and positioning in CSS, transforms, an animation, a custom font and a README.

## Features

- **Responsive layout** that works from small phones to large desktops
- **Sticky navigation** on larger screens, with smooth scrolling and an animated underline
- **Hero section** with a floating avatar, a rotating ring and staggered fade-in text
- **About, Skills and Projects sections** using cards, chips and an auto-fitting grid
- **Contact form** with many field types and built-in browser validation
- **Live form helpers** (JavaScript): character counter, timeline slider value and a minimum date
- **Accessibility**: skip link, visible focus styles, labelled form fields, alt text, AA colour contrast and `prefers-reduced-motion` support
- **Back-to-top button** fixed to the corner of the screen

## Structure

```
portfolio-site/
├── index.html              # Page content (semantic HTML)
├── README.md
├── .gitignore
├── css/
│   └── style.css           # All styles in labelled sections: tokens, layout, components, animations
├── js/
│   └── main.js             # Form helpers and footer year
└── images/
    ├── favicon.svg
    ├── profile-placeholder.svg
    ├── project-planner.svg
    ├── project-visualizer.svg
    └── project-notes.svg
```

### Where each requirement lives

| Requirement | Where |
| --- | --- |
| Images and favicon in their own folder | `images/` |
| Semantic HTML (`header`, `nav`, `main`, `section`, `article`, `aside`, `figure`, `footer`, `form`, `fieldset`) | `index.html` |
| Form with different fields and attributes | `#contact-form` in `index.html` |
| At least 2 transformations | `css/style.css`: `scaleX`, `translateY`, `rotate`, `scale` |
| At least 1 animation | `css/style.css`: `float`, `spin`, `fade-up`, `draw-line` |
| Grid | `css/style.css`: hero, about, skills, projects, contact, form rows |
| Flexbox | `css/style.css`: header, nav, footer, buttons, chips |
| Positioning | `sticky` header, `relative` + `absolute` badges and tags, `fixed` back-to-top button |
| Custom font | Google Fonts: Fraunces (headings) and DM Sans (body) |
| Responsive from day one | Mobile-first CSS with `min-width` media queries |

### Form fields used

`text` (with `required`, `minlength`, `maxlength`, `autocomplete`, `placeholder`), `email`, `tel` (with `pattern` and `title`), `url`, a `readonly` text field, `select` with `optgroup`, `radio` group, `date`, `range` with `output`, `textarea`, `checkbox` (`required`), `hidden`, plus `submit` and `reset` buttons.

## Design

- **Palette** (from [coolors.co](https://coolors.co/b59539)): Ink `#0D1B2A`, Navy `#1B263B`, Slate `#415A77`, Mist `#778DA9`, Gold `#B59539`, Paper `#F6F5F0`. A darker gold `#7D6620` is used for text on light backgrounds so contrast stays high.
- **Typography**: Fraunces for headings, DM Sans for body text, with system font fallbacks.
- **Spacing**: a small scale of CSS variables (`--space-1` to `--space-6`) keeps margins and padding consistent.

## Getting started

No build step is needed.

```bash
git clone https://github.com/your-username/portfolio-site.git
cd portfolio-site
# open index.html in your browser, or use a local server:
python3 -m http.server 8000
```

Then visit `http://localhost:8000`.

## Customising

1. Edit text in `index.html` (hero, about, skills and projects). Look for the HTML comments that say what to replace.
2. Replace the SVGs in `images/` with your own photo and project screenshots, and update the `alt` text.
3. Update the GitHub and LinkedIn links in the footer and the project cards.
4. Change colours or fonts in the `:root` block of `css/style.css`.

## Deployment

### GitHub Pages

```bash
git branch -M main
git remote add origin https://github.com/your-username/portfolio-site.git
git push -u origin main
```

Then open the repository on GitHub: **Settings → Pages → Build and deployment**, choose **Deploy from a branch**, select `main` and `/ (root)`, and save. The site goes live at `https://your-username.github.io/portfolio-site/` after a minute or two.

### Netlify

- **Drag and drop:** drop the project folder onto the Netlify dashboard, or
- **From Git:** connect the GitHub repository. Leave the build command empty and set the publish directory to `.`

## Making the form work

On a static site the form cannot send email by itself. At the moment `main.js` shows a thank-you message instead. To receive real messages:

- **Netlify:** the form already has `data-netlify="true"` and a hidden `form-name` field. Remove the `event.preventDefault()` submit handler in `js/main.js` (or send the data with `fetch`) and submissions will appear in the Netlify dashboard.
- **Formspree or similar:** set the form's `action` to the endpoint they give you.

## Future improvements

- Connect the contact form to a real form service
- Add a dark mode toggle using the existing CSS variables
- Replace placeholder projects with real case studies and live demo links
- Add a downloadable CV and a short "Experience" timeline
- Add a mobile hamburger menu
- Fade sections in on scroll with `IntersectionObserver`
- Add a blog or notes section for what I learn in my courses
- Add meta tags for social sharing (Open Graph image)
- Run an accessibility and performance audit with Lighthouse

## Credits

- Fonts: [Fraunces](https://fonts.google.com/specimen/Fraunces) and [DM Sans](https://fonts.google.com/specimen/DM+Sans) via Google Fonts
- Colour palette: [Coolors](https://coolors.co/b59539)
- Illustrations: hand-written SVGs included in `images/`
