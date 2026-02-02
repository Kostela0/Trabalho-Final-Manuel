🎵 Sistema de Gerenciamento Musical com Relatórios em PDF

Projeto web desenvolvido com Node.js, Express e Sequelize, seguindo a arquitetura MVC, com foco no gerenciamento de artistas, músicas e playlists, além da geração de relatórios em PDF a partir de páginas HTML.

📌 Funcionalidades

Cadastro e listagem de Artistas

Cadastro e listagem de Músicas

Associação entre Artistas e Músicas

Criação e gerenciamento de Playlists

Relatórios em:

📄 HTML (visualização no navegador)

🖨️ PDF (gerados automaticamente com Playwright)

Tema visual escuro inspirado no Spotify

🧱 Arquitetura do Projeto

O projeto utiliza o padrão MVC (Model–View–Controller):

Model: Sequelize + SQLite

View: EJS (HTML dinâmico)

Controller: Express (rotas e regras de negócio)

Essa separação facilita manutenção, organização e escalabilidade.

🛠️ Tecnologias Utilizadas
Backend

Node.js

Express.js

JavaScript (ES Modules)

Banco de Dados

SQLite

Sequelize (ORM)

Frontend

EJS

HTML5

CSS3

Geração de PDF

Playwright

Chromium (headless)

Gerenciamento

NPM

📂 Estrutura de Pastas (simplificada)
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

🖨️ Geração de Relatórios em PDF

Os relatórios em PDF são gerados a partir de views EJS, seguindo o fluxo:

O controller busca os dados no banco (Sequelize)

A view EJS é renderizada em HTML em memória

O Playwright abre um Chromium headless

O HTML é convertido em PDF

O PDF é enviado como resposta HTTP

O processo de geração é centralizado em uma função reutilizável localizada em:

utils/gerarPdf.js


Essa abordagem evita duplicação de código e facilita a manutenção do sistema.

🚀 Como Executar o Projeto
1️⃣ Clonar o repositório
git clone https://github.com/seu-usuario/seu-repositorio.git
cd seu-repositorio

2️⃣ Instalar as dependências
npm install

3️⃣ Instalar os navegadores do Playwright
npx playwright install


Em sistemas Linux, caso necessário:

npx playwright install-deps

4️⃣ Executar o servidor
node server.js


ou

npm run dev

🎓 Objetivo Acadêmico

Este projeto foi desenvolvido com fins educacionais, com o objetivo de aplicar conceitos de:

Desenvolvimento web com Node.js

Arquitetura MVC

ORM e bancos de dados relacionais

Geração automatizada de documentos PDF

Organização e boas práticas de código

👥 Autores

Antonio Hittalo R. P. R. Macêdo

Bento Kauê de Sousa Lima

João Manuel da Silva Paulo

José Nillo Marques Martins

Curso: Análise e Desenvolvimento de Sistemas (ADS)

📄 Licença

Este projeto é de uso acadêmico e livre para fins de estudo.
