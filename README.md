# 🚀 TechStore - Vitrine de Produtos Interativa

Esse é projeto TechStore! Desenvolvido com **HTML, CSS e JavaScript**, esse projeto é focado em simular uma vitrine de e-commerce de produtos tecnologicos dinâmica e moderna. O projeto foi estruturado com uma clara separação de responsabilidades (estrutura, estilo e comportamento), ideal para demonstrar os conceitos fundamentais do desenvolvimento web front-end.

### ✨ Funcionalidades Principais

O sistema proporciona uma experiência de navegação rica e interativa, incluindo:

* **Design Moderno:** Layout limpo e responsivo, construído com CSS Grid e Flexbox.
* **Interatividade Total:** A página reage dinamicamente às ações do usuário, como cliques e digitação.
* **Filtro por Categoria:** Permite ao usuário clicar em categorias para visualizar apenas os produtos relevantes.
* **Busca em Tempo Real:** A lista de produtos é filtrada instantaneamente conforme o usuário digita na barra de busca.
* **Renderização Dinâmica:** Os produtos são gerados via JavaScript a partir de uma lista de dados, e não fixos no HTML.
* **Feedback Visual:** Efeitos de `hover` suaves nos botões e cards de produtos melhoram a usabilidade.

### 🛠️ Detalhes Técnicos e Estrutura do Código

O código é organizado em três arquivos distintos, cada um com uma responsabilidade única, o que torna o projeto coeso, de fácil manutenção e escalabilidade.

#### Arquivos Principais

**`index.html`**

É o arquivo central que define toda a estrutura e o conteúdo da página. Ele contém os elementos que serão manipulados pelo JavaScript e estilizados pelo CSS.

* **Estrutura:** Organiza o conteúdo em seções semânticas, como o cabeçalho (`header`), a barra de categorias (`.categories-bar`), a seção de destaque (`.hero-section`) e o contêiner principal de produtos (`.products-container`).
* **Vínculo:** Conecta os arquivos `style.css` e `scripts.js` para que a página funcione corretamente.
* **Elementos Interativos:** Contém o campo de busca (`.search-input`) e os botões de categoria (`.category-btn`) com atributos `data-category` que são essenciais para a lógica de filtragem.

**`style.css`**

Responsável por toda a parte visual do projeto, desde o layout geral até os mínimos detalhes de design.

* **Layout:** Utiliza **CSS Grid** para organizar os cards de produtos e **Flexbox** para alinhar elementos como o cabeçalho e os menus.
* **Estilização Avançada:** Emprega **Variáveis CSS** (`:root`) para um gerenciamento de tema de cores coeso e fácil de manter.
* **Animações:** Aplica `transitions` e a pseudo-classe `:hover` para criar efeitos de animação suaves, como nos cards de produtos que se elevam ao passar o mouse.

**`scripts.js`**

Controla todo o comportamento e a interatividade da página, manipulando os elementos HTML.

* **`mostrarProdutos()`**
    * **Responsabilidade:** Renderiza os produtos na tela.
    * **Lógica:** Filtra o array principal de `produtos` com base nas variáveis `categoriaAtual` e `textoPesquisa`. [cite_start]Em seguida, gera o HTML para cada produto filtrado e o insere no `.products-container`.
* **`pesquisar()`**
    * **Responsabilidade:** Atualiza o filtro de busca.
    * **Lógica:** É chamada a cada vez que o usuário digita no campo de busca, atualizando a variável `textoPesquisa` e invocando `mostrarProdutos()` para refletir o resultado em tempo real.
* **`trocarCategoria()`**
    * **Responsabilidade:** Altera a categoria de produtos exibida.
    * **Lógica:** É chamada quando um botão de categoria é clicado, atualizando a variável `categoriaAtual` e o estilo do botão ativo, e então invoca `mostrarProdutos()` para exibir os itens da nova categoria.

### 🚀 Como Executar

Para rodar este projeto, você precisa apenas de um navegador web.

1.  Clone o repositório ou baixe os arquivos (`index.html`, `style.css`, `scripts.js`).
2.  Abra seu explorador de arquivos.
3.  Navegue até o diretório onde os arquivos estão localizados.
4.  Dê um duplo-clique no arquivo **`index.html`**.

O projeto será aberto no seu navegador padrão e você já poderá interagir com a página.
