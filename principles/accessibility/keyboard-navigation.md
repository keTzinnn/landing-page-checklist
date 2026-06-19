# Keyboard navigable

> **Category:** Accessibility · **technical baseline**
> Visitors who use a keyboard (by disability, preference, or context) get trapped if your page isn't navigable. How to audit it and fix it.
>
> 🇧🇷 [Versão em português](../../principios/acessibilidade/navegacao-teclado.md)

Three scenarios: a visitor with a motor impairment uses the keyboard as their only way to interact. Another, an experienced user, prefers Tab + Enter for speed. A third is on an old phone with a cramped physical keyboard. All of them depend on keyboard navigation that actually works. Is your page sealed shut to them? Plenty of modern sites — especially a poorly configured SPA or React app — make focus vanish, let Tab skip elements, fail to fire buttons on Enter, and leave dropdowns unreachable without a mouse. The visitor leaves. WCAG AA requires interactive elements to be reachable by keyboard and focus to always be visible.

## Why it matters

- Keyboard accessibility is a legitimate inclusion requirement. People with paralysis, tremors, amputation, or other motor conditions navigate by keyboard alone. And beyond them, professionals and power users choose the keyboard for speed and efficiency. Shutting out the keyboard is direct lost revenue and a barrier for a meaningful slice of the population.
- Beyond inclusion, keyboard support is a hallmark of clean code: well-architected sites (no focus traps, clear HTML semantics) are keyboard-navigable by default. Most modern frameworks (React, Vue, Next.js) make this easy; when it doesn't work, that's negligence. Visitors who hit invisible focus or a stuck Tab read the page as amateur work. Nielsen's usability heuristics call out user control and freedom of navigation as essential — and keyboard support is part of that.

## How to check your page

- [ ] Starting from the top, can Tab reach EVERY interactive element (buttons, links, inputs, dropdowns)?
- [ ] Does no element get 'stuck' — does Tab never loop endlessly or skip elements illogically?
- [ ] Is focus VISIBLE — a clear outline or border around the focused element (not outline:none with no replacement)?
- [ ] Does Enter (or Space) fire buttons, Enter submit forms, and Tab advance through inputs? Do the keys behave as expected?
- [ ] Are dropdowns and selects keyboard-navigable (Arrow Up/Down to move, Enter to select)?
- [ ] Do modals and lightboxes trap focus (Tab can't escape to the background while the modal is open)?

## Common mistakes

- **outline:none with no replacement** — The designer kills the default outline (outline:none) for looking 'ugly' but never builds a custom focus style. Keyboard users can't see where focus went. Navigation becomes impossible.
- **Interactive element isn't tabbable (clickable div)** — A custom button is a <div> with onclick, not a <button>. Tab can't reach it; Enter won't fire it. It's only usable with a mouse.
- **Tab order doesn't match the visual layout** — Tab jumps from one spot on the page to another at random (a z-index or absolute-positioning bug, or a misconfigured tabindex). The user gets disoriented.
- **Open dropdown or menu is visible but not navigable** — A dropdown opens on click, but the arrow keys don't move through the items. Keyboard users see the menu but can't use it; they're forced back to the mouse they may not have.

## Sources

- WCAG 2.1 — Keyboard Accessible (W3C)
- WebAIM — Keyboard Accessibility
- Deque Systems — Keyboard Navigation Best Practices
- Nielsen Norman Group — Keyboard Navigation & Accessibility

---

**Audit your page now →** [uxaudit.miaconecta.com.br](https://uxaudit.miaconecta.com.br?utm_source=github&utm_medium=isca&utm_campaign=checklist) · free: 2 audits

<sub>Part of **landing-page-checklist** · content under [CC BY-SA 4.0](../../LICENSE) · maintained by [UX Audit](https://uxaudit.miaconecta.com.br)</sub>
