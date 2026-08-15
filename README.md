# Nelson Lisboa — Portfólio Pessoal

Landing page pessoal desenvolvida como primeiro projeto de uma trilha de evolução em desenvolvimento web, com foco em fundamentos sólidos de HTML semântico e CSS moderno antes da introdução de frameworks.

**🔗 Demo ao vivo:** https://nemhh25.github.io/meu-portifolio/

## Sobre o projeto

Este é o Projeto 1 de uma sequência de portfólio pensada para demonstrar evolução técnica progressiva. O objetivo aqui foi construir uma página de apresentação profissional utilizando apenas HTML5 e CSS3 puros — sem frameworks ou bibliotecas — para consolidar fundamentos antes de avançar para React, TypeScript e back-end nos próximos projetos.

## Demonstração

<!--
Adicione aqui uma captura de tela limpa (sem barra de navegador/DevTools visível).
Crie uma pasta `screenshots/` no repositório, adicione a imagem lá e referencie assim:
![Preview do portfólio](./screenshots/preview-desktop.png)
-->

## Funcionalidades

- Layout responsivo (mobile, tablet e desktop)
- Tipografia fluida com `clamp()`, sem necessidade de media queries para o título principal
- Navegação por teclado com indicador de foco visível (`:focus-visible`)
- Respeita a preferência do sistema por movimento reduzido (`prefers-reduced-motion`)
- Paleta e tipografia centralizadas via CSS Custom Properties (design tokens)
- HTML semântico (`header`, `main`, `section`) para melhor SEO e acessibilidade

## Tecnologias utilizadas

- **HTML5** semântico
- **CSS3** — Flexbox, Custom Properties, `clamp()`, pseudo-classes (`:not()`, `:focus-visible`)
- **Google Fonts** — Cormorant Garamond (títulos) e Inter (corpo de texto)

Nenhum framework ou biblioteca foi utilizado nesta etapa — decisão deliberada para fixar fundamentos de HTML/CSS antes de introduzir ferramentas como React.

## Decisões técnicas e de design

- **Paleta "terno preto":** fundo quase-preto (`#0d0d0d`, não preto puro) combinado com texto off-white e um único acento dourado acinzentado, buscando uma sensação editorial e sóbria em vez de um visual genérico de template.
- **Par tipográfico:** uma serifa fina (Cormorant Garamond) para títulos, contrastando com uma sans-serif estruturada (Inter) para corpo e rótulos — reforça hierarquia visual sem depender de imagens.
- **Design tokens:** toda a paleta de cores foi centralizada em variáveis CSS (`:root`), permitindo ajuste do tema inteiro a partir de um único ponto.
- **Mobile-first:** o layout foi construído como coluna única por padrão; nenhuma media query foi necessária até o momento graças ao uso de `clamp()` e `max-width` com `margin: 0 auto`.

## Desafios encontrados e soluções

| Desafio | Solução |
|---|---|
| Branch local criada como `Main` (maiúsculo), incompatível com o padrão `main` do GitHub | Renomeada com `git branch -M main`; `init.defaultBranch` configurado globalmente para evitar recorrência |
| Push rejeitado por histórico não relacionado (repositório remoto com commit inicial próprio) | Resolvido com `git pull origin main --allow-unrelated-histories` |
| Marcadores de conflito de merge (`<<<<<<< HEAD`) deixados no HTML após merge | Identificados e removidos manualmente, com o conteúdo revisado antes do commit final |

## Testes realizados

- Verificação visual responsiva manual via DevTools em 375px (mobile), 768px–1024px (tablet) e desktop
- Revisão de código linha a linha em cada etapa, buscando HTML inválido, CSS órfão/duplicado e problemas de acessibilidade

## Como rodar localmente

Este é um projeto estático, sem processo de build ou dependências:

```bash
git clone https://github.com/Nemhh25/meu-portifolio.git
cd meu-portifolio
```

Depois, basta abrir o `index.html` diretamente no navegador (ou usar uma extensão como Live Server no VS Code para recarregamento automático).

## Estrutura do projeto

```
meu-portifolio/
├── index.html
├── style.css
└── README.md
```

## Próximos passos

- Substituir a seção "Projetos" por projetos reais conforme forem concluídos na trilha
- Avaliar alternância de tema claro/escuro
- Migração para React no Projeto 2 do portfólio

## Autor

**Nelson Lisboa**

- GitHub: [@Nemhh25](https://github.com/Nemhh25)
- LinkedIn: [Nelson Lisboa](https://www.linkedin.com/in/nelsonlisboa/)
- Email: nelsondossantos739@gmail.com
