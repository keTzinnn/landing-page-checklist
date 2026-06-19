# Segurança sinalizada onde pede dados

> **Categoria:** Confiança · **impacto médio**
> Visitante hesita em preencher formulário sem sinal de segurança. Como mostrar HTTPS e política de privacidade.
>
> 🇺🇸 [English version](../../principles/trust/visible-security.md)

Quando alguém é pedido para preencher formulário e compartilhar email ou telefone, o primeiro pensamento é: 'meus dados são seguros aqui?'. Sem sinais óbvios de segurança — URL com HTTPS, ícone de cadeado, aviso sobre privacidade — a desconfiança cresce. Este princípio aborda como sinalizar segurança perto do ponto de entrada de dados e como auditar esses sinais.

## Por que importa

- HTTPS é requisito básico para landing pages com formulário. Browsers modernos marcam HTTP como 'não seguro' — visitante vê aviso e desconfia. Ter HTTPS é necessário, mas não suficiente: muitos visitantes não notam a barra de endereço. Por isso, recomenda-se sinalizar próximo ao formulário: 'Seus dados são protegidos por SSL/TLS' com um ícone de cadeado.
- Segundo Nielsen Norman Group, ícones de segurança (cadeado, selo) reduzem objeção quando posicionados perto do campo de entrada. Não precisa ser selo externo; pode ser simples: 'Transmissão segura via SSL' com ícone. Visitante vê isso e sente-se um pouco mais seguro.
- Política de privacidade é crítica. LGPD (Brasil) e GDPR (UE) exigem consentimento explícito. Uma linha perto do submit — 'Ao enviar, você concorda com nossa [política de privacidade]' com link clicável — é essencial. Sem isso, não só é ilegal; também reduz confiança porque visitante não sabe para onde seus dados vão.

## Como verificar na sua página

- [ ] A página é servida em HTTPS (não HTTP)?
- [ ] Há um ícone de cadeado ou aviso de segurança visível perto do formulário (ex.: 'Dados protegidos por SSL')?
- [ ] O formulário inclui uma linha de consentimento/privacidade clara antes do botão de submit?
- [ ] O link de 'política de privacidade' é clicável e leva a um documento legível (não quebrado)?
- [ ] Se há integração com terceiro (Stripe, Zapier, email), há aviso ('seus dados são processados por...')?
- [ ] Campos sensíveis (telefone, CPF) têm microcopy explicando por que são pedidos?

## Erros comuns

- **Formulário em HTTPS, mas sem nenhum ícone/aviso visível de segurança perto do campo** — Visitante não sabe automaticamente que é seguro. Adicione ícone de cadeado pequeno ou texto 'Sua transmissão é protegida'.
- **Link de política de privacidade quebrado ou em página vazia** — Pior que não ter link. Visitante clica, vê erro ou página vazia, confiança cai. Garanta que funciona e leva a documento real.
- **Nenhuma menção de consentimento de dados antes do submit** — Violação de LGPD/GDPR. Além disso, aumenta suspeita. Adicione: 'Ao enviar, você concorda em receber atualizações e aceita nossa [política]'.
- **Aviso de segurança em corpo minúsculo ou cores apagadas** — Se está ali mas invisível, tem efeito zero. Use corpo legível (12-14px) e cor contrastada (verde para segurança, azul para link).

## Fontes

- OWASP — HTTPS Best Practices
- Nielsen Norman Group — Trust in Web Design (segurança visível)
- CXL Institute — Form Design & Conversion (confiança em formulários)
- W3C/WCAG — Accessibility & Trust Standards

---

**Audite a sua página agora →** [uxaudit.miaconecta.com.br](https://uxaudit.miaconecta.com.br?utm_source=github&utm_medium=isca&utm_campaign=checklist) · grátis: 2 auditorias

<sub>Parte de **landing-page-checklist** · conteúdo sob [CC BY-SA 4.0](../../LICENSE) · mantido por [UX Audit](https://uxaudit.miaconecta.com.br)</sub>
