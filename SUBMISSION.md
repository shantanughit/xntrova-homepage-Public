# Submission – Web Developer Homepage Redesign (Xntrova Technologies)

**GitHub repository:** https://github.com/shantanughit/xntrova-homepage-Public
**Live URL:** https://xntrova-homepage.netlify.app/

## Stack
HTML, CSS and vanilla JavaScript. No framework or build step, so the page is fast and easy to maintain.

## Major changes and why
| Area | Change | Reason |
|---|---|---|
| Positioning | B2B-first hero, rotating headline, two CTAs | Value proposition and next step visible immediately |
| Trust | Logo marquee, results counters, testimonials | Credibility before the visitor reaches the form |
| Services | Bento grid with a featured service | Easier to scan, clearer hierarchy |
| Portfolio | Filter tabs and hover case-study overlay | Visitors self-select relevant work |
| Objections | FAQ accordion | Removes friction before contact |
| Conversion | Sticky header CTA, sticky mobile CTA bar, CTA banner, short validated form | Multiple low-friction entry points |
| UX polish | Scroll progress, scroll-spy, back-to-top, dark/light theme | Orientation and a premium feel |
| Accessibility | Landmarks, single h1, skip link, focus states, ARIA, reduced motion | Inclusive and SEO-friendly |

## Responsive approach
Relative units, flexbox and grid. Breakpoints: up to 720px mobile, 721–1024px tablet, 1000px+ desktop, 1280px+ wide. Safe-area insets for notched phones; hover effects disabled on touch devices.

## Performance
No libraries, no images to load, deferred font loading (`font-display: swap`), transform/opacity-only animations, IntersectionObserver instead of scroll listeners.

## Code structure
CSS uses design tokens on `:root` (light and dark) followed by layout, reusable components (`.btn`, `.card`, `.eyebrow`, `.grid`) and responsive rules. JavaScript is split into small independent blocks: menu, reveal and counters, portfolio filter, scroll-spy, theme toggle, form validation.

## Known limitations / next steps
- Form validates on the client only; next step is Formspree/Netlify Forms or a backend endpoint.
- Portfolio, logos and testimonials are placeholders to be replaced with real client content.
- Add real project images (WebP, lazy-loaded) and an Open Graph image.

