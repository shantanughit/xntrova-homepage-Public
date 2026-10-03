# Submission – Web Developer Homepage Redesign (Xntrova Technologies)

**Candidate:** <your name>
**GitHub repository:** <paste repo URL>
**Live URL:** <paste Netlify URL>

## Stack
Plain HTML, CSS and vanilla JavaScript. No framework and no build step, so the page is fast and easy to maintain. Only external resource: Google Fonts (Plus Jakarta Sans, with system-font fallback).

## Major changes and why
| Area | Change | Reason |
|---|---|---|
| Positioning | B2B-first hero with rotating headline and two clear CTAs | Communicates the value proposition and conversion path immediately |
| Trust | Logo marquee, results band with counters, testimonials | Builds credibility early, before the visitor reaches the form |
| Services | Bento grid with one featured service | Easier to scan than a flat list; visual hierarchy |
| Portfolio | Filter tabs and hover case-study overlay | Lets visitors self-select relevant work |
| Objections | FAQ accordion | Removes friction (timeline, pricing, contract) before contact |
| Conversion | Sticky header CTA, sticky mobile CTA bar, repeated CTA banner, short validated form | Multiple low-friction entry points |
| UX polish | Scroll progress, scroll-spy nav, back-to-top, dark/light theme, micro-interactions | Better orientation and a premium feel |
| Accessibility | Semantic landmarks, single h1, skip link, focus states, aria on menu/accordion, reduced-motion support | Inclusive and SEO-friendly |

## Responsive approach
Mobile-friendly CSS with relative units, flexbox and grid. Breakpoints: ≤720px mobile (hamburger menu, swipe carousel and tabs, sticky CTA), 721–1024px tablet, ≥1000px desktop (two-column hero), ≥1280px wide. Safe-area insets handle notched phones; hover effects are disabled on touch devices.

## Performance
- No JS or CSS libraries, no images (visuals are CSS and emoji), so the payload is small
- `font-display: swap`, deferred JS, long-lived cache headers (netlify.toml)
- IntersectionObserver for animations instead of scroll listeners (with fallback)
- Animations use transform/opacity only

## Cross-browser
Fallbacks for `color-mix()`, `-webkit-` prefixes for backdrop-filter and masks, IntersectionObserver fallback. Targets latest Chrome, Edge, Safari 15+, Firefox, Android and iOS browsers.

## Code structure
- `css/style.css`: design tokens on `:root` (light and dark), then layout, reusable components (`.btn`, `.card`, `.eyebrow`, `.grid`), and responsive sections
- `js/main.js`: small independent modules (menu, reveal and counters, filter, scroll-spy, theme, form)

## Known limitations / next steps
- Contact form validates on the client only. Next step: Formspree/Netlify Forms or a backend endpoint
- Portfolio, logos, numbers and testimonials are placeholders; they should be replaced with real client content
- Add real project images (WebP, lazy-loaded) and an Open Graph image

## Be ready to explain in the discussion
Why vanilla JS over React for a single landing page, how the scroll-spy and counters work (IntersectionObserver), how the form validation flow works, and how the responsive breakpoints were chosen.
