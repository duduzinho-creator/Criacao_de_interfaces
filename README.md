# Projeto de Interface Web: Usabilidade, UX e Acessibilidade

> Link do Projeto no GitHub Pages: [Clique aqui para acessar o site]

---

## Integrantes e Divisão de Tarefas

Cada integrante ficou responsável pela concepção, codificação HTML e validação de 2 telas conectadas do sistema:

| Integrante | Telas sob Responsabilidade | Contribuição Principal |
| :--- | :--- | :--- |
| **Integrante 1** | `index.html` (Home)<br>`sobre.html` (Sobre Nós) | Arquitetura geral, navegação principal e estrutura institucional. |
| **Integrante 2** | `servicos.html` (Serviços)<br>`detalhes-servico.html` (Detalhes) | Layout em grid dos cards e hierarquia visual dos produtos. |
| **Integrante 3** | `blog.html` (Central de Notícias)<br>`artigo.html` (Página de Leitura) | Formatação de leitura confortável, tipografia e contraste visual. |
| **Integrante 4** | `contato.html` (Formulário)<br>`faq.html` (Perguntas Frequentes) | Usabilidade de formulários, rótulos (labels) e acessibilidade de entradas. |

---

## Conceitos Aplicados e Escolhas de Design

### 1. Usabilidade (Heurísticas de Nielsen)
* **Visibilidade do Status do Sistema:** A barra de navegação indica a página atual utilizando o atributo semântico `aria-current="page"` e contraste visual distinto.
* **Consistência e Padrões:** O cabeçalho, a barra de navegação e o rodapé mantêm o mesmo posicionamento e comportamento em todas as 8 telas.
* **Prevenção de Erros e Controle do Usuário:** Formulários possuem rótulos claros (`<label>`) vinculados explicitamente aos campos de entrada através do atributo `for`.

### 2. Experiência do Usuário (UX)
* **Hierarquia Visual e Leitura:** Estrutura baseada no padrão de leitura F, com títulos de destaque (`h1`, `h2`, `h3`) bem definidos tipograficamente.
* **Áreas de Toque (Touch Targets):** Links e botões possuem altura/largura mínima efetiva de `44px`, facilitando o clique em dispositivos móveis.
* **Feedback Visual:** Efeitos de `:hover` e `:focus-visible` aplicados para fornecer confirmação imediata das ações do usuário.

### 3. Acessibilidade (A11y / WCAG 2.1 AA)
* **Contraste de Cores:** A paleta utilizada (Azul escuro `#0f4c81` sobre fundo claro `#ffffff` e `#f8f9fa`) atinge a taxa de contraste superior a 4.5:1 exigida pelas diretrizes WCAG.
* **Navegação por Teclado:** Implementação do link visível de atalho `<a class="skip-link">` para saltar diretamente ao conteúdo principal, além da indicação visual clara de foco (`outline`).
* **HTML Semântico & ARIA:** Uso correto de tags como `<header>`, `<nav>`, `<main>`, `<section>`, `<article>` e `<footer>`, permitindo que leitores de tela (como NVDA e TalkBack) interpretem a estrutura sem ambiguidade.

### 4. Responsividade (Mobile-First & Layouts Flexíveis)
* **Design Fluido:** Utilização de unidades relativas (`rem`, `%`, `vh`) em vez de valores fixos em pixels.
* **CSS Grid e Flexbox:** O catálogo de cards adapta-se automaticamente ao tamanho da tela através do `repeat(auto-fit, minmax(280px, 1fr))`.
* **Media Queries:** Reorganização da barra de navegação em coluna em telas menores que `768px` para evitar rolagem horizontal.

---

## Tecnologias Utilizadas
* **HTML5** (Semântica e Acessibilidade)
* **CSS3** (Variáveis, Flexbox, CSS Grid, Media Queries)
* **Git / GitHub** (Controle de Versão e Colaboração)
* **GitHub Pages** (Hospedagem)
