# FilmesAPI

Este é um projeto de API para gerenciamento de informações relacionadas a cinemas e filmes.

## Sobre o Projeto

O projeto **FilmesAPI** é uma API desenvolvida em C# utilizando o framework ASP.NET Core. Ela fornece endpoints para manipular informações sobre cinemas, endereços, filmes, gerentes e sessões.

## Configuração

O arquivo `Startup.cs` contém a configuração da inicialização da aplicação, incluindo a configuração dos serviços, middleware e roteamento.

### Adicionando Serviços

No método `ConfigureServices`, vários serviços são adicionados ao contêiner de injeção de dependência. Alguns destes serviços incluem:

- Configuração do banco de dados através do `AppDbContext` usando o MySQL como provedor.
- Configuração do mapeamento entre objetos de domínio e DTOs utilizando o AutoMapper.
- Adição de serviços relacionados a Cinema, Endereço, Filme, Gerente e Sessão através das classes de serviço correspondentes.

### Configurando o Pipeline de Requisições HTTP

No método `Configure`, o pipeline de requisições HTTP é configurado. Isso inclui:

- Tratamento de exceções em ambiente de desenvolvimento para facilitar a depuração.
- Redirecionamento HTTPS para garantir a segurança das comunicações.
- Definição de roteamento para direcionar as requisições aos controladores corretos.

## Executando o Projeto

Certifique-se de ter o ambiente de desenvolvimento configurado com o SDK do ASP.NET Core e o MySQL instalados. Você pode utilizar o Visual Studio ou a linha de comando para executar o projeto.

### Passos Básicos:

1. Clone este repositório.
2. Abra o projeto no Visual Studio ou utilize o terminal.
3. Verifique e atualize a string de conexão do banco de dados no arquivo `appsettings.json`.
4. Execute o projeto.
5. Acesse os endpoints da API através do navegador ou ferramentas como o Postman.

## Contribuição

Contribuições são bem-vindas! Se você encontrar problemas, tiver sugestões ou melhorias, sinta-se à vontade para abrir uma issue ou enviar um pull request.
