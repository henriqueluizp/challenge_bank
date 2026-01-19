# Challenge Bank

Repositorio exclusivo para desafios em JSON.
O app consome esses arquivos sem expor o codigo.

Estrutura sugerida:
- schema.json
- languages.json
- challenges/
  - dart.json
  - javascript.json

Regras:
- languageId deve existir em languages.json
- level: easy | medium | hard
- isCompleted e somente no app (nao entra no repo)

Publicacao rapida:
1) git init
2) git add . && git commit -m "Initial challenges"
3) git remote add origin <URL>
4) git push -u origin main
