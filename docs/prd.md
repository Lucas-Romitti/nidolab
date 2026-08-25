# Nidolab — Pokémon Team Builder

## 1. Identificação

**Nome:** Lucas Romitti Kummer
**Projeto:** Nidolab
**Tema:** Sistema web para criação e gerenciamento de equipes de Pokémon

---

## 2. Descrição

O **Nidolab** é uma aplicação web que permite aos usuários pesquisar Pokémon, consultar suas principais informações e montar equipes personalizadas de até seis integrantes.

O sistema tem como objetivo facilitar a criação e organização de equipes de Pokémon em uma interface simples, responsiva e interativa. As informações dos Pokémon serão obtidas dinamicamente por meio de uma API pública, enquanto as equipes criadas pelos usuários poderão ser persistidas por meio de uma API fake.

Além da montagem das equipes, a aplicação contará com recursos de validação de formulários, armazenamento local e integração com APIs externas, proporcionando uma experiência dinâmica ao usuário.

O projeto também busca aplicar boas práticas de desenvolvimento web, como organização modular do código, versionamento, padronização, responsividade e utilização de frameworks e bibliotecas JavaScript.

### Problema que o sistema resolve

A criação de uma equipe de Pokémon pode exigir que o usuário pesquise individualmente informações sobre diferentes Pokémon e organize manualmente suas escolhas. O sistema centraliza esse processo em uma única aplicação, permitindo pesquisar, visualizar, selecionar, organizar e salvar uma equipe de maneira rápida e prática.

---

## 3. Objetivos

### Objetivo geral

Desenvolver uma aplicação web responsiva que permita aos usuários pesquisar Pokémon e montar, visualizar e gerenciar equipes personalizadas de até seis integrantes.

### Objetivos específicos

* Permitir a pesquisa de Pokémon por nome ou número.
* Exibir informações dos Pokémon de forma organizada.
* Permitir adicionar e remover Pokémon de uma equipe.
* Limitar uma equipe a no máximo seis Pokémon.
* Permitir salvar equipes personalizadas.
* Permitir visualizar e excluir equipes salvas.
* Utilizar APIs para obtenção e persistência de dados.
* Integrar uma API pública adicional para demonstrar consumo de serviços externos.
* Oferecer uma interface responsiva para dispositivos mobile e desktop.
* Aplicar validações no lado cliente.
* Aplicar boas práticas de organização e desenvolvimento de software.

---

## 4. Atores do Sistema

### 4.1 Visitante

Usuário que acessa a aplicação sem necessidade de autenticação.

**Principais ações:**

* Acessar a página inicial.
* Pesquisar Pokémon.
* Visualizar informações dos Pokémon.
* Montar uma equipe.
* Adicionar e remover Pokémon.
* Consultar informações externas disponibilizadas pela aplicação.

### 4.2 Usuário

Visitante que utiliza as funcionalidades de gerenciamento de equipes.

**Principais ações:**

* Todas as ações do visitante.
* Nomear uma equipe.
* Salvar uma equipe.
* Visualizar equipes salvas.
* Excluir equipes.
* Armazenar preferências ou informações localmente.

> **Observação:** A primeira versão do sistema não terá necessariamente um mecanismo de autenticação. O termo "Usuário" representa o ator que utiliza as funcionalidades de gerenciamento da aplicação.

---

# 5. Histórias de Usuário — Escopo

## 5.1 Pesquisa e consulta de Pokémon

### US01 — Acessar a aplicação

**Como Visitante, eu quero acessar uma página inicial responsiva, para que eu possa utilizar o sistema tanto em dispositivos móveis quanto em computadores.**

### US02 — Pesquisar Pokémon

**Como Visitante, eu quero pesquisar um Pokémon pelo nome ou número, para que eu possa encontrar rapidamente o Pokémon que desejo utilizar na minha equipe.**

### US03 — Visualizar Pokémon

**Como Visitante, eu quero visualizar os Pokémon encontrados em cards com suas principais informações, para que eu possa comparar e escolher quais Pokémon adicionar à minha equipe.**

### US04 — Consultar detalhes

**Como Visitante, eu quero visualizar detalhes de um Pokémon em uma janela de informações, para que eu possa consultar suas características sem precisar sair da página de montagem da equipe.**

### US05 — Tratar erros de consulta

**Como Visitante, eu quero receber uma mensagem quando não for possível consultar os dados de um Pokémon, para que eu saiba que ocorreu um problema e possa tentar novamente.**

---

## 5.2 Montagem da equipe

### US06 — Adicionar Pokémon

**Como Visitante, eu quero adicionar um Pokémon à minha equipe, para que eu possa construir uma composição personalizada.**

### US07 — Remover Pokémon

**Como Visitante, eu quero remover um Pokémon da minha equipe, para que eu possa alterar minha composição quando desejar.**

### US08 — Limitar o tamanho da equipe

**Como Visitante, eu quero ser informado quando tentar adicionar mais de seis Pokémon, para que eu saiba que uma equipe possui no máximo seis integrantes.**

### US09 — Visualizar equipe

**Como Visitante, eu quero visualizar os Pokémon selecionados em uma área dedicada à minha equipe, para que eu possa acompanhar minha composição durante a montagem.**

### US10 — Receber feedback das ações

**Como Visitante, eu quero receber um feedback visual ao adicionar ou remover um Pokémon, para que eu saiba que minha ação foi realizada com sucesso.**

---

## 5.3 Gerenciamento de equipes

### US11 — Nomear equipe

**Como Usuário, eu quero informar um nome para minha equipe, para que eu possa identificar facilmente a composição criada.**

### US12 — Salvar equipe

**Como Usuário, eu quero salvar minha equipe, para que eu possa manter minha composição registrada e consultá-la posteriormente.**

### US13 — Visualizar equipes salvas

**Como Usuário, eu quero visualizar minhas equipes salvas, para que eu possa recuperar e consultar composições criadas anteriormente.**

### US14 — Excluir equipe

**Como Usuário, eu quero excluir uma equipe salva, para que eu possa remover composições que não desejo mais manter.**

### US15 — Confirmar exclusão

**Como Usuário, eu quero receber uma confirmação antes de excluir uma equipe, para que eu possa evitar a remoção acidental de uma composição.**

---

## 5.4 Formulários e informações adicionais

### US16 — Preencher dados da equipe

**Como Usuário, eu quero preencher informações adicionais sobre minha equipe, para que eu possa registrar características e preferências relacionadas à composição.**

### US17 — Escolher características

**Como Usuário, eu quero selecionar opções como geração e estilo de jogo por meio de campos de seleção, para que eu possa categorizar minha equipe.**

### US18 — Validar informações

**Como Usuário, eu quero receber mensagens de erro quando preencher informações inválidas ou deixar campos obrigatórios vazios, para que eu possa corrigir os dados antes de salvar a equipe.**

### US19 — Consultar CEP

**Como Usuário, eu quero informar meu CEP para consultar automaticamente minha cidade e estado, para que eu possa preencher os dados de localização de maneira mais rápida.**

### US20 — Tratar erros de APIs externas

**Como Usuário, eu quero receber uma mensagem adequada quando uma API externa estiver indisponível ou retornar um erro, para que eu saiba que a consulta não pôde ser concluída.**

---

## 5.5 Persistência local e experiência do usuário

### US21 — Manter informações localmente

**Como Usuário, eu quero que determinadas informações da minha utilização sejam armazenadas localmente, para que eu não precise preenchê-las novamente durante novas sessões.**

### US22 — Utilizar a aplicação em diferentes dispositivos

**Como Visitante, eu quero utilizar o sistema em diferentes tamanhos de tela, para que a montagem da minha equipe seja confortável tanto no celular quanto no computador.**

### US23 — Visualizar imagens adequadamente

**Como Visitante, eu quero visualizar as imagens dos Pokémon de forma adaptada ao tamanho dos componentes, para que elas não fiquem distorcidas ou ultrapassem os limites da interface.**

---

# 6. Escopo Funcional

A primeira versão do sistema deverá contemplar:

1. Página inicial responsiva.
2. Pesquisa de Pokémon.
3. Consumo de API pública para obtenção dos dados.
4. Exibição dos Pokémon em cards.
5. Visualização de detalhes.
6. Adição de Pokémon à equipe.
7. Remoção de Pokémon da equipe.
8. Limite de seis Pokémon por equipe.
9. Formulário para identificação e configuração da equipe.
10. Validação dos dados do formulário.
11. Persistência das equipes por meio de uma API fake.
12. Listagem das equipes salvas.
13. Exclusão de equipes.
14. Persistência de informações selecionadas no Web Storage.
15. Consulta de CEP por API pública.
16. Tratamento de erros das requisições.
17. Interface adaptável para mobile e desktop.

---

# 7. Escopo Técnico Relacionado às Funcionalidades

Para viabilizar as histórias de usuário, o projeto deverá utilizar recursos de desenvolvimento web como:

* Framework CSS para construção de layouts responsivos.
* Flexbox e/ou CSS Grid.
* Componentes de interface reutilizáveis.
* Sass/SCSS para organização dos estilos.
* Design System com cores, tipografia e componentes padronizados.
* Tipografia responsiva ou fluida.
* Imagens responsivas e formatos modernos.
* Validação nativa e customizada de formulários.
* Expressões regulares para validações específicas.
* Web Storage para persistência local.
* Node.js e NPM para gerenciamento do projeto.
* Git/GitHub para versionamento.
* ESLint e Prettier para padronização do código.
* jQuery para manipulação do DOM e interações.
* Plugin ou biblioteca JavaScript complementar.
* API fake para persistência e consulta das equipes.
* APIs públicas para obtenção de informações externas.

---

# 8. Fora do Escopo

Para manter o projeto adequado ao escopo acadêmico, não fazem parte da primeira versão:

* Sistema completo de autenticação e recuperação de senha.
* Sistema de pagamentos.
* Aplicativo mobile nativo.
* Batalhas entre jogadores em tempo real.
* Inteligência artificial para criação automática de equipes.
* Sistema multiplayer.
* Banco de dados de produção.
* Sistema competitivo ou ranking global.

Essas funcionalidades poderão ser consideradas como possíveis evoluções futuras do projeto.

---

# 9. Resultado Esperado

Ao final do projeto, espera-se disponibilizar uma aplicação web na qual o usuário possa **pesquisar Pokémon, consultar suas informações, montar uma equipe de até seis integrantes, salvar suas composições e gerenciá-las posteriormente**, utilizando uma interface responsiva e consistente.

O sistema deverá demonstrar, além da funcionalidade de Team Building, a aplicação prática dos conceitos técnicos exigidos na disciplina, especialmente **responsividade, formulários, validação, Web Storage, consumo de APIs, manipulação do DOM, bibliotecas JavaScript, organização de código e boas práticas de desenvolvimento web**.
