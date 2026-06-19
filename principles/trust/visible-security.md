# Security cues where you ask for data

> **Category:** Trust · **medium impact**
> Visitors hesitate to fill out a form with no sign of security. How to show HTTPS and a privacy policy.
>
> 🇧🇷 [Versão em português](../../principios/confianca/seguranca-visivel.md)

When someone is asked to fill out a form and hand over their email or phone, the first thought is: 'is my data safe here?'. Without obvious security cues — an HTTPS URL, a padlock icon, a note about privacy — distrust grows. This principle is about signaling security right at the point where you collect data, and how to audit those cues.

## Why it matters

- HTTPS is the baseline for any landing page with a form. Modern browsers flag HTTP as 'not secure' — the visitor sees the warning and hesitates. HTTPS is necessary but not sufficient: many visitors never look at the address bar. That's why it pays to signal security near the form: 'Your data is protected with SSL/TLS', with a padlock icon.
- Per the Nielsen Norman Group, security icons (padlock, seal) lower objection when placed near the input fields. It doesn't need to be an external seal; something simple works: 'Secure transmission via SSL', with an icon. The visitor sees it and feels a bit safer.
- The privacy policy is critical. Brazil's LGPD and the EU's GDPR require explicit consent. A single line near the submit button — 'By submitting, you agree to our [privacy policy]', with a clickable link — is essential. Without it, you're not only non-compliant; you also lower trust, because the visitor doesn't know where their data is going.

## How to check your page

- [ ] Is the page served over HTTPS (not HTTP)?
- [ ] Is there a padlock icon or security note visible near the form (e.g., 'Data protected with SSL')?
- [ ] Does the form include a clear consent/privacy line before the submit button?
- [ ] Is the 'privacy policy' link clickable and pointing to a readable document (not broken)?
- [ ] If a third party is involved (Stripe, Zapier, email), is there a note ('your data is processed by...')?
- [ ] Do sensitive fields (phone, national ID) have microcopy explaining why they're needed?

## Common mistakes

- **HTTPS but no visible cue** — A form on HTTPS with no security icon or note near the field leaves the visitor unsure it's safe. Add a small padlock icon or a line like 'Your transmission is protected.'
- **Broken privacy link** — A privacy policy link that's broken or leads to a blank page is worse than no link. The visitor clicks, sees an error, and trust drops. Make sure it works and leads to a real document.
- **No consent before submit** — No mention of data consent before the submit button breaks LGPD/GDPR and raises suspicion. Add: 'By submitting, you agree to receive updates and accept our [policy].'
- **Security note too faint** — A security note in tiny type or washed-out color has zero effect. Use legible body size (12–14px) and a contrasting color (green for security, blue for the link).

## Sources

- OWASP — HTTPS Best Practices
- Nielsen Norman Group — Trust in Web Design (visible security)
- CXL Institute — Form Design & Conversion (trust in forms)
- W3C/WCAG — Accessibility & Trust Standards

---

**Audit your page now →** [uxaudit.miaconecta.com.br](https://uxaudit.miaconecta.com.br?utm_source=github&utm_medium=isca&utm_campaign=checklist) · free: 2 audits

<sub>Part of **landing-page-checklist** · content under [CC BY-SA 4.0](../../LICENSE) · maintained by [UX Audit](https://uxaudit.miaconecta.com.br)</sub>
