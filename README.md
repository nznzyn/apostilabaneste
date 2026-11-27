# Estuda Banestes 2026

Portal independente de estudos para Técnico Bancário.

## Publicar no GitHub Pages

1. Crie um repositório no GitHub (por exemplo, `estuda-banestes`).
2. Envie **o conteúdo desta pasta** para a raiz do repositório, incluindo `index.html`, `materia.html` e as pastas.
3. Em Settings > Pages, selecione Deploy from a branch, branch `main`, pasta `/ (root)` e Save.
4. Abra o endereço informado pelo GitHub Pages (`https://SEU-USUARIO.github.io/estuda-banestes/`).

## Organização

- `index.html`: página inicial.
- `materia.html`: catálogo das nove disciplinas.
- `materia/<disciplina>/index.html`: menu dos assuntos.
- `materia/<disciplina>/<assunto>.html`: teoria, exemplos e exercícios de cada assunto.
- `css/style.css`: estilos globais e responsivos.
- `javaScript/dados.js`: índice de busca e questões do simulado.
- `javaScript/script.js`: progresso, pesquisa, tema e simulado.
- `imagens/icone.svg`: ícone do portal.
- `guia.html`, `formulario.html`, `fontes.html`, `simulado.html`: materiais complementares.

## Editar

O conteúdo de cada aula está diretamente no respectivo HTML, dentro de `.reading-body`. Ao criar ou renomear aulas, atualize os links das páginas e os metadados de busca em `javaScript/dados.js`. As fórmulas usam MathML nativo.

Para testar, abra `index.html` no navegador ou execute `python -m http.server 8000` na raiz e acesse `http://localhost:8000`. O progresso é salvo no localStorage do navegador; em arquivos locais, a persistência entre páginas depende do navegador. Em GitHub Pages, todas as páginas compartilham a mesma origem. Não há backend nem dependências externas.

Material independente, não oficial do Banestes nem da FCC.
