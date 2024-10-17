# Projeto Web-Lh Pets - Versão 1

Este projeto é uma aplicação web simples desenvolvida em C#, utilizando .NET 6.0, que gerencia um cadastro de clientes, permitindo visualizar informações sobre pessoas físicas e jurídicas.

## Estrutura do Projeto

- **BIN/**: Contém os arquivos compilados do projeto.
- **OBJ/**: Contém os arquivos temporários e de compilação.
- **PROPERTIES/**: Contém as configurações do projeto.
- **wwwroot/**: Contém arquivos estáticos do projeto.
  - `index.html`: Página inicial que dá as boas-vindas ao usuário.

### Arquivos Principais

- **Banco.cs**: Classe responsável por gerenciar a conexão com o banco de dados e realizar operações relacionadas aos clientes.
- **Clientes.cs**: Classe que define a estrutura de um cliente, incluindo atributos como CPF/CNPJ, nome, endereço, RG/IE, tipo, valor, valor do imposto e total.
- **Program.cs**: Ponto de entrada da aplicação, que configura o servidor web, define as rotas e manipula as requisições.
- **projeto_web_lh_pets_alunos.csproj**: Arquivo de configuração do projeto, que define as dependências e as propriedades do mesmo.
- **vendas.sql**: Script SQL para criação do banco de dados e tabela de clientes, além de inserir dados de exemplo.

## Funcionalidades

- **Cadastro de Clientes**: Permite visualizar a lista de clientes cadastrados, incluindo suas informações e valores de imposto.
- **Visualização da Página Inicial**: O usuário é recebido com uma página de boas-vindas.

## Como Executar

1. **Configurar o Banco de Dados**:
   - Execute o script `vendas.sql` em um servidor SQL para criar o banco de dados e a tabela de clientes.
   
2. **Compilar e Executar**:
   - Clone o repositório.
   - Abra o terminal no diretório do projeto e execute os comandos:
     ```bash
     dotnet build
     dotnet run
     ```
   
3. **Acessar a Aplicação**:
   - Abra um navegador e acesse `http://localhost:5000` para ver a página inicial.
   - Para visualizar a lista de clientes, acesse `http://localhost:5000/listaClientes`.

## Exemplo de Uso

Após a execução da aplicação, o usuário verá a página inicial com a mensagem de boas-vindas. Ao acessar a rota `/listaClientes`, o sistema retornará uma lista formatada de clientes cadastrados, mostrando informações como CPF/CNPJ, nome, endereço, RG/IE, tipo, valor, valor do imposto e total.