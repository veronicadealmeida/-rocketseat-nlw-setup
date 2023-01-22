# BACKEND

```
npm run dev
```

## CONFIGURAÇÃO DO AMBIENTE

1. Instalar NVM (para gerenciar versões diferentes do node)
2. Criar projeto com node

   ```
   npm init -y
   ```

3. Instalar Fastify (utilizaremos ao invés do express)

   ```
   npm i fastify
   ```

4. Inicializar npx

   ```
   npx tsc --init
   ```

5. Alterar tsconfig.json

   ```
   "target": "ES2020"
   ```

6. Instalar tsx como dependência de desenvolvimento

   ```
   npm tsx -d
   ```

7. Incluir comando de atalho no package.json para executar de forma mais fácil

   ```
       "scripts": {
           "dev": "tsx watch ./src/server.ts"
           }
   ```

8. Configurar prisma para acesso aos dados como dependência de desenvolvimento

   ```
   npm i -D prisma
   ```

9. Instalar o client do prisma (não é uma dependência de desenvolvimento)

   ```
   npm i @prisma/client
   ```

10. Inicializar o prisma utilizando o banco de dados SQLite

    ```
    npx prisma init --datasource-provider SQLite
    ```

11. Instalar CORS
    ```
    npm i @fastify/cors
    ```

## Extensões

1. Prisma

   - para visualizar o relacionamento das tabelas

     - instalar

       ```
       npm i -D prisma-erd-generator @mermaid-js/mermaid-cli
       ```

     - Adicionar em schema.prisma
       ```
       generator erd {
           provider = "prisma-erd-generator"
       }
       ```
     - Para gerar o model ( será gerado no arquivo ERD.svg )
       ```
       npx prisma generate
       ```

2. Seed

   - criar um arquivo dentro da pasta prisma seed.ts

   - no package.json incluir

     ```
     "prisma": {
          "seed": "tsx prisma/seed.ts"
      }
     ```

   - para executar o seed
     ```
     npx prisma db seed
     ```

## NOTAS

- node: permite utilizar javascript no back-end (tirou V8 do chrome e colocou no node)
- instalção do nvm https://josiaspereira.com.br/como-configurar-o-node-com-nvm-windows/
- comandos NVM

  ```
  nvm install latest
  nvm list
  nvm use 16.15.1
  ```

- Para executar um programa .ts

  ```
  npx tsx src/server.ts
  ```

- Tipos de métodos

  - GET
  - POST
  - PUT
  - PATCH
  - DELETE

- Para Atualizar as tabelas no prisma, executar o comando

  ```
  npx prisma migrate dev
  ```

- Para visualizar os dados no prisma

  ```
  npx prisma studio
  ```

- CORS: determina quem pode acessar os dados do backend

- seed: é um populador de bando de dados
