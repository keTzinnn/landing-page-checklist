# Imagens com texto alternativo

> **Categoria:** Acessibilidade · **base técnica**
> Imagens sem alt perdem visitantes cegos e machucam SEO. Como identificar qual imagem precisa de texto alternativo e evitar os erros comuns.

Sua landing tem uma hero image de um executivo sorrindo com o produto, um gráfico de crescimento, e screenshots do dashboard. Um visitante cego ou com leitura de tela ligada ouve: 'imagem', 'imagem', 'imagem'. Ele não sabe o que vê; a promessa visual da página desaparece. Texto alternativo (atributo alt) é a ponte entre o que é mostrado e quem não consegue ver — e não é detalhe: é conversão perdida e conformidade WCAG.

## Por que importa

- Imagens comunicam valor na maioria das landing pages. Um gráfico de 'crescimento de 300%' ou screenshot do produto em ação transmitem confiança e tangibilidade muito mais rápido que texto. Mas se a imagem não tem alt ou tem alt genérico ('image123.jpg' ou 'screenshot'), visitantes usando leitor de tela não captam esse valor. A perda é dupla: acessibilidade e contexto de persuasão. Usuários que dependem de leitura de tela constituem parcela significativa da população; mais ainda têm visão baixa e dependem de zoom + navegação por texto.
- Além disso, texto alternativo impacta SEO. Motores de busca não 'enxergam' imagens; usam o alt para entender contexto. Uma imagem do seu produto sem alt é invisível para ranking; com alt descritivo, melhora relevância. É ganho simultâneo: acessibilidade E visibilidade de busca.

## Como verificar na sua página

- [ ] Toda imagem informativa tem um atributo alt (não vazio ou genérico)?
- [ ] O alt descreve o SIGNIFICADO da imagem, não sua existência ('gráfico crescimento de 300% em Q3' vs. 'gráfico')?
- [ ] Imagens puramente decorativas têm alt vazio (alt='') para não serem anunciadas?
- [ ] Capturas de tela ou gráficos têm alt que resume a informação-chave visível?
- [ ] Ícones com função (ex: seta de scroll) têm alt que explica a ação?
- [ ] Logos de cliente (prova social) têm alt com o nome da empresa ou alt vazio se apenas decorativo?

## Erros comuns

- **Alt genérico ou automático** — alt='image.jpg' ou alt='screenshot 1' não ajuda ninguém. Leitor de tela anuncia o nome do arquivo, sem contexto. Visitante cego não sabe se é hero, gráfico ou ícone.
- **Alt muito longo ou vira parágrafo** — alt='Este é um gráfico que mostra como a ferramenta X aumentou o tempo dos usuários em 300% no terceiro trimestre de 2025, baseado em dados de 5000 clientes' é poluição. Alt deve ser conciso, 100-125 caracteres no máximo.
- **Ícone ou ornamento com alt descritivo desnecessário** — Um ícone de decoração ao lado do headline tem alt='ícone de foguete roxa com chamas'. Leitor de tela anuncia desnecessariamente. Ornamento puro deve ter alt='' para ser ignorado.
- **Ícone interativo sem alt ou com semântica quebrada** — Um ícone de hambúrguer para abrir menu não tem alt, ou tem alt='menu' mas sem label visível. Teclado usuário não consegue entender a função ou o link não é semanticamente conectado.

## Fontes

- WCAG 2.1 — Non-text Content (W3C)
- WebAIM — Alternative Text for Images
- Baymard Institute — E-commerce Product Image & Text Quality

---

**Audite a sua página agora →** [uxaudit.miaconecta.com.br](https://uxaudit.miaconecta.com.br?utm_source=github&utm_medium=isca&utm_campaign=checklist) · grátis: 2 auditorias

<sub>Parte de **landing-page-checklist** · conteúdo sob [CC BY-SA 4.0](../../LICENSE) · mantido por [UX Audit](https://uxaudit.miaconecta.com.br)</sub>
