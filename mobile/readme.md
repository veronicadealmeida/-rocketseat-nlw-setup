# PLUGINS

# PREPARAÇÃO DO AMBIENTE

- Instalar o Expo Go no celular (é um client do Expo Go de desenvolvimento)
- Instalar o Expo

  ```
      npm i -g expo-cli
  ```

  Blank (TypeScript)

- Criar o projeto com --template para que possa escolher o ts

  ```
      npx create-expo-app my-app --template
  ```

  - importar fonte utilizada (inter) do https://fonts.google.com/?query=inter pelo comando (para o server antes)

    ```
        npx expo install expo-font @expo-google-fonts/inter
    ```

# EXECUTANDO A APLICAÇÃO

    ```
        npx expo start
        npx expo start --clear
    ```

# NOTAS

- Figma: https://www.figma.com/file/o3N528ZqMxr9z0xSpqhkSf/Habits-(i)-(Community)?node-id=6%3A343&t=W8ftLvVyFRJcyh4U-0

- Documentação do Ambiente React Native: https://react-native.rocketseat.dev/

- Expo: facilitador do ambiente de desenvolvimento

  - facilita configurações de apis;
  - disponibiliza emulador no celular através de um qrcode

- Pode-se utilizar o celular ou um emulador para o desenvolvimento

- Nativewind: permite estilização na aplicação mobile

- <> : é conhecido como fragment para envolver e devolver um único component

- svg: biblioteca para trabalhar com arquivos svg
- react-native-svg-tranformer: para trabalhar con svg como componente
