# Images with alt text

> **Category:** Accessibility · **technical baseline**
> Images without alt text lose blind visitors and hurt your SEO. How to spot which images need alt text and dodge the usual mistakes.
>
> 🇧🇷 [Versão em português](../../principios/acessibilidade/alt-em-imagens.md)

Your landing page has a hero shot of a smiling executive holding the product, a growth chart, and a few dashboard screenshots. A blind visitor, or anyone running a screen reader, hears: 'image,' 'image,' 'image.' They have no idea what they're looking at, and the page's whole visual promise vanishes. Alt text (the alt attribute) is the bridge between what's shown and the people who can't see it — and it's no minor detail: it's lost conversions and a WCAG compliance gap.

## Why it matters

- Images carry the value proposition on most landing pages. A chart screaming '300% growth' or a screenshot of the product in action builds trust and tangibility far faster than text ever could. But if an image has no alt text, or a useless one ('image123.jpg' or 'screenshot'), visitors on screen readers never get that value. The loss is twofold: accessibility and persuasive context. People who rely on screen readers make up a meaningful slice of the population, and even more have low vision and depend on zoom plus text-based navigation.
- Alt text also moves SEO. Search engines don't 'see' images; they read the alt attribute to understand context. An image of your product with no alt text is invisible for ranking; with a descriptive alt, it boosts relevance. You win on both fronts at once: accessibility AND search visibility.

## How to check your page

- [ ] Does every informative image have an alt attribute that isn't empty or generic?
- [ ] Does the alt describe the MEANING of the image, not just that it exists ('chart showing 300% growth in Q3' vs. 'chart')?
- [ ] Do purely decorative images have an empty alt (alt='') so they aren't announced?
- [ ] Do screenshots and charts have alt text that sums up the key information they convey?
- [ ] Do functional icons (like a scroll arrow) have alt text that explains the action?
- [ ] Do client logos (social proof) carry the company name in the alt, or an empty alt if they're purely decorative?

## Common mistakes

- **Generic or auto-generated alt** — alt='image.jpg' or alt='screenshot 1' helps no one. The screen reader just reads the file name with zero context. A blind visitor can't tell whether it's the hero, a chart, or an icon.
- **Alt that runs on into a paragraph** — alt='This is a chart showing how tool X increased user time by 300% in the third quarter of 2025, based on data from 5,000 customers' is noise. Keep alt text tight — 100 to 125 characters at most.
- **Decorative icon with needless descriptive alt** — A decorative icon next to the headline gets alt='purple rocket icon with flames.' The screen reader announces it for no reason. Pure ornament should use alt='' so it's skipped.
- **Interactive icon with no alt or broken semantics** — A hamburger icon that opens the menu has no alt, or it has alt='menu' with no visible label. Keyboard users can't tell what it does, and the link isn't semantically wired up.

## Sources

- WCAG 2.1 — Non-text Content (W3C)
- WebAIM — Alternative Text for Images
- Baymard Institute — E-commerce Product Image & Text Quality

---

**Audit your page now →** [uxaudit.miaconecta.com.br](https://uxaudit.miaconecta.com.br?utm_source=github&utm_medium=isca&utm_campaign=checklist) · free: 2 audits

<sub>Part of **landing-page-checklist** · content under [CC BY-SA 4.0](../../LICENSE) · maintained by [UX Audit](https://uxaudit.miaconecta.com.br)</sub>
