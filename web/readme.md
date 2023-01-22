1. Criar projeto no vite

   ```
   npm create vite@latest
   ```

2. Instalar dependências

   ```
   npm install
   ```

3. Instalar

   ```
       npm install -D tailwindcss postcss autoprefixer
       npx tailwindcss init -p
   ```

4. No arquivo tailwind.config.cjs

   ```
   content: ['./src/**/*.tsx', './index.html'],
   ```

5. Criar arquivo de stilos

   - criar pasta styles dentro do src
   - criar arquivo global.css

   ```
       @tailwind base;
       @tailwind utilities;
       @tailwind components;
   ```

6. Dentro do app.tsx adicione essa linha import
   ```
    './styles/global.css';
   ```

# Notas

- Para executar o server
  ```
  npm run dev
  ```
