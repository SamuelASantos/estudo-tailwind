## 🛠 Instalação

### ⚙️ Como o Tailwind CSS funciona?
O Tailwind CSS utiliza um conjunto de classes utilitárias que são aplicadas diretamente no HTML para estilizar os elementos. Ele pode ser usado via CDN, integrado em frameworks modernos ou configurado manualmente em projetos independentes.

---

### 🌐 Rodando via CDN
A maneira mais rápida de testar o Tailwind CSS é utilizando um link CDN. Basta adicionar a seguinte linha no `<head>` do seu HTML:

```html
<link href="https://cdn.jsdelivr.net/npm/tailwindcss@latest/dist/tailwind.min.css" rel="stylesheet">
```

Isso permite utilizar as classes do Tailwind diretamente sem precisar de instalação adicional.

---

### 🏗 Adicionando em frameworks
O Tailwind pode ser facilmente integrado a frameworks como React, Vue, Next.js e outros. Normalmente, a instalação é feita com npm ou yarn:

```sh
npm install -D tailwindcss postcss autoprefixer
npx tailwindcss init -p
```

Isso cria um arquivo de configuração `tailwind.config.js`, permitindo personalizar o Tailwind conforme necessário.

---

### 📂 Adicionando em um projeto avulso
Se você deseja usar o Tailwind CSS em um projeto HTML/CSS puro, siga estes passos:

1. Instale o Tailwind CSS:
   ```sh
   npm install -D tailwindcss
   ```
2. Crie um arquivo CSS e importe o Tailwind:
   ```css
   @tailwind base;
   @tailwind components;
   @tailwind utilities;
   ```
3. Compile o CSS com:
   ```sh
   npx tailwindcss -i ./src/input.css -o ./dist/output.css --watch
   ```

---

### 🛠 Extensão para o VSCode
Para melhorar a experiência de desenvolvimento, é recomendado instalar a extensão **Tailwind CSS IntelliSense** no VSCode. Ela fornece:

✅ Autocompletar de classes utilitárias.

✅ Sugestões de estilos e cores.

✅ Suporte para JIT (Just-in-Time).

Para instalar, basta buscar por **Tailwind CSS IntelliSense** na aba de extensões do VSCode e clicar em instalar.

---