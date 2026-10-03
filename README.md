# Xntrova Technologies – Homepage Redesign

Responsive, conversion-focused homepage for Xntrova Technologies, a B2B digital marketing agency.

- **Live demo:** https://xntrova-homepage.netlify.app/
- **Repository:** https://github.com/shantanughit/xntrova-homepage-Public

## Tech
Plain HTML, CSS and vanilla JavaScript in a single `index.html` (CSS in one `<style>` block, JS in one `<script>` block). No frameworks, no build step. Only external resource: Google Fonts (with system-font fallback).

## Sections
Header/navigation, hero, trust marquee, services, about, why choose us, process, results, portfolio (filterable), testimonials, FAQ, CTA banner, contact/lead form, footer.

## Major changes
- B2B-first hero with rotating headline and two clear CTAs
- Trust signals early: logo marquee, results counters, testimonials
- Bento services grid, filterable portfolio with hover overlay, FAQ accordion
- Sticky header CTA, sticky mobile CTA bar, repeated CTA banner, validated lead form
- UX polish: scroll progress, scroll-spy nav, back-to-top, dark/light theme, micro-interactions
- Accessibility and SEO: semantic landmarks, single h1, meta description, skip link, focus states, reduced-motion support

## Responsive
Mobile (up to 720px): hamburger menu, swipe carousel and tabs, sticky CTA bar. Tablet (721–1024px). Desktop (1000px+) with a two-column hero. Wide (1280px+).

## Browser support
Latest Chrome, Edge, Safari 15+, Firefox, Android and iOS browsers. Fallbacks for `color-mix()` and vendor prefixes for Safari.

## Run locally
Open `index.html` in a browser, or run `python3 -m http.server 8000` and visit http://localhost:8000.

## Known limitations
- The contact form validates on the client only; connect Formspree, Netlify Forms or a backend to receive submissions.
- Portfolio, logos, numbers and testimonials are placeholders.
