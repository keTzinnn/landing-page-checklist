# A form that prevents errors before submit

> **Category:** Conversion · **high impact**
> Flag required fields and expected formats before submit, so the visitor doesn't discover errors only when they try to send the form.
>
> 🇧🇷 [Versão em português](../../principios/conversao/prevencao-de-erro-formulario.md)

The visitor fills out a form, hits submit, and gets an error saying a field is required or the format is invalid. Frustrating. Worse still when the field was there all along but nothing flagged it as required or showed the format. A well-signaled form cuts that friction: required fields marked, expected format spelled out (e.g. 'DD/MM/YYYY' for dates, '11 digits' for phone), validation on blur where it matters. It's not red tape — it's respect for the visitor's time.

## Why it matters

- When a visitor hits a form error with no warning up front, they have to reread the field, figure out what went wrong, fix it, and try again. Each cycle eats attention and creates friction. Usability research shows that forms with clear visual cues (an asterisk or 'required' label, format examples) and real-time validation lower abandonment and raise completion. The 'validate everything on the server after the click' pattern is dated — immediate feedback is expected today.
- For conversion landing pages, every second counts. A visitor who abandons a form out of frustration doesn't come back. And missing cues breed distrust: 'why won't they say if it's required?' becomes 'are they harvesting my data?'. Clear signaling (and progressive validation) raises completion and conveys professionalism — the opposite of a generic form that punishes the visitor for guessing.
- Beyond the overall experience, required fields and format instructions should be bound semantically into the page structure — not just visually. A screen-reader or keyboard user needs to know a field is required before trying to fill it. When the page is well structured, those cues are available to any tool — it's foundation, not decoration.

## How to check your page

- [ ] Is every required field marked visually (asterisk, color, label) AND indicated semantically in the page structure?
- [ ] Does each required field have a clear label that explains what it expects (e.g. 'Email' vs. 'Email (name@example.com)')?
- [ ] Do fields with a specific format (tax ID, date, phone) show an example or mask that makes it clear (e.g. 'DD/MM/YYYY' or a placeholder like '(11) 9xxxx-xxxx')?
- [ ] Is there validation and feedback before submission (e.g. an empty field is highlighted on blur and shows a hint)?
- [ ] Do validated fields (email, tax ID, number) flag what's wrong without forcing a submit first?
- [ ] Are instruction messages (e.g. 'Numbers only') clearly tied to the visible field?
- [ ] Does the form have no 'hidden' required fields — is everything discoverable before trying to send?

## Common mistakes

- **Required field marked only visually** — An asterisk or color flags it as required, but with no matching semantic cue in the structure. Assistive-tech users never get the warning, and browsers can't trigger native validation.
- **Label disconnected from the field** — A text field and its label sit side by side visually, but with no clear structural association. Mobile and keyboard users have to click the exact field; the label doesn't extend the tap target or the access.
- **Expected format unclear** — A phone field with no example, no mask, no instruction. The visitor enters '+ 55 11 98765-4321' when the system wants '11987654321,' gets a generic error, and has no idea what to fix.
- **Validation only after submit** — The visitor types an email as 'user@' (no domain), hits submit, gets an error. With no real-time feedback, there's no chance to fix it before resubmitting the whole form.

## Sources

- Usability Heuristics for User Interface Design — Nielsen (Heuristic #5: Error Prevention and Recovery)
- Web Form Design — Luke Wroblewski (best practices for form labeling, validation, and user guidance)
- Web Content Accessibility Guidelines (WCAG) 2.1 — W3C (3.3.1 Error Identification, 3.3.2 Labels or Instructions)
- Form Field Research Report — Baymard Institute (impact of required-field indicators and labeling on form completion)

---

**Audit your page now →** [uxaudit.miaconecta.com.br](https://uxaudit.miaconecta.com.br?utm_source=github&utm_medium=isca&utm_campaign=checklist) · free: 2 audits

<sub>Part of **landing-page-checklist** · content under [CC BY-SA 4.0](../../LICENSE) · maintained by [UX Audit](https://uxaudit.miaconecta.com.br)</sub>
