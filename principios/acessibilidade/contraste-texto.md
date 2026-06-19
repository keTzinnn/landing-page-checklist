# Contraste de texto adequado

> **Categoria:** Acessibilidade · **base técnica**
> Texto com baixo contraste afasta leitores e visitantes com baixa visão. Como medir, por que importa e os erros que mais custam conversão.
>
> 🇺🇸 [English version](../../principles/accessibility/text-contrast.md)

Uma landing page precisa de muitos visitantes para escalar conversão. Mas se o texto não contrasta bem com o fundo, parte desses visitantes sai imediatamente — especialmente quem tem baixa visão, daltonismo ou está ao sol em um celular. Contraste inadequado não é detalhe de acessibilidade; é perda de receita. O padrão WCAG AA (relação de contraste 4.5:1 para texto normal, 3:1 para texto grande) não é capricho técnico: é o mínimo para que uma página seja legível por praticamente qualquer visitante.

## Por que importa

- A legibilidade é pré-requisito da conversão. Se o visitante não consegue ler a headline ou a cópia do CTA, ele não converte — nem por falta de interesse, mas por incapacidade física. Texto com baixo contraste reduz a velocidade de leitura e aumenta o cansaço ocular, expulsando visitantes antes do engajamento. Nielsen, em suas 10 Heurísticas, flagra que legibilidade e clareza visual são princípios críticos de usabilidade, impactando taxa de permanência e confiança.
- Além do aspecto de inclusão, o contraste afeta a percepção de qualidade: uma página com texto que custa ler parece amadora ou descuidada, prejudicando a confiança. Sites de alta conversão (SaaS, e-commerce, lead capture) investem em hierarquia tipográfica clara, incluindo contraste robusto, porque sabem que legibilidade é conversão. O inverso também é verdadeiro: contraste fraco é sinônimo de falta de atenção ao detalhe.

## Como verificar na sua página

- [ ] Todo texto do corpo tem contraste de pelo menos 4.5:1 contra o fundo (WCAG AA)?
- [ ] Headings e texto grande (18pt+) atendem o mínimo de 3:1?
- [ ] O CTA e copy de ação crítica (promise, objeção, segurança) foram testados em contraste?
- [ ] Nenhum texto importante foi combinado com fundo de imagem/gradiente que cai em contraste abaixo do alvo?
- [ ] A página foi verificada em modo claro E escuro (se suporta tema) para manter contraste?
- [ ] Você testou a legibilidade em um celular sob luz solar simulada ou real?

## Erros comuns

- **Texto cinza-claro sobre branco** — Combinação clássica que parece elegante no design, mas é ilegível. A maioria dos visitantes com qualquer deficiência visual sai da página no primeiro clique.
- **Texto sobre fundo de imagem sem overlay** — A imagem de hero/background é linda, mas o contraste do texto contra ela varia e cai abaixo de 4.5:1 em várias áreas. O visitante só consegue ler a headline em partes.
- **Labels de formulário em contraste fraco** — Os campos têm labels visualmente bonitos mas muito claros. Usuários com qualquer dificuldade visual erram ao preencher ou desistem.
- **Foco/hover sem contraste diferenciado** — Botões e links mudam apenas de cor ao passar o mouse, não de contraste — teclado usuários e leitores de tela não veem a mudança de estado.

## Fontes

- WCAG 2.1 — Web Content Accessibility Guidelines, nível AA (W3C)
- Nielsen Norman Group — Contrast and Color Accessibility
- Steve Krug — Don't Make Me Think (legibilidade como usabilidade)
- Google Web Vitals — Visual Stability & Readability

---

**Audite a sua página agora →** [uxaudit.miaconecta.com.br](https://uxaudit.miaconecta.com.br?utm_source=github&utm_medium=isca&utm_campaign=checklist) · grátis: 2 auditorias

<sub>Parte de **landing-page-checklist** · conteúdo sob [CC BY-SA 4.0](../../LICENSE) · mantido por [UX Audit](https://uxaudit.miaconecta.com.br)</sub>
