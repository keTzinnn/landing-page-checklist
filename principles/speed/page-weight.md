# Lightweight page

> **Category:** Speed · **technical**
> Lighter pages load faster on slow connections. Trimming bytes from images, scripts, and CSS improves the experience, lowers bounce rate, and lifts conversion — especially on mobile.
>
> 🇧🇷 [Versão em português](../../principios/performance/peso-pagina.md)

A page's total size — measured in kilobytes — dictates how fast it loads. The lighter it is, the sooner it reaches your visitor. On mobile networks (3G/4G), every extra megabyte costs real seconds. A slow load pushes people to abandon before they ever see your offer — the heavier the page, the more likely you are to lose the visitors who showed up. This principle checks whether your page is optimized for weight: compressed images, unnecessary scripts stripped out, and lean CSS with no bloat.

## Why it matters

- Mobile connections are limited. A visitor on 3G is working with real-world bandwidth of about 1–2 Mbps. A 5 MB page takes 40 seconds to load — and nobody waits that long. Trim it to 1–2 MB and the experience becomes realistic (10–20 seconds), where fewer people bail. Desktop benefits less (faster connections), but still gains from lower latency.
- Google Core Web Vitals penalizes slow pages in organic search. Speed isn't just UX — it's a quality signal to search engines. A slow page ranks worse, draws less traffic, and converts less simply because fewer people arrive. The chain reaction is: less weight → faster load → better ranking → more traffic → more conversions.
- The psychology of waiting is non-linear. The first 3 seconds decide whether someone stays or leaves. Between 3 and 10 seconds, abandonment climbs exponentially. Under 3 seconds, visitors don't even notice the speed — they just browse. Optimizing weight is the most effective way to stay below that line.

## How to check your page

- [ ] Is the total page size (HTML, CSS, JS, images, fonts) ideally 1–2 MB — capped at 3 MB on desktop and 1.5 MB on mobile?
- [ ] Are images served in an optimized format (WebP with a PNG/JPEG fallback) and sized for each screen (not pushing a 2000px image to a 375px display)?
- [ ] Are scripts that aren't critical to the initial load deferred or loaded asynchronously (async/defer)?
- [ ] Is critical (above-the-fold) CSS inlined or split into a separate critical file, while non-critical CSS loads without blocking?
- [ ] Are web fonts limited to 2–3 weights/styles and loaded with preload or an optimized font-display to avoid layout shift?
- [ ] Have non-essential JavaScript libraries been removed or swapped for vanilla JS or lighter alternatives (e.g., Alpine instead of jQuery)?
- [ ] Is browser caching set up (appropriate Cache-Control headers) so returning visitors don't re-download everything?
- [ ] Does the page use transfer compression (gzip, Brotli) on the server?

## Common mistakes

- **High-res images with no optimization** — Serving 4K images to mobile devices. A single 3 MB photo can eat half your weight budget on its own. Fix: resize for the first screen, use WebP with a fallback, and lazy-load anything below the fold.
- **Unchecked tracking and third-party scripts** — Google Tag Manager, Intercom, Hotjar, CRM widgets, ad pixels — each one adds 100–500 KB. Stack a few tools and it adds up fast. Fix: audit and remove what isn't essential, and delay non-critical scripts until after conversion.
- **Unminified or duplicated CSS and JS** — A style.css with 200 KB of unminified code. A bundle.js shipping two copies of Bootstrap. Fix: minify, drop duplicates, and use tree-shaking in your bundler.
- **Web fonts loaded with no limits** — Ten variations of one font (Light, Regular, Bold, Black, plus italics) all downloading at once. Fix: limit it to 2–3 critical weights and fall back to system fonts.
- **No image lazy-loading** — Every image loads on the first request — even the ones 2000px below the fold. Fix: use loading='lazy' or an Intersection Observer to defer images outside the first screen.

## Sources

- Google Web Vitals: Largest Contentful Paint (LCP) and page load optimization (developers.google.com/web/vitals)
- Nielsen Norman Group: Website Response Time and User Satisfaction (research on how load time affects bounce rate and engagement)
- Baymard Institute: Impact of load time on e-commerce conversion
- Julian Shapiro: Web Performance Best Practices (performance budgets, image optimization, and lazy-loading strategies)

---

**Audit your page now →** [uxaudit.miaconecta.com.br](https://uxaudit.miaconecta.com.br?utm_source=github&utm_medium=isca&utm_campaign=checklist) · free: 2 audits

<sub>Part of **landing-page-checklist** · content under [CC BY-SA 4.0](../../LICENSE) · maintained by [UX Audit](https://uxaudit.miaconecta.com.br)</sub>
