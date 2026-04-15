# Festivite - Formulario de Convite

Projeto front-end para criacao de convites digitais de eventos, com foco em uma experiencia visual moderna e formulario completo de personalizacao.

## Sobre

A pagina permite configurar informacoes do evento, escolher tema visual, selecionar cor principal, enviar imagem de capa e preencher dados de contato antes de gerar o convite.

## Funcionalidades

- Cadastro de dados do evento:
  - titulo
  - periodo (inicio e fim)
  - tipo (presencial ou online)
  - local/link
  - descricao
- Personalizacao visual:
  - selecao de cor principal
  - selecao de tema do evento
  - alternancia de estilo (escuro/claro)
  - upload de foto de capa
- Dados para contato:
  - nome (validacao obrigatoria)
  - e-mail
  - telefone
- Termos e consentimentos:
  - aceite de termos e politica
  - opt-in para comunicacoes por e-mail e SMS
- Validacoes em JavaScript:
  - exibicao de erro para nome vazio
  - exibicao de erro quando nao ha imagem selecionada no envio do formulario

## Tecnologias utilizadas

- HTML5
- CSS3
- JavaScript (vanilla)
- Google Fonts

## Estrutura de pastas

```text
.
|-- index.html
|-- README.md
|-- assets/
|   |-- icons/
|   `-- image/
`-- styles/
    |-- global.css
    |-- index.css
    `-- layout.css
```

## Como executar localmente

1. Clone ou baixe este repositorio.
2. Abra a pasta do projeto no VS Code.
3. Execute o arquivo `index.html` no navegador.

Sugestao: use a extensao Live Server para atualizar a pagina automaticamente durante o desenvolvimento.

## Estilizacao

- `styles/global.css`: variaveis globais (cores, fontes e reset base).
- `styles/layout.css`: layout principal, campos do formulario e componentes visuais.
- `styles/index.css`: ponto de entrada de estilos via `@import`.

## Comportamento de validacao (script inline)

No arquivo `index.html`, um script controla:

- estado do upload (texto padrao, nome do arquivo selecionado e estado de erro)
- validacao do campo de nome no blur/input
- bloqueio do submit quando houver pendencias obrigatorias

## Melhorias futuras

- mover o JavaScript inline para um arquivo dedicado (ex.: `scripts/main.js`)
- adicionar mascara de entrada para data, telefone e validacoes mais robustas
- implementar persistencia (localStorage ou API)
- criar versao totalmente responsiva para telas menores
- adicionar testes de interface e acessibilidade

## Licenca

Este projeto e para estudo e pratica de desenvolvimento front-end.
