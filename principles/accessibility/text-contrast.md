# Adequate text contrast

> **Category:** Accessibility · **technical baseline**
> Low-contrast text pushes away readers and low-vision visitors. How to measure it, why it matters, and the mistakes that cost the most conversions.
>
> 🇧🇷 [Versão em português](../../principios/acessibilidade/contraste-texto.md)

A landing page needs plenty of visitors to scale conversions. But if the text doesn't stand out clearly against the background, you lose a chunk of them on arrival — especially anyone with low vision, color blindness, or a phone screen in direct sunlight. Poor contrast isn't an accessibility footnote; it's lost revenue. The WCAG AA standard (a 4.5:1 contrast ratio for body text, 3:1 for large text) isn't technical fussiness: it's the floor for a page to be readable by virtually any visitor.

## Why it matters

- Readability is the prerequisite for conversion. If a visitor can't read the headline or the CTA copy, they don't convert — not for lack of interest, but for a physical inability to. Low-contrast text slows reading and strains the eyes, driving visitors off before they ever engage. Nielsen's 10 Heuristics flag legibility and visual clarity as critical usability principles that shape dwell time and trust.
- Beyond inclusion, contrast shapes perceived quality. A page with text that's a chore to read looks amateurish or careless, and that erodes trust. High-converting sites — SaaS, e-commerce, lead capture — invest in clear typographic hierarchy, robust contrast included, because they know legibility is conversion. The reverse holds too: weak contrast signals a lack of attention to detail.

## How to check your page

- [ ] Does all body text hit at least 4.5:1 contrast against its background (WCAG AA)?
- [ ] Do headings and large text (18pt and up) meet the 3:1 minimum?
- [ ] Have you tested contrast on the CTA and critical action copy (promise, objection handling, trust)?
- [ ] Has any important text been placed over an image or gradient where contrast drops below the target?
- [ ] Have you checked the page in both light AND dark mode (if you support themes) to keep contrast intact?
- [ ] Have you tested legibility on a phone under real or simulated sunlight?

## Common mistakes

- **Light-gray text on white** — The classic combo that looks elegant in the mockup but is unreadable in practice. Most visitors with any visual impairment bounce on the first click.
- **Text over an image with no overlay** — The hero or background image is gorgeous, but the text's contrast against it shifts and falls below 4.5:1 in spots. The visitor can only read the headline in patches.
- **Form labels with weak contrast** — The fields have visually pretty labels that are far too light. Visitors with any visual difficulty mis-fill the form or give up.
- **Focus and hover states with no contrast shift** — Buttons and links only change color on hover, not contrast — keyboard users and screen reader users never register the state change.

## Sources

- WCAG 2.1 — Web Content Accessibility Guidelines, level AA (W3C)
- Nielsen Norman Group — Contrast and Color Accessibility
- Steve Krug — Don't Make Me Think (legibility as usability)
- Core Web Vitals — Visual Stability & Readability

---

**Audit your page now →** [uxaudit.miaconecta.com.br](https://uxaudit.miaconecta.com.br?utm_source=github&utm_medium=isca&utm_campaign=checklist) · free: 2 audits

<sub>Part of **landing-page-checklist** · content under [CC BY-SA 4.0](../../LICENSE) · maintained by [UX Audit](https://uxaudit.miaconecta.com.br)</sub>
