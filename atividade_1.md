# Instalando e criando o primeiro projeto

Nessa atividade vamos primeiramente instalar o dotnet para poder criar um projeto básico de api.

## 1. Instalação

Para instalar no Windows, vá no link https://dotnet.microsoft.com/download, clique em "Baixar .NET Core SDK x64" para baixar e apenas instale o SDK normalmente.

No linux, a alternativa mais fácil para instalar o .NET é usando o Snap ("Snapcraft"), um gerenciador de pacotes universal.

Apenas rode o seguinte comando como usuário comum (não root/sudo):

```sh
snap install dotnet-sdk --classic --channel=latest/edge
```

Para verificar se o .NET foi instalado corretamente, rode o comando:

```sh
dotnet --version
```

## 2. Criar um projeto de API

Com o .NET instalado, para criar um projeto, basta rodar o seguinte comando:

```sh
dotnet new webapi -o NomeDoProjeto
```

## 3. Rodando os testes

Testes são scripts automatizados que verificam se o seu projeto está funcionado conforme o esperado. A maioria dos testes funciona inserindo um dado e esperando um valor de retorno. Caso o valor de retorno seja o esperado, o teste encerra com sucesso, caso contrário, ele envia um erro.

É responsabilidade do desenvolvedor criar testes que garantem o funcionamento correto do seu código e que evitam que alguem faça alguma alteração que quebre alguma feature ou o sistema inteiro. Ou seja, desenvolvedores estão sempre rodando os testes antes ou depois de fazerem alterações no código para terem certeza de que está tudo funcionando conforme o esperado.

Para rodar testes em um ambiente .NET Core, basta rodar o seguinte comando:

```sh
dotnet test
```

## 4. Rodando o projeto

O projeto básico criado com o comando `dotnet new webapi` já possui um exemplo de endpoint implementando nomeado WeatherForecast.

Para rodar o projeto, execute o comando:

```sh
dotnet run
```

E acesse o link no seu navegador http://localhost:5000/WeatherForecast

Obs: como o projeto redireciona para a opção em HTTPS, você precisará clicar em "Aceitar os riscos" para poder acessar o endpoint.

Será exibido um JSON com dados de temperatura aleatórios para os próximos 5 dias.

Outra feature interessante é o Swagger, que é uma documentação interativa da API gerada automaticamente.

Para acessá-la, entre no link http://localhost:5000/swagger/index.html. Ela deve mostrar os detalhes do endpoint WeatherForecast.

## Link do tutorial incial da documentação

https://docs.microsoft.com/en-us/aspnet/core/tutorials/first-web-api?view=aspnetcore-5.0&tabs=visual-studio

## Extra: TDD

TDD ou Test-driven Development é um processo de desenvolvimento de software que consiste em escrever o teste antes do código a ser desenvolvido, com o objetivo programar de forma mais eficiente.

O vídeo a seguir explica um pouco mais sobre o assunto:

https://www.youtube.com/watch?v=bLdEypr2e-8
