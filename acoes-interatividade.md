# 🎯 Ações e Interações no Tailwind CSS

## ✨ 1. Hover e estados do elemento
O Tailwind CSS facilita a adição de estilos interativos, como `hover`, `focus`, `active` e `disabled`. Basta adicionar o prefixo correspondente antes da classe utilitária.

**Exemplo:**
```html
<button class="bg-blue-500 hover:bg-blue-700 text-white font-bold py-2 px-4 rounded">
  Passe o mouse aqui
</button>
```

---

## 🖱 2. Group Hover
O `group-hover` permite alterar o estilo de um elemento quando um pai específico recebe `hover`. Para isso, basta adicionar a classe `group` ao elemento pai e `group-hover:` aos filhos.

**Exemplo:**
```html
<div class="group p-4 border border-gray-300 hover:bg-gray-100">
  <p class="text-gray-500 group-hover:text-black">Passe o mouse aqui</p>
</div>
```

---

## 🌙 3. Dark Mode - Usando Color Scheme do sistema
O Tailwind CSS suporta Dark Mode baseado no esquema de cores do sistema. Basta ativar no `tailwind.config.js`.

**Configuração:**
```js
module.exports = {
  darkMode: 'media', // ou 'class'
}
```

**Exemplo:**
```html
<div class="bg-white dark:bg-gray-900 text-black dark:text-white p-4">
  Modo claro e escuro automático 🌞🌑
</div>
```

---

## 🎨 4. Usando estilos base
O Tailwind permite definir estilos globais e reutilizáveis através do arquivo `tailwind.config.js` e `@apply`.

**Exemplo usando `@apply`:**
```css
.btn {
  @apply bg-blue-500 text-white font-bold py-2 px-4 rounded;
}
```
```html
<button class="btn">Botão reutilizável</button>
```

---

## 🏗 5. Criando componentes
Criar componentes no Tailwind permite reutilizar estilos de forma eficiente dentro de frameworks como React, Vue ou até HTML puro.

**Exemplo com React:**
```jsx
const Button = () => {
  return <button className="bg-blue-500 hover:bg-blue-700 text-white font-bold py-2 px-4 rounded">Clique aqui</button>;
};
```

---

## 🏷 6. Definindo um prefixo
Para evitar conflitos com outras bibliotecas, você pode definir um prefixo no `tailwind.config.js`.

**Configuração:**
```js
module.exports = {
  prefix: 'tw-',
}
```

**Uso:**
```html
<button class="tw-bg-blue-500 tw-text-white">Botão</button>
```

---

## 💎 7. Tailwind UI
O **Tailwind UI** é uma coleção de componentes premium criados pela equipe do Tailwind CSS, prontos para uso.

🔗 Acesse: [https://tailwindui.com/](https://tailwindui.com/)

---