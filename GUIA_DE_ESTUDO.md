# Guia para entender e explicar o projeto

Este material foi preparado com auxílio de IA. O enunciado exige compreensão: revise, personalize e explique as decisões antes da entrega. Não apresente testes, leituras do AVA ou experiências pessoais que você não realizou.

## 1. O que o HTML faz?

O HTML descreve o significado e a ordem do conteúdo. `header` contém identidade e navegação; `nav` reúne links; `main` guarda o conteúdo principal; `section` separa os assuntos; `article` representa cada livro ou unidade; `footer` encerra a página. Há um único `h1` e títulos `h2` e `h3` para os níveis seguintes.

`lang="pt-BR"` informa o idioma. `meta charset="UTF-8"` preserva os acentos. `meta name="viewport"` permite que celulares usem sua largura real de layout.

## 2. Como HTML e CSS estão ligados?

`<link rel="stylesheet" href="css/style.css">` carrega o arquivo de estilos. O caminho é relativo ao HTML, por isso funciona tanto no computador quanto em uma subpasta do GitHub Pages.

No CSS, `.book-card` seleciona todos os elementos com `class="book-card"`. `#livros` identifica a seção de livros. Classes são reutilizáveis; IDs devem ser únicos.

## 3. Por que usar variáveis?

Em `:root`, `--blue: #005fa8` define o azul principal. `color: var(--blue)` reaproveita esse valor. Ao editar a variável, links e componentes relacionados mudam juntos. Isso reduz inconsistências.

## 4. Como o catálogo se adapta?

`.book-grid` usa `display: grid`. Em telas largas, `repeat(3, minmax(0, 1fr))` distribui três colunas com o mesmo espaço disponível. Abaixo de 1000 px, são duas; abaixo de 640 px, uma. `minmax(0, 1fr)` permite que as colunas encolham sem impor uma largura mínima de conteúdo inadequada.

O contêiner usa `min(1160px, calc(100% - 64px))`: ocupa a largura disponível com margens e para de crescer em 1160 px. No celular, as margens caem para 20 px de cada lado.

## 5. O que é Flexbox?

O cabeçalho e as ações do banner usam Flexbox para alinhar elementos em uma dimensão. O Grid organiza áreas em linhas e colunas, como os cartões do catálogo. Cada recurso foi escolhido conforme a organização do conteúdo.

## 6. Por que não há menu hambúrguer?

São apenas quatro links. No celular, eles permanecem visíveis em uma linha abaixo da marca. A solução evita esconder opções e não depende de JavaScript nem de truques com checkbox.

## 7. Como funciona “Saiba mais” sem JavaScript?

O navegador oferece esse comportamento com `<details>` e `<summary>`. O título clicável fica em `summary`; o restante do conteúdo aparece ao abrir `details`. Também é possível usar teclado. O atributo `open` é controlado nativamente pelo navegador.

## 8. Quais recursos de acessibilidade existem?

- Link inicial “Pular para o conteúdo”, visível ao receber foco.
- Foco com contorno contrastante em `:focus-visible`.
- Títulos hierárquicos e regiões semânticas.
- Texto visível para ações e categorias; não dependem só de cor.
- Imagens decorativas com `alt=""`; ilustração principal com descrição.
- Nome completo do livro no texto acessível de cada “Saiba mais”.
- Preferência por movimento reduzido desativa a rolagem suave.

Isso não equivale a uma certificação de conformidade integral com WCAG.

## 9. Por que os livros são demonstrativos?

O objetivo é montar a interface inicial, sem inventar que uma obra está disponível na instituição. Títulos, descrições e capas foram criados para a demonstração e identificados dessa forma. Os canais oficiais permitem consultar o catálogo real.

## 10. Como testar por conta própria?

1. Abra o HTML e altere a largura da janela.
2. No DevTools, ative a barra de dispositivos e teste 320, 390, 768, 1024 e 1440 px.
3. Confira se não existe rolagem horizontal, cortes ou sobreposições.
4. Use Tab desde o início e confira o link de salto.
5. Pressione Enter no link de salto e nos resumos dos livros.
6. Amplie para 200% e confirme se o texto continua legível.
7. Abra os links externos; eles dependem da disponibilidade das páginas oficiais.
8. Compare os resultados com as capturas do relatório.

## Perguntas para praticar

- O que mudaria se `box-sizing: border-box` fosse removido?
- Por que a imagem pode ter largura de 100% sem ficar distorcida?
- Qual é a diferença entre um link de âncora e um filtro de dados?
- Por que um botão sem ação seria inadequado?
- Como você adicionaria um sétimo livro mantendo a consistência?
- Onde alteraria o ponto em que o catálogo passa para uma coluna?

## Créditos

Texto de interface e ilustrações SVG preparados para este projeto com auxílio de IA. Marca textual adaptada para exercício acadêmico; não é reprodução de um manual oficial. Os tons de azul e verde tomam como referência o material do enunciado. Nenhuma imagem de terceiros foi incorporada.
