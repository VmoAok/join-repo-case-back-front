🛍️ Cosméticos Jiki - Backend & Frontend

Este repositório contém o backend e frontend do projeto Jiki Skin, uma plataforma para gerenciar pedidos e produtos cosméticos.
  Jiki 

🏗️ Backend (backend-jikicosmeticos)

🔹 Funcionalidades
1. 🔑 Autenticação e Autorização
   - Implementada via JWT, com geração e validação de tokens (`TokenConfig`).  
   - Endpoints de login e registro em `AuthController`.

2. 👤 Cadastro e Atualização de Usuário  
   - Cadastro de novos usuários e atualização de dados via `CadastroUsuarioController`.  
   - Entidade principal: `Usuario`, DTO: `CadastroDTO`.

3. 📦 Gestão de Produtos
   - CRUD de produtos via REST API, conforme especificado no `swagger.yaml`.  
   - Entidades: `Product` e `Estoque`.

4. 🛒 Gestão de Pedidos 
   - Criar, consultar e atualizar pedidos de compra (`Pedido`).  

5. 📧 Envio de E-mails
   - Serviço para confirmação de cadastro via `EmailServices`.  

6. 📄 Documentação da API
   - Swagger/OpenAPI disponível (`SwaggerConfig`).  

7. ✅ Testes Automatizados
   - Testes unitários e de integração (`AuthControllerTest`, `ProductTest`).  

💻 Frontend (node-js-cosmeticos-jiki)

🔹 Funcionalidades
1. 🏠 Página Inicial
   - Exibe produtos em destaque, banners e categorias (`pages/index.js`).  

2. 🎯 Navegação por Categorias
   - Usuário pode filtrar produtos (`Categories`).  

3. 🛍️ Página de Produtos
   - Lista todos os produtos (`pages/produtos.js`).  

4. 🔑 Página de Login
   - Autenticação via `/auth/login` (`pages/login.js`).  

5. 🎨 Estilização
   - CSS Modules para design (`styles/Categories.module.css`).  

6. 🔄 Integração com Backend
   - Uso de `axios` para requisições HTTP.  

7. ⚙️ Configuração de Ambiente
   - Variáveis `.env.local` para configuração.  


🔗 Como os módulos se conectam?
✔️ O frontend consome a API REST do **backend** para autenticação, cadastro, listagem de produtos e pedidos.  
✔️ O backend gerencia autenticação, persistência de dados, regras de negócio e envio de e-mails.  
✔️ O Swagger/OpenAPI permite testar e documentar os endpoints.  
✔️ Testes automatizados garantem a qualidade das principais funcionalidades do backend.



🚀 Como rodar o projeto?

1️⃣ Clone este repositório:

bash
  git clone https://github.com/seu-usuario/cosmeticos-jiki.git
  
2️⃣ Acesse a pasta do backend:
bash
  cd backend-jikicosmeticos
  
3️⃣ Execute com Docker - 🐳
  docker compose up -d

6️⃣ Acesse http://localhost:3000 no navegador! 🎉

📬 Contato Caso tenha dúvidas ou sugestões, entre em contato: 📧 Email: oliveiravmss@gmail.com 🔗 LinkedIn: https://www.linkedin.com/in/vit%C3%B3ria-oliveira-758949159/)

