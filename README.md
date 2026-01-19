# Challenge Bank

Repositorio exclusivo para desafios em JSON.
Este repo e consumido pelo app, sem acesso ao codigo-fonte.

## Objetivo
- Receber PRs da comunidade com novos desafios.
- Manter os desafios isolados do repositorio do app.

## Politica de contribuicao
- O repositorio do app nao aceita PRs de desafios.
- Pull requests devem conter apenas arquivos JSON em `challenges/`.

## Estrutura
- `languages.json` lista as linguagens disponiveis
- `schema.json` define o formato valido de um desafio
- `challenges/` contem um arquivo por linguagem
  - `dart.json`
  - `javascript.json`
  - `python.json`
  - `java.json`

## Formato do desafio
Cada arquivo de linguagem e um array de objetos no formato:

```json
[
  {
    "id": "dart_001",
    "title": "Inverter string",
    "description": "Escreva uma funcao que receba uma string e retorne o seu inverso.",
    "solution": "String reverse(String input) => input.split('').reversed.join();",
    "level": "easy",
    "languageId": "dart",
    "isCompleted": false
  }
]
```

## Campos
- `id`: identificador unico do desafio
- `title`: titulo exibido ao usuario
- `description`: enunciado do desafio
- `solution`: uma solucao valida (texto ou codigo)
- `level`: `easy` | `medium` | `hard`
- `languageId`: deve existir em `languages.json`
- `isCompleted`: bool (pode iniciar como `false`)

## Regras
- Cada linguagem deve ter um arquivo com nome igual ao `languageId`.
- Evite duplicar `id` entre desafios.
- Mantenha o texto em portugues.
