# 🔴🔵 Homem Aranha - Um Novo Dia 🕷🕸🔴🔵

> Inspirado pela minha admiração pelo Homem-Aranha, recriei este projeto para colocar em prática os conhecimentos adquiridos na WebHub.

---

## 📌 Sobre o Projeto

Este projeto é uma landing page interativa e imersiva inspirada no universo do **Homem-Aranha**, desenvolvida para demonstrar técnicas avançadas de animação web baseadas em rolagem (*scroll-driven animations*).

A aplicação conta com:
- **Sequência de Frames Animados**: Animação de entrada sincronizada com a rolagem do usuário no Canvas.
- **Efeito Typographic Fade**: Animação letra por letra das sinopses do filme utilizando a biblioteca SplitText.
- **Revelação de Trailer**: Abertura dinâmica no estilo máscara (*clip-path*) revelando o trailer interativo.
- **Selo Rotatório**: Animação contínua e fluida do badge circular (`.scroll-badge__ring`).
- **Navegação com Âncora**: Botão de navegação que rola a página suavemente até o trailer.

---

## 🛠️ Tecnologias Utilizadas

- **HTML5**: Estruturação semântica e acessível da página.
- **CSS3**: Estilização moderna, variáveis CSS, animações `@keyframes` e layout responsivo.
- **JavaScript (ES6+)**: Lógica da aplicação, manipulação do DOM e controle do player de vídeo.
- **GSAP (GreenSock Animation Platform)**:
  - `GSAP Core`: Motor de animação ultra-performático.
  - `ScrollTrigger`: Sincronização de animações com a rolagem da página.
  - `ScrollSmoother`: Rolagem suave (smooth scroll).
  - `SplitText`: Quebra e animação de texto caractere por caractere.
- **Google Fonts**: Tipografia com a fonte *Poppins*.

---

## 📦 Bibliotecas Necessárias e Instalação

### Opção 1: Via CDN (Recomendado / Já Configurado)

O projeto está configurado para carregar as bibliotecas do GSAP diretamente via **CDN (Content Delivery Network)** no arquivo `index.html`. Não é necessário instalar nenhuma dependência via terminal para visualizar o projeto.

As dependências incluídas no `index.html` são:

```html
<!-- GSAP Core + Plugins -->
<script src="https://cdn.jsdelivr.net/npm/gsap@3.13.0/dist/gsap.min.js"></script>
<script src="https://cdn.jsdelivr.net/npm/gsap@3.13.0/dist/ScrollTrigger.min.js"></script>
<script src="https://cdn.jsdelivr.net/npm/gsap@3.13.0/dist/ScrollSmoother.min.js"></script>
<script src="https://cdn.jsdelivr.net/npm/gsap@3.13.0/dist/SplitText.min.js"></script>
```

---

### Opção 2: Instalação via NPM (Para Desenvolvimento Local / Bundlers)

Caso deseje transformar o projeto em uma estrutura baseada em Node.js / NPM (usando Vite, Webpack, etc.), siga o passo a passo abaixo:

1. **Inicialize o projeto Node.js**:
   ```bash
   npm init -y
   ```

2. **Instale a biblioteca GSAP**:
   ```bash
   npm install gsap
   ```

3. **Importe as dependências no seu arquivo JavaScript (`main.js`)**:
   ```javascript
   import { gsap } from "gsap";
   import { ScrollTrigger } from "gsap/ScrollTrigger";
   import { ScrollSmoother } from "gsap/ScrollSmoother";
   import { SplitText } from "gsap/SplitText";

   gsap.registerPlugin(ScrollTrigger, ScrollSmoother, SplitText);
   ```

4. **Instale um servidor local leve (ex: `serve`)**:
   ```bash
   npm install -g serve
   ```

---

## 🚀 Como Executar o Projeto

1. **Clonar o Repositório**:
   ```bash
   git clone https://github.com/seu-usuario/homem-aranha-um-novo-dia.git
   ```

2. **Acessar a Pasta do Projeto**:
   ```bash
   cd homem-aranha-um-novo-dia
   ```

3. **Abrir a Aplicação**:
   - **Opção A (VS Code)**: Abra a pasta no VS Code e utilize a extensão **Live Server** clicando em *"Go Live"*.
   - **Opção B (Terminal)**: Execute um servidor local simples com Node.js ou Python:
     ```bash
     npx serve
     ```
     ou
     ```bash
     python -m http.server 8000
     ```

4. Acesse o endereço informado no navegador (geralmente `http://localhost:3000` ou `http://localhost:8000`).

---

## 🤝 Créditos e Agradecimentos

Desenvolvido como projeto de estudo juntamente com os materiais e conteúdos da **WebHub**.

---
*🕷️ "Com grandes poderes vêm grandes responsabilidades."*
