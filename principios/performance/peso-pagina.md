# Página leve

> **Categoria:** Velocidade · **técnico**
> Páginas mais leves carregam mais rápido em conexões lentas. Reduzir bytes em imagens, scripts e CSS melhora experiência, reduz bounce rate e aumenta conversão — especialmente em mobile.
>
> 🇺🇸 [English version](../../principles/speed/page-weight.md)

O tamanho total de uma página — em kilobytes — determina velocidade de carregamento. Quanto mais leve, mais rápido chega ao visitante. Em redes móveis (3G/4G), cada megabyte extra custa segundos reais. Atraso de carregamento empurra o visitante para o abandono antes de ele ver a oferta — quanto mais pesada a página, maior o risco de perder quem chegou. Este princípio verifica se a página está otimizada em peso — imagens comprimidas, scripts desnecessários removidos, CSS puro sem bloat.

## Por que importa

- Conexões móveis são limitadas. Um visitante em rede 3G enfrenta largura de banda real de ~1-2 Mbps. Uma página de 5 MB leva 40 segundos para carregar — tempo que ninguém aguarda. Reduzir para 1-2 MB muda a experiência para realista (10-20 segundos), onde abandono é menor. Desktop beneficia menos (conexões mais rápidas), mas ainda ganha com latência reduzida.
- Google Core Web Vitals penaliza páginas lentes em busca orgânica. Velocidade não é apenas UX — é sinal de qualidade para motores de busca. Página lenta ranqueia pior, recebe menos tráfego, converte menos por falta de volume. A equação é: peso reduzido → carregamento rápido → melhor ranking → mais tráfego → mais conversões.
- A psicologia de espera é não-linear. Os primeiros 3 segundos concentram a decisão de ficar ou sair. Entre 3-10 segundos, taxa de abandono sobe exponencialmente. Abaixo de 3 segundos, o visitante não reclama de velocidade — apenas navega. Otimizar peso é forma mais efetiva de ficar abaixo dessa linha.

## Como verificar na sua página

- [ ] O tamanho total da página (HTML, CSS, JS, imagens, fontes) fica entre 1-2 MB idealmente, máximo 3 MB em desktop, máximo 1.5 MB em mobile?
- [ ] Imagens estão em formato otimizado (WebP com fallback para PNG/JPEG) e redimensionadas para cada tela (não servir imagem de 2000px para tela de 375px)?
- [ ] Scripts não-críticos para carregamento inicial estão diferidos ou carregados assincronamente (async/defer)?
- [ ] CSS crítico (acima da dobra) está inline ou em arquivo crítico separado; CSS não-crítico é carregado de forma não-bloqueante?
- [ ] Fontes web estão limitadas a 2-3 variações (peso/estilo) e são carregadas com preload ou font-display otimizado para reduzir layout shift?
- [ ] Bibliotecas JavaScript não-essenciais foram removidas ou substituídas por vanilla JS / bibliotecas menores (ex: Alpine em vez de jQuery)?
- [ ] Cache de navegador está configurado (headers Cache-Control apropriados) para evitar redownload em visitas futuras?
- [ ] A página usa compressão de transferência (gzip, brotli) no servidor?

## Erros comuns

- **Imagens de alta resolução sem otimização** — Página carregando imagens de 4K para dispositivos mobile. Uma foto de 3MB sozinha consume metade do orçamento de peso. Solução: redimensionar para primeira tela, usar WebP com fallback, e aplicar lazy-loading para imagens abaixo da dobra.
- **Scripts de rastreamento e third-party sem controle** — Google Tag Manager, Intercom, Hotjar, CRM widgets, pixel de anúncio — cada uma carrega 100-500KB. Múltiplas ferramentas acumulam rápido. Solução: auditar e remover ferramentas não-essenciais; atrasar carregamento de não-críticas para depois da conversão.
- **CSS e JS não-minificados ou duplicados** — Arquivo style.css com 200KB de código não-minificado. Arquivo bundle.js carregando duas versões de Bootstrap. Solução: minificar, remover duplicatas, usar tree-shaking em bundlers.
- **Fontes web carregadas sem limites** — 10 variações de uma fonte (Light, Regular, Bold, Black, italic versions) todas sendo baixadas. Solução: limitar a 2-3 variações críticas; usar system fonts como fallback.
- **Sem lazy-loading de imagens** — Todas as imagens carregam na primeira requisição, mesmo as 2000px abaixo da dobra. Solução: usar loading='lazy' ou Intersection Observer para defer imagens fora da primeira tela.

## Fontes

- Google Web Vitals: Largest Contentful Paint (LCP) and page load optimization (developers.google.com/web/vitals)
- Nielsen Norman Group: Website Response Time and User Satisfaction (study on impact of load time on bounce rate and engagement)
- Baymard Institute: Impact of load time on e-commerce conversion
- Julian Shapiro: Web Performance Best Practices (performance budgets, image optimization, and lazy-loading strategies)

---

**Audite a sua página agora →** [uxaudit.miaconecta.com.br](https://uxaudit.miaconecta.com.br?utm_source=github&utm_medium=isca&utm_campaign=checklist) · grátis: 2 auditorias

<sub>Parte de **landing-page-checklist** · conteúdo sob [CC BY-SA 4.0](../../LICENSE) · mantido por [UX Audit](https://uxaudit.miaconecta.com.br)</sub>
