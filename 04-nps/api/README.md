# Utilizando Typescript

- Instalar typescript
`yarn add -D typescript`

- Iniciar o typscript
`yarn tsc --init`

- Converter o código em tempo de execução
`yarn ts-node-dev`

- Adicionar script no package.json
```json
"scripts": {
  "dev": "ts-node-dev --transpile-only --ignore-watch node_modules src/server.ts"
},
```

# Migrations TypeORM
```
// Cria uma migration
yarn typeorm migration:create -n "CreateUsers"

// Roda as migrations
yarn typeorm migration:run

// Desfaz as migrations
yarn typeorm migration:revert
```