# Navegável por teclado

> **Categoria:** Acessibilidade · **base técnica**
> Visitantes que usam teclado (por deficiência, preferência ou contexto) ficam presos se sua página não é navegável. Como auditar e consertar.
>
> 🇺🇸 [English version](../../principles/accessibility/keyboard-navigation.md)

Três cenários: um visitante com lesão motora usa teclado como seu único meio de interação. Outro, experiente, prefere Tab + Enter por velocidade. Um terceiro está em um celular antigo com teclado físico reduzido. Todos dependem de navegação por teclado funcional. Sua landing é hermética? Muitos sites modernos — especialmente em SPA/React mal configurado — fazem foco desaparecer, Tab pula elementos, Enter não ativa botões, e dropdown (com select ou combobox) é inacessível sem mouse. O visitante sai. WCAG AA exige que elementos interativos sejam alcançáveis por teclado e que foco seja sempre visível.

## Por que importa

- Acessibilidade por teclado é requisito de inclusão legítima. Pessoas com paralisia, tremor, amputação ou problemas motores navegam exclusivamente por teclado. Além delas, profissionais e power users preferem teclado por velocidade e eficiência. Excluir teclado é perda de receita direta e uma barreira para parcela significativa da população.
- Além da inclusão, teclado é prerrogativa de qualidade de code: sites bem arquitetados (sem armadilhas de foco, com semântica HTML clara) são navegáveis por teclado por padrão. A maioria das frameworks modernas (React, Vue, Next.js) fornece ferramentas para fazer isso fácil; se não funciona, é negligência. Visitantes que detectam foco invisível ou Tab preso percebem a página como amadora. Nielsen, em estudos de heurísticas de usabilidade, destaca controle do usuário e liberdade de navegação como critério essencial — teclado é parte disso.

## Como verificar na sua página

- [ ] Começando na página, Tab consegue alcançar TODOS os elementos interativos (botões, links, inputs, dropdowns)?
- [ ] Nenhum elemento fica 'preso' — Tab nunca circula infinitamente ou salta elementos sem lógica?
- [ ] O foco é VISÍVEL — há um outline/border claro ao redor do elemento focado (não outline:none sem substituto)?
- [ ] Enter (ou Space) ativa botões; Enter submete formulário; Tab avança em inputs? Teclas funcionam como esperado?
- [ ] Dropdowns/selects são navegáveis por teclado (Arrow Up/Down para itens, Enter para selecionar)?
- [ ] Modals/lightbox têm trap de foco (Tab não sai para fundo enquanto modal está aberta)?

## Erros comuns

- **outline:none sem substituto** — Designer remove o outline padrão (outline:none) por achar 'feio', mas não implementa foco customizado. Teclado usuário não vê para onde foi o foco. Navegar fica impossível.
- **Elemento interativo não é tabulável (div clicável)** — Um botão customizado é um <div> com onclick, não um <button>. Tab não alcança; Enter não ativa. Acessível apenas para mouse.
- **Ordem de Tab não faz sentido visual** — Tab salta de um ponto da página para outro aleatoriamente (bug de z-index/posição absoluta, ou tabindex mal configurado). Usuário fica desorientado.
- **Dropdown ou menu aberto fica visível mas não navegável** — Um menu dropdown abre ao clicar, mas Arrow Keys não navegam itens. Teclado usuário vê o menu mas não consegue usar; volta ao mouse (que pode não ter).

## Fontes

- WCAG 2.1 — Keyboard Accessible (W3C)
- WebAIM — Keyboard Accessibility
- Deque Systems — Keyboard Navigation Best Practices
- Nielsen Norman Group — Keyboard Navigation & Accessibility

---

**Audite a sua página agora →** [uxaudit.miaconecta.com.br](https://uxaudit.miaconecta.com.br?utm_source=github&utm_medium=isca&utm_campaign=checklist) · grátis: 2 auditorias

<sub>Parte de **landing-page-checklist** · conteúdo sob [CC BY-SA 4.0](../../LICENSE) · mantido por [UX Audit](https://uxaudit.miaconecta.com.br)</sub>
