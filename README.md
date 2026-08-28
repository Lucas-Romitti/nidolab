# Nidolab

### **Autor:** Lucas Romitti Kummer

O **Nidolab** é uma aplicação web desenvolvida com o objetivo de facilitar a criação e organização de times para o jogo **Pokémon Champions**.

A aplicação permite que o usuário pesquise Pokémon, consulte suas informações e monte uma equipe personalizada de até seis integrantes.

O frontend da aplicação será desenvolvido utilizando **HTML, CSS e JavaScript**, com **MaterializeCSS** para a construção da interface e **jQuery** para manipulação do DOM e interatividade.

Para simular a persistência dos dados, será utilizada uma **API Fake com JSON Server**.

---

## 📚 Documentação do Projeto

Para entender o propósito, escopo e estrutura técnica da aplicação, consulte os documentos abaixo:

* [📄 Product Requirements Document (PRD)](./docs/prd.md) — Descrição do sistema, objetivo, atores e histórias de usuário.
* [🛠️ Especificação Técnica](./docs/architecture.md) — Modelo de dados e relacionamentos das entidades da aplicação.
* [🎨 Design System](./docs/design-system.md) — Identidade visual, cores, tipografia e padrões de componentes.
* [🖼️ Protótipo no Figma](#) — Protótipo das principais telas da aplicação.

---

## 🎨 Design

O projeto contará com um Design System próprio para manter a identidade visual consistente entre as páginas e componentes da aplicação.

O protótipo das interfaces será desenvolvido no **Figma**, contemplando as versões:

* 📱 Mobile
* 💻 Desktop

### Protótipo no Figma

*(link será adicionado posteriormente)*

---

## 🌐 Site em Produção

**Ainda em desenvolvimento.**

O projeto será disponibilizado posteriormente por meio do GitHub Pages.

---

## 💻 Tecnologias e Dependências

### Frontend

* **HTML5** — Estrutura das páginas.
* **CSS3** — Estilização complementar.
* **JavaScript** — Lógica e funcionalidades da aplicação.
* **MaterializeCSS** — Framework CSS utilizado para componentes e layout responsivo.
* **jQuery** — Manipulação do DOM, eventos e interatividade.

### Backend / Persistência

* **JSON Server** — Utilizado para simular uma API REST e persistir os dados das equipes.

### Ferramentas de desenvolvimento

* **Node.js**
* **NPM**
* **Git**
* **GitHub**
* **ESLint**
* **Prettier**

---

## 🗂️ Estrutura do Projeto

```text
nidolab/
│
├── docs/
│   ├── prd.md
│   ├── architecture.md
│   └── design-system.md
│
├── src/
│   ├── assets/
│   ├── components/
│   ├── pages/
│   ├── services/
│   ├── styles/
│   ├── utils/
│   └── main.js
│
├── db.json
├── package.json
├── .gitignore
└── README.md
```

A organização poderá ser ajustada durante o desenvolvimento, mantendo o princípio de modularização e separação de responsabilidades.

---

## 🚀 Manual de Execução

### 1. Clonar o repositório

```bash
git clone URL_DO_REPOSITORIO
```

### 2. Acessar o diretório do projeto

```bash
cd nidolab
```

### 3. Instalar as dependências

```bash
npm install
```

### 4. Executar o JSON Server

O JSON Server será utilizado para disponibilizar a API Fake da aplicação.

Caso esteja configurado como script no `package.json`:

```bash
npm run json-server
```

Ou, caso seja necessário executar diretamente:

```bash
npx json-server --watch db.json
```

Por padrão, o servidor será disponibilizado em:

```text
http://localhost:3000
```

### 5. Executar o frontend

O frontend poderá ser executado utilizando a extensão **Live Server** do Visual Studio Code ou outro servidor HTTP local.

---

## 📱 Funcionalidades

As principais funcionalidades previstas para o Nidolab são:

* 🔎 Pesquisa de Pokémon.
* 📋 Visualização das informações dos Pokémon.
* ➕ Adição de Pokémon à equipe.
* ➖ Remoção de Pokémon da equipe.
* 👥 Montagem de equipes com até seis Pokémon.
* 💾 Salvamento de equipes.
* 📂 Visualização de equipes salvas.
* 🗑️ Exclusão de equipes.
* 📱 Interface responsiva para mobile e desktop.

---

## 📝 Checklist | Indicadores de Desempenho

### RA1 — Frameworks CSS e layouts responsivos

* [ ] ID 01 — Protótipo adaptável para mobile e desktop.
* [ ] ID 02 — Layout responsivo utilizando MaterializeCSS.
* [ ] ID 03 — Layout responsivo utilizando CSS puro com Flexbox/Grid.
* [ ] ID 04 — Componentes do MaterializeCSS e componentes JavaScript.
* [ ] ID 05 — Utilização de unidades relativas.
* [ ] ID 06 — Aplicação de Design System.
* [ ] ID 07 — Utilização de Sass/SCSS.
* [ ] ID 08 — Tipografia responsiva ou fluida.
* [ ] ID 09 — Imagens responsivas.
* [ ] ID 10 — Otimização e carregamento adaptativo de imagens.

### RA2 — Formulários e validações

* [ ] ID 11 — Validação HTML nativa.
* [ ] ID 12 — Validações customizadas utilizando REGEX.
* [ ] ID 13 — Utilização de checkbox, radio e select.
* [ ] ID 14 — Utilização de localStorage/sessionStorage.

### RA3 — Ferramentas de desenvolvimento

* [ ] ID 15 — Node.js e NPM.
* [ ] ID 16 — Git/GitHub e `.gitignore`.
* [ ] ID 17 — README.md padronizado.
* [ ] ID 18 — Organização modular dos arquivos.
* [ ] ID 19 — ESLint e Prettier.

### RA4 — Bibliotecas JavaScript

* [ ] ID 20 — Utilização de jQuery.
* [ ] ID 21 — Utilização de plugin jQuery ou biblioteca complementar.

### RA5 — Requisições assíncronas

* [ ] ID 22 — Requisições para API Fake para persistência.
* [ ] ID 23 — Requisições para API Fake para exibição de dados.
* [ ] ID 24 — Requisições para API pública real.

---

## 📌 Status

**Em desenvolvimento.**

O escopo e as funcionalidades poderão ser refinados conforme o desenvolvimento do projeto e os requisitos da disciplina.
