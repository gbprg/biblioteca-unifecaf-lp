# Biblioteca Digital UniFECAF

Projeto acadêmico de Design Web. Interface original, estática, construída com HTML e CSS, sem JavaScript, framework ou template pronto.

## Como abrir

Extraia o ZIP inteiro e abra `biblioteca-unifecaf/index.html` em um navegador. Mantenha as pastas `css` e `assets` junto ao HTML. O conteúdo e as imagens funcionam localmente; os links institucionais precisam de internet.

Site público: https://biblioteca-unifecaf-gabriel.navymule64.chatgpt.site

## Organização

- `index.html`: estrutura semântica, textos, links e seis cartões de livros.
- `css/style.css`: identidade visual, componentes, estados de foco e media queries.
- `assets/imagens/`: dez ilustrações SVG originais, incluindo capas demonstrativas.
- `css/visualizacao.css`: arquivo auxiliar de captura; não é utilizado pela página principal.

## Funcionalidades reais

- Menu e botões com navegação para seções por âncoras.
- Atalhos de áreas direcionam a um título representativo; não são filtros.
- `details` e `summary` expandem informações dos seis livros sem JavaScript.
- Links direcionam aos serviços oficiais da instituição.
- Link de salto para o conteúdo e indicação de foco para teclado.
- Layout de três, duas ou uma coluna, conforme a largura da tela.

Não há login, busca dinâmica, empréstimos, banco de dados nem envio de formulário. A proposta do enunciado é a primeira interface web. Os títulos e as capas são ilustrativos, sem promessa de disponibilidade no acervo real. As imagens de prédios são ilustrações genéricas, não fotografias das unidades.

## Como personalizar

Edite textos em `index.html`. Altere as cores em `:root`, no começo de `css/style.css`. Para mudar um livro, mantenha o `id` usado pelo atalho de área ou atualize o link correspondente. Ao trocar uma imagem, preserve um texto alternativo adequado e as proporções.

## Publicação do repositório (pendente)

O site público já está publicado. O enunciado também pede um repositório público separado. Para isso, crie um repositório público chamado `biblioteca-unifecaf` no seu GitHub e envie o CONTEÚDO desta pasta, de modo que `index.html` fique na raiz do repositório. Não envie apenas o ZIP.

Opcionalmente, publique também pelo GitHub Pages: em Settings > Pages, escolha Deploy from a branch, branch main, pasta /(root), e salve. Use o endereço que o GitHub mostrar após concluir a publicação. O site já publicado acima dispensa essa segunda hospedagem, mas não dispensa o repositório público.

Documentação: https://docs.github.com/en/pages/quickstart

## Antes de enviar ao professor

1. Leia `GUIA_DE_ESTUDO.md` e teste a página para entender o código.
2. Revise o relatório e confira a identificação acadêmica exigida pelo AVA.
3. Abra o site no seu smartphone e teste o menu e “Saiba mais”.
4. Crie ou envie o repositório público e copie seu link.
5. Envie o PDF, este projeto, o link do site e o link do repositório.

O vídeo pitch foi excluído deste pacote a pedido do aluno; essa exclusão não representa uma dispensa concedida pela instituição.
