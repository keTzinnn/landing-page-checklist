# Form fields with labels

> **Category:** Accessibility · **technical baseline**
> A field with no label, or an invisible one, confuses screen readers and anyone arriving with zoom or on mobile. A real accessibility test plus a checklist of mistakes.
>
> 🇧🇷 [Versão em português](../../principios/acessibilidade/labels-em-formularios.md)

A visitor on a zoomed-in phone — or using a screen reader — lands on an input field on your page. There's no visible label, just gray placeholder text that disappears the moment they start typing. They don't know what to enter. Keyboard navigators lose all context. A blind visitor hears 'text field' with no idea which one. The field technically exists, but it's useless. Accessible labels fix this: visible text, tied to the input via the 'for' attribute, and announceable by a screen reader.

## Why it matters

- Forms are the point of maximum friction on a landing page. The visitor has already decided to convert; now they have to fill it out. If the fields aren't clear, friction explodes: errors, abandonment, a lost lead. Visible labels cut errors and completion time — that's pure usability, not isolated accessibility. Luke Wroblewski and Steve Krug documented empirically that well-placed labels (above the field, not inside it) lift completion rates. And that holds for ALL visitors, blind or not.
- For blind and screen reader users, the stakes are higher: without an accessible label wired to the input, the reader can't announce what the field is. Keyboard navigation falls apart. And for anyone on zoom or a small phone, a placeholder isn't enough (it vanishes on typing and can get clipped). A persistent label is the universal standard.

## How to check your page

- [ ] Does every input field (text, email, phone, select) have a visible <label> element?
- [ ] Is the <label> tied to the <input> via a 'for' attribute matching the input's 'id' (or wrapping the input)?
- [ ] Is the label readable and does it describe the information expected ('Work email,' not just 'Email')?
- [ ] Does any field rely on placeholder or microcopy alone as the label — instead of permanent visible text, not a hover/onfocus state?
- [ ] Do required fields have a clear indicator (asterisk or 'required') that's both visible AND accessible?
- [ ] Do checkboxes and radio buttons have an accessible label, not just adjacent text with no technical link?

## Common mistakes

- **Placeholder as the only label** — The field has placeholder='Work email' but no visible label. The moment the visitor clicks in and starts typing, the placeholder is gone. The screen reader sees only 'text field,' with no context.
- **Label not tied to the input (broken semantics)** — There's 'Email' text near the input, but it's just a <span>, not a <label>. Clicking the label doesn't focus the field. The screen reader never connects the label to the input.
- **Invisible or near-invisible label** — The label exists in the HTML but it's display:none or color:#ccc on white. A screen reader can read it, but a sighted visitor sees a page that looks disorganized and directionless.
- **Required fields with no accessible marker** — A red asterisk signals 'required,' but there's no aria-required='true'. The screen reader never announces that the field is mandatory, causing errors and frustration on submit.

## Sources

- WCAG 2.1 — Labels or Instructions (W3C)
- Luke Wroblewski — Web Form Design (empirical behavior in forms)
- WebAIM — Form Accessibility
- Nielsen Norman Group — Form Design Best Practices

---

**Audit your page now →** [uxaudit.miaconecta.com.br](https://uxaudit.miaconecta.com.br?utm_source=github&utm_medium=isca&utm_campaign=checklist) · free: 2 audits

<sub>Part of **landing-page-checklist** · content under [CC BY-SA 4.0](../../LICENSE) · maintained by [UX Audit](https://uxaudit.miaconecta.com.br)</sub>
