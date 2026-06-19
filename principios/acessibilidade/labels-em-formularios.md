# Campos de formulário com rótulos

> **Categoria:** Acessibilidade · **base técnica**
> Campo sem label ou label invisível confunde leitores de tela e qualquer visitante que entra com zoom/mobile. Teste real de acessibilidade + checklist de erros.
>
> 🇺🇸 [English version](../../principles/accessibility/form-field-labels.md)

Um visitante em um celular ampliado — ou usando leitor de tela — chega a um campo de entrada na sua landing. Não há label visível, apenas placeholder cinzento que some quando digita. Ele não sabe o que digitar. Teclado navegador perde o contexto. Visitante cego ouve 'campo de texto' sem saber qual. O campo existe tecnicamente, mas é inútil. Labels acessíveis resolvem isso: texto visível, ligado ao input via atributo 'for', anunciável por leitura de tela.

## Por que importa

- Formulários são o momento de máxima fricção em uma landing page. Visitante já decidiu converter; agora tem de preencher. Se campos não são claros, a fricção explode: erro, abandono, perda de lead. Labels visíveis reduzem erros e tempo de conclusão — é usabilidade pura, não acessibilidade isolada. Luke Wroblewski e Steve Krug documentaram empiricamente que labels bem posicionados (acima do campo, não dentro) aumentam taxa de conclusão. E essa premissa vale para TODOS os visitantes, cegos ou não.
- Para usuários cegos/com leitor de tela, a situação é crítica: sem label acessível ligada ao input, o leitor não consegue anunciar qual é o campo. Navegação por teclado fica desmoralizada. Já para quem tem zoom ou está em celular pequeno, placeholder não é suficiente (some ao digitar, pode ser cortado). Label permanente é o padrão universal.

## Como verificar na sua página

- [ ] Todo campo de entrada (texto, email, phone, select) tem um elemento <label> visível?
- [ ] O <label> está ligado ao <input> via atributo 'for' que corresponde ao 'id' do input (ou wrapping o input)?
- [ ] O label é legível e descreve o tipo de informação esperada ('Email corporativo', não 'Email')?
- [ ] Nenhum campo usa apenas placeholder ou microcopy como label — texto visível permanente, não hover/onfocus?
- [ ] Campos obrigatórios têm indicação clara (asterisco ou 'obrigatório') tanto visível quanto acessível?
- [ ] Checkbox e radio buttons têm label acessível (não apenas um rótulo ao lado sem ligação técnica)?

## Erros comuns

- **Placeholder como único rótulo** — Campo tem placeholder='Email corporativo' mas sem label visível. Quando visitante clica e começa a digitar, o placeholder desaparece. Leitor de tela vê só 'campo de texto', sem contexto.
- **Label não ligado ao input (semântica quebrada)** — Há texto 'Email' perto do input, mas é apenas um <span>, não um <label>. Clique no label não foca o campo. Leitor de tela não conecta rótulo e entrada.
- **Rótulo invisível ou muito claro** — Label existe no HTML mas é display:none ou color:#ccc sobre branco. Leitor de tela consegue ler, mas visitante sighted vê a página desorganizada ou sem direção.
- **Campos obrigatórios sem marcação acessível** — Um asterisco vermelho indica 'obrigatório', mas não há aria-required='true'. Leitor de tela não anuncia que é obrigatório, causando erros e frustração na submissão.

## Fontes

- WCAG 2.1 — Labels or Instructions (W3C)
- Luke Wroblewski — Web Form Design (empiria de comportamento em formulários)
- WebAIM — Form Accessibility
- Nielsen Norman Group — Form Design Best Practices

---

**Audite a sua página agora →** [uxaudit.miaconecta.com.br](https://uxaudit.miaconecta.com.br?utm_source=github&utm_medium=isca&utm_campaign=checklist) · grátis: 2 auditorias

<sub>Parte de **landing-page-checklist** · conteúdo sob [CC BY-SA 4.0](../../LICENSE) · mantido por [UX Audit](https://uxaudit.miaconecta.com.br)</sub>
