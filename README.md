# Xntrova Technologies – Homepage Redesign

Responsive, conversion-focused homepage for a B2B digital marketing agency. Built with plain HTML, CSS and JavaScript. No frameworks or build step.

## Structure
```
index.html        semantic markup, single h1, SEO meta
css/style.css     design tokens, layout, components, responsive breakpoints
js/main.js        menu, scroll-spy, reveal/counters, filter, form validation
```

## Major changes
- Clear hero with value proposition, rotating headline and two CTAs
- Trust marquee, bento services grid, results band, FAQ accordion
- Portfolio filter, testimonials carousel on mobile, validated lead form
- Sticky mobile CTA bar, scroll progress, back-to-top, dark/light theme
- Zero dependencies (only Google Fonts), accessible (skip link, focus states, reduced motion)

## Responsive
Desktop (1000px+), tablet (721–1024px), mobile (up to 720px), plus small-phone and landscape tweaks.

## Browser support
Latest Chrome, Edge, Safari 15+, Firefox, Android and iOS browsers.

## Run locally
Open `index.html`, or run `python3 -m http.server` and visit http://localhost:8000.

## Deploy (free)
GitHub Pages: push to `main`, then Settings → Pages → Source: GitHub Actions. The included workflow deploys automatically.

## Notes
Case studies, logos, numbers and testimonials are placeholders. The form validates on the client only; connect Formspree/EmailJS or a backend to receive submissions.

## Netlify deploy
Drag the project folder to https://app.netlify.com/drop, or connect the GitHub repo (build command: none, publish directory: `.`). `netlify.toml` is included.
