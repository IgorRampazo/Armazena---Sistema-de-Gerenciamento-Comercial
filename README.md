********** 📘 Trabalho Bimestral – Aplicação Web com Cadastros **********

#------> Armazena---Sistema-de-Gerenciamento-Comercial <------#

### ? Estrutura do Projeto ? ###

🗂️ Projeto
|
├── 🔒 Private                   // Páginas acessadas somente mediante login
|   |
│   ├── 🖼️ assets                // Recursos privados (imagens, etc.)
│   └── 📁 cadastro              // Módulos de cadastro restritos
|       |
│       ├── 👤 Clientes
│       ├── 🏢 Fornecedores
│       ├── 🚚 Entregador
│       ├── 🏷️ Categoria
│       └── 📦 Produto
|
├── 🌐 public                    // Páginas e recursos públicos
|   |
│   ├── 🖼️ assets                // Recursos públicos (imagens, etc.)
│   ├── 📝 CadastroCliente       // Cadastro aberto de clientes
│   └── 🔑 Login                 // Tela de login
|
├── 🛡️ security                  // Segurança e autenticação
|   |
│   ├── 🗝️ Auth                  // Lógica de autenticação (login, logout e verificação de sessão)
│   └── 🧱 AuthMiddleware        // Middleware de autenticação (bloqueio / permissão de acesso às páginas privadas)
|
├── ⚙️ app                       // Arquivo principal do servidor Node.js
└── 📦 package                   // Configurações e dependências do projeto

___________________________________________________________________________________________________________________

🧱 Estrutura da Aplicação

#-------------------------------------------------------------------------------------#
🧩 Página                            🔓 Acesso    🎯 Função Principal
#-------------------------------------------------------------------------------------#
🏠 Vitrine de Produtos               Pública       Exibir produtos para visitantes
🔐 Login                             Pública       Autenticar usuário no sistema
👤 Cadastro de Cliente               Privada       Cadastrar clientes
📦 Cadastro de Produto               Privada       Cadastrar produtos
🏭 Cadastro de Fornecedor            Privada       Cadastrar fornecedores
🚚 Cadastro de Entregador            Privada       Cadastrar entregadores
🗂️ Cadastro de Categorias            Privada       Cadastrar categorias de produtos
👥 Cadastro de Usuários do Sistema   Privada       Criar contas de usuários
#-------------------------------------------------------------------------------------#

___________________________________________________________________________________________________________________

✅ Requisitos Técnicos

- 🔐 Autenticação com **cookies/sessão HTTP**
- 🚫 Validação: **sem campos vazios**
- 🗃️ Dados gerenciados via **JSON-SERVER**
- 🧭 Menu de navegação com opção de **Logout**
- 🌍 Páginas públicas: **Login** e **Vitrine de Produtos**
- 🔒 Demais páginas: **acesso restrito a usuários logados**
- 👥 Uso de **Git + GitHub**
