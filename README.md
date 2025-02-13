<div> 
<p><a href="https://github.com/JosiTubaroski/WEB-API-com-.NET-8-e-SQL-Server">Home</a></p>
</div> 

# WEB API com .NET 8 e SQL-Server

### Criando o Projeto

1) Criando um projeto no Visual Studio 2022

<img src="https://github.com/JosiTubaroski/WEB-API-com-.NET-8-e-SQL-Server/blob/main/img/01_Criar_Projeto.png"/>

2) Criar um projeto: API Web do ASP.NET Core

<img src="https://github.com/JosiTubaroski/WEB-API-com-.NET-8-e-SQL-Server/blob/main/img/02_API_WEB.png"/>

- Repositório do Código C:\Users\josiq\source\repos

<img src="https://github.com/JosiTubaroski/WEB-API-com-.NET-8-e-SQL-Server/blob/main/img/03_Nome_Projeto.png"/>

3) Criar Projeto

<img src="https://github.com/JosiTubaroski/WEB-API-com-.NET-8-e-SQL-Server/blob/main/img/04_Estrutura_Projeto.png"/>

4) Estrutura Projeto

<img src="https://github.com/JosiTubaroski/WEB-API-com-.NET-8-e-SQL-Server/blob/main/img/05_Pastas_Projetos.png"/>

### Como funciona a estrutura de projetos Web-API .Net8?

A estrutura de um projeto Web API em .NET 8 é organizada de forma modular e segue boas práticas para garantir a escabilidade, manutenção e clareza de código. Vamos explorar como essa estrutura funciona, os principais componentes e como eles se integram:

### Estrutura Básica de um Projeto Web API .NET 8

Quando você cria um projeto Web API no .NET 8 (usando o Visual Studio, Visual Studio Code ou CLI do .NET), a estrutura inicial é gerada automaticamente. Aqui está uma visão geral dos principais componentes:

### 1. Pasta Controllers:

- Contém os controladores da API, que são classes que lidam com requisições HTTP.
- Cada controlador geralmente corresponde a um recurso da API (ex.: ProdutosController, UsuariosController).

<img src="https://github.com/JosiTubaroski/WEB-API-com-.NET-8-e-SQL-Server/blob/main/img/Estrutura/01_Controler_Exemplo.png"/>

### 2. Pasta Models:

- Contém as classes que representam os dados da aplicação (entidades).
- Essas classes são usadas para mapear objetos para o banco de dados (Entity Framework) ou para serializar/deserializar dados JSON.

<img src="https://github.com/JosiTubaroski/WEB-API-com-.NET-8-e-SQL-Server/blob/main/img/Estrutura/02_Models_Exemplo.png"/>

### 3. Pasta Data:

- Contém classes relacionadas ao acesso a dados, como o DbContext do Entity Framework.

<img src="https://github.com/JosiTubaroski/WEB-API-com-.NET-8-e-SQL-Server/blob/main/img/Estrutura/03_Data_Exemplo.png"/>

### 4. Pasta Service:

- Contém classes de serviço que encapsulam a lógica de negócios da aplicação.
- Esses serviços são injetados nos controladores via injeção de dependência.

<img src="https://github.com/JosiTubaroski/WEB-API-com-.NET-8-e-SQL-Server/blob/main/img/Estrutura/04_Services_Exemplo.png"/>

### 5. Pasta Migrations (se usar Entity Framework):

- Contém as migrações do banco de dados, que são usadas para criar e atualizar o esquema do banco de dados.

<img src="https://github.com/JosiTubaroski/WEB-API-com-.NET-8-e-SQL-Server/blob/main/img/Estrutura/05_Migrations_Exemplo.png"/>

### 6. Arquivo Program.cs:

- É o ponto de entrada da aplicação, onde os serviços e middlewares são configurados.
- No .NET 6 em diante, o Program.cs substitui o Startup.cs em versões anteriores.

<img src="https://github.com/JosiTubaroski/WEB-API-com-.NET-8-e-SQL-Server/blob/main/img/Estrutura/06_Programs_Exemplo.png"/>

### 7. Arquivo appsettings.json:

- Contém configurações da aplicação, como strings de conexão com o banco de dados, chaves de API, etc.

<img src="https://github.com/JosiTubaroski/WEB-API-com-.NET-8-e-SQL-Server/blob/main/img/Estrutura/07_Settings_Json.png"/>

### 8. Pasta Properties:

- Contém o arquivo launchSettings.json, que define configurações de execução da aplicação, como URLs e ambientes.

<img src="https://github.com/JosiTubaroski/WEB-API-com-.NET-8-e-SQL-Server/blob/main/img/Estrutura/08_Propertis.png"/>

### Fluxo de Funcionamento

#### 1. Requisição HTTP:

- O cliente (navegador, aplicativo móvel, etc.) faz uma requisição HTTP para a API (ex.: GET /api/produtos).

#### 2. Roteamento:

- O roteamento do ASP.NET Core mapeia a requisição para o controlador e método apropriados (ex.: ProdutosController.Get).

#### 3. Processamento no Controlador:

- O controlador recebe a requisição, pode chamar serviços para processar a lógica de negócios e retorna uma resposta HTTP.

#### 4. Resposta HTTP:

- A resposta é enviada de volta ao cliente, geralmente no formato JSON.

## Conclusão

A estrutura de um projeto Web API .NET 8 é organizada para promover a separação de responsabilidades, facilitando a manutenção e a escalabilidade. Os principais componentes incluem controladores, modelos, serviços, acesso a dados e a escalabilidade. Os principais componentes incluem controladores, modelos, serviços, acesso a dados e configurações. Seguindo essa estrutura.

## Como é a hierarquia de um projeto .NET8?

A hierarquia de um projeto .NET8 é organizada de forma modular e segue boas praticas para garantir a clareza, manutenção e escalabilidade do código. A estrutura pode variar dependendo do tipo de projeto (Web API, MVC, Console, etc.), mas, em geral, segue um padrão comum. Vamos explorar a hierarquia típica de um projeto Web API em .NET 8:

## Estrutura de Pastas e Arquivos

Aqui está a hierarquia comum de um projeto Web API .NET 8:

<img src="https://github.com/JosiTubaroski/WEB-API-com-.NET-8-e-SQL-Server/blob/main/img/Estrutura/09_Hierarquia.png"/>
