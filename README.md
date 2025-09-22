# Projeto: Trabalhando com ASP.NET Minimal APIs

Este projeto é um guia prático e abrangente para o desenvolvimento de APIs RESTful usando a abordagem **Minimal APIs do ASP.NET Core**. Ele foi estruturado para demonstrar, passo a passo, a construção de uma aplicação desde a sua criação até a implementação de funcionalidades avançadas como autenticação, autorização e testes.

## 🌟 O que o Projeto Aborda

### 1. Introdução
Uma visão geral sobre as Minimal APIs, seus benefícios e por que são uma excelente escolha para construir microsserviços e APIs leves.

### 2. O que precisa ter instalado para começar
- [SDK do .NET](https://dotnet.microsoft.com/download) (versão 6.0 ou superior)
- Um editor de código (como [Visual Studio Code](https://code.visualstudio.com/) ou [Visual Studio](https://visualstudio.microsoft.com/))
- [Git](https://git-scm.com/downloads) para controle de versão

### 3. Criando projeto e entendendo o código do boilerplate
- Instruções para criar o projeto via linha de comando (`dotnet new web`)
- Explicação do código inicial gerado no arquivo `Program.cs`.

### 4. Definição do que teremos no projeto
- Implementação de uma API para gerenciamento de veículos.

### 5. Criando uma rota login para validação em memória
- Endpoint `POST /login` para autenticação com credenciais em memória.

### 6. Configurando o projeto com Entity Framework e tabela de administradores
- Instalação dos pacotes do Entity Framework.
- Configuração do `DbContext` e criação do modelo `Administrador`.
- Criação e aplicação de migrações para o banco de dados.

### 7. Criando Seed para cadastrar administrador padrão
- Lógica para popular a tabela de administradores com um usuário padrão na inicialização da aplicação.

### 8. Validando administrador com login e senha no banco de dados
- Refatoração do endpoint `/login` para verificar credenciais no banco de dados.

### 9. Configurando modelo de veículos
- Definição do modelo `Veiculo` e suas propriedades.
- Adição da tabela `Veiculos` ao `DbContext`.

### 10. Configurando Swagger na aplicação
- Instalação do [Swashbuckle](https://www.nuget.org/packages/Swashbuckle.AspNetCore/).
- Configuração do Swagger para gerar a documentação da API.

### 11. Criando rota Home respondendo por JSON
- Exemplo de um endpoint simples que retorna um JSON.

### 12. POST para criar veículo
- Endpoint `POST /veiculos` para adicionar um novo veículo ao banco de dados.

### 13. GET para retornar os veículos
- Endpoint `GET /veiculos` para listar todos os veículos cadastrados.

### 14. Organizando rotas por contexto no Swagger
- Uso de `WithOpenApi()` e `tags` para agrupar endpoints no Swagger UI.

### 15. GET para retornar um veículo
- Endpoint `GET /veiculos/{id}` para buscar um veículo específico por seu ID.

### 16. PUT para atualizar veículo
- Endpoint `PUT /veiculos/{id}` para atualizar as informações de um veículo existente.

### 17. DELETE para apagar veículo
- Endpoint `DELETE /veiculos/{id}` para remover um veículo do banco de dados.

### 18. Criando validação ao cadastrar e atualizar veículo
- Implementação de validações (via data annotations ou FluentValidation) para os modelos.

### 19. Criando endpoints para administrador
- Endpoints específicos para gerenciamento de administradores.

### 20. Configurando token JWT no projeto
- Instalação e configuração do JWT Bearer Authentication.

### 21. Configurando Swagger para a passagem de token JWT
- Adição de um campo para autenticação via token no Swagger UI.

### 22. Criando autorização com perfil de Adm e Editor
- Uso de políticas de autorização baseadas em _claims_ para restringir o acesso a endpoints.

### 23. Refatorando projeto criando sln e projeto de test
- Reorganização do código em uma _solution_ com projetos separados (`API` e `Tests`).

### 24. Criando teste de unidade para o modelo de Administrador
- Implementação de testes de unidade para a lógica do modelo de `Administrador`.

### 25. Testes de Persistência
- Testes para garantir que as operações com o Entity Framework funcionam como esperado.

### 26. Criando testes de request
- Testes de integração para verificar o comportamento dos endpoints HTTP.

### 27. Fazendo deploy da aplicação
- Instruções básicas para realizar o _deploy_ em um ambiente como Azure, AWS ou outro provedor.
