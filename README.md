DESAFIO GITHUB ACTIONS

Proposta

Implantação Automatizada de uma Aplicação Web ASP.NET Core com Docker e Github Actions

Seu desafio consiste em criar uma aplicação web ASP.NET Core, colocá-la em um container Docker, enviar essa imagem para o Docker Hub e, por fim, 
usar o GitHub Actions para implantar essa aplicação sempre que um novo commit for feito para o repositório do GitHub. Com isso em mente, temos os seguintes passos:

1. Crie uma Aplicação Web ASP.NET Core: pode ser uma aplicação simples de página única ou um Web API que retorne um "Hello, World!".
   
2. Escreva um Dockerfile:

  a. Use a imagem oficial do .NET Core 5 ou 6 como base.

  b. Copie os arquivos do projeto para o container e defina um comando para iniciar a aplicação.

3. Crie uma Imagem Docker:

  a. Navegue até a pasta do projeto e crie a imagem Docker da sua aplicação.

4. Faça o push da imagem para o Docker Hub:

  a. Crie uma conta no Docker Hub (se ainda não tiver uma).
  
  b. Faça o tag da sua imagem Docker.
  
  c. Faça o push da sua imagem Docker para o Docker Hub.

5. Configure o GitHub Actions:

  a. Crie um novo repositório no GitHub para sua aplicação.
  
  b. No seu repositório, vá para a aba "Actions" e configure uma nova ação.
  
  c. Escreva um arquivo .yml para configurar essa ação. O objetivo é que toda vez que um novo código for atualizado no repositório, o GitHub Actions:
    
    i. Crie uma nova imagem Docker.
    
    ii. Faça o push da nova imagem para o Docker Hub.
    
    iii. Opcional: se estiver usando um serviço de hospedagem que suporte Docker (como AWS ECS, Azure Container Instances etc.), 
    configure o GitHub Actions para também atualizar a aplicação hospedada sempre que uma nova imagem for atualizada no Docker Hub
   
6. Teste sua configuração:

  a. Faça algumas mudanças em sua aplicação.
  
  b. Faça o commit das mudanças para o GitHub.
  
  c. Verifique se o GitHub Actions executa conforme o esperado.
  d. Verifique se a nova versão da sua aplicação foi atualizada no Docker Hub (e, se aplicável, no seu serviço de hospedagem)
