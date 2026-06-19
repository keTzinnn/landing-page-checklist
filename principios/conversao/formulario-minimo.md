# Formulário pedindo só o essencial

> **Categoria:** Conversão · **impacto alto**
> Campos mínimos e microcopy justificam cada pergunta sensível, reduzindo fricção e abandonos antes da conversão.
>
> 🇺🇸 [English version](../../principles/conversion/minimal-form.md)

Quanto mais campos um formulário pede, menor a taxa de conclusão. Cada campo adicional é uma barreira psicológica. O princípio do formulário mínimo exige: solicitar só dados realmente necessários, justificar por microcopy campos sensíveis (telefone, CPF, empresa), e reduzir opcionalidade falsa. Usuários sentem menos fricção, abandonam menos, e a conversão sobe.

## Por que importa

- Formulários longos criam atrito cognitivo. A Lei de Hick diz que mais opções (ou campos) aumentam tempo de decisão e abandono. Reduzir o número de campos reduz esse custo psicológico, especialmente campos sensíveis como telefone, CPF ou empresa. Usuários hesitam quando temem spam ou vazamento de dados. Sem microcopy que explique *por quê* você precisa disso, a desconfiança vence a vontade de converter.
- Microcopy funciona porque humaniza a fricção. 'Telefone: para contatá-lo após aprovação (não vendemos seu número)' reduz medo de spam. 'CPF: obrigatório por lei para contratos B2B' justifica a invasão. Sem essa clareza, o usuário projeta cenários negativos. O medo narrativo (imaginado) é mais forte que o medo baseado em evidência. Microcopy interrompe a narrativa ruim e reinstala confiança.
- Formulários mínimos também aumentam qualidade de dados. Menos campos = menos preenchimento automático errado, menos emails digitados de pressa. E facilitam testes: é possível testar variações rápido (5 vs 8 campos, com ou sem microcopy) e medir impacto real em conversão.

## Como verificar na sua página

- [ ] Você pede nome completo quando só precisa do nome? Ou empresa quando poderia vir após conversão?
- [ ] Cada campo sensível (telefone, CPF, dados bancários) tem microcopy que explica por quê você precisa e como os dados serão usados?
- [ ] Você distinguiu campos obrigatórios de opcionais visualmente? Opcionais devem parecer opcionais, não armadilhas.
- [ ] O formulário foi testado para medir taxa de abandono por campo — qual é o campo onde mais gente sai?
- [ ] Você poderia mover algum campo para *depois* da conversão (ex.: dados de faturamento após confirmação de compra)?
- [ ] A ordem dos campos segue lógica: dados pessoais simples primeiro, dados sensíveis ou complexos depois?
- [ ] Você validou se a microcopy atual reduz fricção ou se parece jargão corporativo que ninguém lê?

## Erros comuns

- **Formulário com 15+ campos na mesma tela** — Usuário vê parede de perguntas, abandona antes de começar. Teste: divida em duas telas, ou reduza campos para o essencial (nome, email, telefone). Dados complementares como empresa podem vir após conversão. Resultado esperado: aumento em envios completos.
- **Telefone ou CPF sem microcopy explicativa** — Usuário pensa 'por que querem isso?', teme venda de dados, sai. Adicione em 1 linha: 'Telefone: para contato pós-aprovação. Seu número não é vendido nem compartilhado.' Isso custa zero espaço, salva conversões.
- **Campo 'Empresa' obrigatório em formulário consumer** — Consumidor comum não tem empresa. Você força resposta vazia, campo inválido, conversão falha. Deixe vazio ou mude para 'Profissão (opcional)'.
- **Validação de erro genérica após envio** — Usuário enche tudo, envia, vê 'Erro: preencha campos obrigatórios' sem dizer qual. Ele fica frustrado, fecha a aba. Valide em tempo real por campo (inline), mostre erro específico antes que clique enviar.

## Fontes

- Luke Wroblewski, Web Form Design: Filling in the Blanks (Rosenfeld Media, 2008)
- Nielsen Norman Group, Form Design Patterns and Minimize Cognitive Load (nngroup.com)
- Robert Cialdini, Influence: The Psychology of Persuasion (HarperBusiness, 2006)
- Baymard Institute, Form Field Labels and Form Field Studies (baymard.com)

---

**Audite a sua página agora →** [uxaudit.miaconecta.com.br](https://uxaudit.miaconecta.com.br?utm_source=github&utm_medium=isca&utm_campaign=checklist) · grátis: 2 auditorias

<sub>Parte de **landing-page-checklist** · conteúdo sob [CC BY-SA 4.0](../../LICENSE) · mantido por [UX Audit](https://uxaudit.miaconecta.com.br)</sub>
