# 🎵 Sistema de Gerenciamento Musical com Relatórios em PDF

Projeto acadêmico desenvolvido no curso de **Análise e Desenvolvimento de Sistemas (ADS)**, 
utilizando **Node.js**, **Express**, **Sequelize** e **SQLite**, seguindo a arquitetura **MVC (Model–View–Controller)**.

O sistema permite o gerenciamento de **artistas, músicas e playlists**, além da geração de 
**relatórios em PDF** a partir de páginas HTML utilizando **Playwright**.

---

## 📌 Funcionalidades

- Cadastro e listagem de **Artistas**
- Cadastro e listagem de **Músicas**
- Associação entre **Artistas e Músicas**
- Criação e gerenciamento de **Playlists**
- Relatórios em:
  - 📄 **HTML** (visualização no navegador)
  - 🖨️ **PDF** (gerados automaticamente)
- Tema visual escuro inspirado no Spotify

---

## 🧱 Arquitetura do Projeto

O projeto utiliza o padrão **MVC (Model–View–Controller)**:

- **Model:** Sequelize + SQLite  
- **View:** EJS (HTML dinâmico)  
- **Controller:** Express (rotas e regras de negócio)

Essa separação facilita a manutenção, organização e escalabilidade do sistema.

---

## 🛠️ Tecnologias Utilizadas

### Backend
- **Node.js**
- **Express.js**
- **JavaScript (ES Modules)**

### Banco de Dados
- **SQLite**
- **Sequelize (ORM)**

### Frontend
- **EJS**
- **HTML5**
- **CSS3**

### Geração de PDF
- **Playwright**
- **Chromium (headless)**

### Gerenciamento
- **NPM**

---

## 📂 Estrutura de Pastas (simplificada)

```text
├── controller/
│   ├── artista.controller.js
│   ├── musica.controller.js
│   └── playlist.controller.js
│
├── models/
│   ├── Artista.js
│   ├── Musica.js
│   ├── Playlist.js
│   └── index.js
│
├── views/
│   ├── amigos/
│   │   └── relatorioArtistas.ejs
│   ├── jogos/
│   ├── emprestimos/
│   └── relatorios/
│
├── utils/
│   └── gerarPdf.js
│
├── public/
│   ├── css/
│   └── img/
│
├── database-dev.sqlite
├── server.js
├── package.json
└── README.md
```

## 🚀 Como Executar o Projeto
## 1️⃣ Clonar o repositório
- git clone https://github.com/seu-usuario/seu-repositorio.git
- cd seu-repositorio

## 2️⃣ Instalar as dependências
- npm install

## 3️⃣ Instalar os navegadores do Playwright
- npm i playwright
- npx playwright install

## 4️⃣ Executar o servidor
- node server.js

## 🎓 Objetivo Acadêmico
Este projeto foi desenvolvido com fins educacionais, com o objetivo de aplicar conceitos de:
- Desenvolvimento web com Node.js
- Arquitetura MVC
- ORM e bancos de dados relacionais
- Geração automatizada de documentos PDF
- Organização e boas práticas de programação

## 👥 Autores
- Antonio Hittalo R. P. R. Macêdo
- Bento Kauê de Sousa Lima
- João Manuel da Silva Paulo
- José Nillo Marques Martins
🎓 **Curso**: Análise e Desenvolvimento de Sistemas (ADS)
