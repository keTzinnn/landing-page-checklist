# Formulário que previne erros antes do envio

> **Categoria:** Conversão · **impacto alto**
> Sinalize campos obrigatórios e formato esperado antes do envio para evitar que o visitante descubra erros só ao tentar submeter o formulário.

Visitante preenche formulário, clica enviar, recebe erro dizendo que um campo é obrigatório ou o formato não é válido. Frustrante. Pior ainda quando o campo estava lá o tempo todo, mas nada indicava que era necessário ou qual formato. Um formulário bem sinalizado reduz esse atrito: campos obrigatórios marcados, formato esperado explicado (ex.: "DD/MM/AAAA" para datas, "11 dígitos" para telefone), validação ao sair do campo quando relevante. Não é decoreba — é respeito ao tempo do visitante.

## Por que importa

- Quando um visitante enfrenta um erro de formulário sem avisos prévios, precisa reler o campo, entender o que deu errado, corrigir e tentar novamente. Cada ciclo consome atenção e cria fricção. Pesquisas de usabilidade mostram que formulários com indicadores visuais claros (asterisco ou label 'obrigatório', exemplos de formato) e validação em tempo real reduzem abandono e aumentam conclusão. O padrão 'validar tudo no servidor após o clique' é antiquado — hoje é esperado feedback imediato.
- Para landing pages de conversão, cada segundo conta. Um visitante que abandona no formulário por frustração não volta. Além disso, a ausência de indicadores claros pode gerar desconfiança: 'por que não dizem se é obrigatório?' vira 'será que estão roubando dados'. Sinalizar claramente (e validar progressivamente) aumenta taxa de conclusão e transmite profissionalismo — o oposto de um formulário genérico que castiga o visitante por adivinhar.
- Além da experiência geral, campos obrigatórios e instruções de formato devem estar amarrados semanticamente na estrutura da página — não só visualmente. Um usuário de leitor de tela ou teclado precisa saber se um campo é obrigatório antes de tentar preencher. Quando a página está bem estruturada, essas indicações são acessíveis a qualquer ferramenta — é fundação, não acessório.

## Como verificar na sua página

- [ ] Todo campo obrigatório está marcado visualmente (ex.: asterisco, cor, label) E indicado semanticamente na estrutura da página?
- [ ] Cada campo obrigatório tem uma label clara que explica o que espera (ex.: 'E-mail' vs. 'E-mail (nome@exemplo.com)')?
- [ ] Campos com formato específico (CPF, data, telefone) exibem um exemplo ou máscara que deixa claro (ex.: 'DD/MM/AAAA' ou placeholder '(11) 9xxxx-xxxx')?
- [ ] Há validação e feedback antes da submissão (ex.: campo fica visualmente destacado ao sair de foco se vazio, mostra dica)?
- [ ] Campos com validação (email, CPF, número) avisam o que está errado sem obrigar submit primeiro?
- [ ] Mensagens de instrução (ex.: 'Digite apenas números') estão claramente associadas ao campo visível?
- [ ] O formulário não tem campos 'ocultos' como obrigatórios — tudo é descobrível antes de tentar enviar?

## Erros comuns

- **Campo obrigatório só marcado visualmente** — Um asterisco ou cor indica que é obrigatório, mas sem indicação semântica apropriada na estrutura. Usuários de tecnologia assistiva não recebem o aviso, e navegadores não conseguem ativar validação nativa.
- **Label desconectada do campo** — Um campo de texto e sua label estão lado a lado visualmente, mas sem associação estrutural clara. Usuários mobile e de teclado precisam clicar no campo exato; a label não expande a área sensível ou o acesso.
- **Formato esperado não é claro** — Campo de telefone sem exemplo, sem máscara, sem instrução. Visitante envia '+ 55 11 98765-4321' quando o sistema espera '11987654321', recebe erro genérico e não sabe o que corrigir.
- **Validação só acontece após submit** — Visitante preenche email como 'usuario@' (sem domínio), clica enviar, recebe erro. Sem feedback em tempo real, não há oportunidade de corrigir antes de reenviar o formulário inteiro.

## Fontes

- Usability Heuristics for User Interface Design — Nielsen (Heuristic #5: Error Prevention and Recovery)
- Web Form Design — Luke Wroblewski (best practices for form labeling, validation, and user guidance)
- Web Content Accessibility Guidelines (WCAG) 2.1 — W3C (3.3.1 Error Identification, 3.3.2 Labels or Instructions)
- Form Field Research Report — Baymard Institute (impact of required field indicators and labeling on form completion)

---

**Audite a sua página agora →** [uxaudit.miaconecta.com.br](https://uxaudit.miaconecta.com.br?utm_source=github&utm_medium=isca&utm_campaign=checklist) · grátis: 2 auditorias

<sub>Parte de **landing-page-checklist** · conteúdo sob [CC BY-SA 4.0](../../LICENSE) · mantido por [UX Audit](https://uxaudit.miaconecta.com.br)</sub>
