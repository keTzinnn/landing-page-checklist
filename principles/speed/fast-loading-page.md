# Fast-loading page

> **Category:** Speed · **technical**
> The page loads fast. A slow page scares visitors away before they ever convert.
>
> 🇧🇷 [Versão em português](../../principios/performance/tempo-carregamento.md)

A visitor landing on your page decides whether to stay or leave within seconds. If the page isn't responsive during that critical window, they're gone — no matter how good the content is. Slow load times are invisible only to the person measuring their own home broadband. For everyone else — on mobile or any less-than-perfect network — it's a concrete barrier.

## Why it matters

- Perceived speed drives trust. A page that's slow to respond reads as careless, whatever the technical reason. Visitors don't distinguish between an overloaded server, unoptimized images, or blocking JavaScript — they just feel the delay. And their response is simple: close the tab.
- In conversion contexts (e-commerce, SaaS, lead gen), load time is a measurable driver of abandonment. A page that's responsive from the very first bytes signals professionalism and trust — and those land before any promise your copy or visual design can make.
- Speed doesn't care what device the visitor is on: they don't control their 4G, satellite, or public Wi-Fi connection. Optimizing for real-world conditions, not just ideal ones, is how you show the visitor matters more than the number on your laptop.

## How to check your page

- [ ] Does the page respond to interaction within 1 second?
- [ ] Are the key elements (CTA button, form, hero image) visible without scrolling in under 2.5 seconds?
- [ ] Is the total number of network requests (images, CSS, JavaScript) under 100?
- [ ] Is the page's total byte size within reasonable limits for a 4G mobile connection?
- [ ] Are any third-party scripts (analytics, chat, ads) blocking the main page from loading?

## Common mistakes

- **Confusing first paint with interactivity** — A page can show content fast but stay sluggish to respond to clicks and input. A page that shows the form in 1 second but takes 5 to accept input still loses the conversion.
- **Optimizing for desktop only** — Local tests on broadband hide the real problem. Most visitors arrive on mobile — a page that feels snappy on desktop can be unusable on a real 4G connection.
- **Blaming the visitor's connection** — Shutting out visitors on slow connections or making them wait isn't acceptable on a landing page — it's signing off on predictable abandonment. Optimizing for real-world connections is part of the job.

## Sources

- Google Web Vitals — the core page performance metrics: LCP, FID, CLS. https://web.dev/vitals
- Nielsen Norman Group. 'Website Response Times' — the classic research on perceived usability and page speed. https://www.nngroup.com
- Lighthouse — Google's performance auditing tool, with documentation on optimization and metrics. https://developers.google.com/web/tools/lighthouse
- Steve Krug. 'Don't Make Me Think: A Common Sense Approach to Web Usability' (usability and perceived speed).

---

**Audit your page now →** [uxaudit.miaconecta.com.br](https://uxaudit.miaconecta.com.br?utm_source=github&utm_medium=isca&utm_campaign=checklist) · free: 2 audits

<sub>Part of **landing-page-checklist** · content under [CC BY-SA 4.0](../../LICENSE) · maintained by [UX Audit](https://uxaudit.miaconecta.com.br)</sub>
