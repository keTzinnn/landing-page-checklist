# Ferramenta de medição instalada

> **Categoria:** Conversão · **impacto alto**
> Pixel ou analytics não instalados deixam você escalando tráfego às cegas. O que é medição instalada, como verificar a sua página e por que é recomendação, não nota.
>
> 🇺🇸 [English version](../../principles/conversion/measurement-installed.md)

Uma landing page sem analytics configurado é como dirigir de olhos vendados. O visitante clica no botão, desaparece, e você fica sem saber se completou a ação, desistiu no formulário, ou se fechou a aba. Sem esse feedback, cada tentativa de melhorar a conversão é adivinhação — não iteração.

## Por que importa

- A medição é o fundamento de qualquer melhoria iterativa. Quando você não consegue medir o comportamento da página (cliques no CTA, preenchimento de formulário, navegação pós-conversão), qualquer decisão de design ou copy é um palpite. Testes A/B, estimativa de conversão, benchmark contra concorrentes — tudo exige baseline confiável.
- Escalar tráfego pago (Google Ads, Facebook, LinkedIn) sem analytics é queimar dinheiro sistematicamente. Plataformas de anúncio otimizam campanhas com base em eventos de conversão que você precisa reportar — clique no botão, submissão de formulário, page view pós-conversão. Sem pixel ou analytics, a plataforma não sabe o que otimizar e queima budget em tráfego que não converte.
- O feedback loop é quebrado: você não consegue distinguir entre um problema de design (visitante vê o CTA, mas não clica) e um problema de tráfego (visitante nunca chega ao CTA). Analytics estrutura essas perguntas — é o primeiro passo para diagnóstico honesto.

## Como verificar na sua página

- [ ] Você tem Google Analytics 4 (GA4), Google Tag Manager (GTM), Meta Pixel ou similar instalado e ativo na página?
- [ ] Eventos de conversão estão configurados (clique no CTA, submissão de formulário, page view pós-conversão)?
- [ ] Você consegue rastrear ao menos uma ação pós-clique (obrigado page, redirect, confirmação visual)?
- [ ] Os eventos de conversão aparecem no painel de analytics nos últimos 7 dias (prova de que estão acionando)?
- [ ] Você já comparou a contagem de conversões no analytics com os dados do CRM/e-mail/backend (verificar se os números batem)?
- [ ] Formulários têm campo oculto de source/medium para rastrear campanha de origem (ou UTM parameters funcionando)?
- [ ] Você tem goal/conversion setup rodando para ao menos o objetivo primário da página (lead, venda, trial)?

## Erros comuns

- **Sem pixel instalado** — Página com formulário, sem analytics. Dono pensa que está convertendo porque recebe e-mails. Depois descobre que a maioria abandona no formulário — mas nunca viu isso porque não mede clique-por-clique.
- **Pixel instalado, mas sem eventos** — GA4 está lá, mas só rastreia page views. Conversões não estão mapeadas para eventos. O dono vê volume, mas não consegue responder 'quantos clicaram no CTA'.
- **Medir sem validar** — Números no analytics não batem com registros no banco de dados. Divergência pode sair caro (falsa otimização baseada em métrica errada). Validação cruzada é essencial.
- **Pixel em ambiente de staging, não production** — Desenvolvedor instalou em dev/staging pra testar, mas nunca moveu pra live. Página está ao ar, analytics não está.

## Fontes

- Google Analytics 4 Documentation — Event Tracking and Goal Configuration (developers.google.com/analytics)
- Demand Curve — Landing Page Testing and Iteration (demandcurve.com)
- Nielsen Norman Group — Measuring Usability: Quantitative Studies (nngroup.com)
- Baymard Institute — E-commerce Tracking and Attribution (baymard.com)

---

**Audite a sua página agora →** [uxaudit.miaconecta.com.br](https://uxaudit.miaconecta.com.br?utm_source=github&utm_medium=isca&utm_campaign=checklist) · grátis: 2 auditorias

<sub>Parte de **landing-page-checklist** · conteúdo sob [CC BY-SA 4.0](../../LICENSE) · mantido por [UX Audit](https://uxaudit.miaconecta.com.br)</sub>
