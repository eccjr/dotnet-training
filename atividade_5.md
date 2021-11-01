# Implementação dos métodos PUT e DELETE, e boas práticas

No video a seguir são ensinados os métodos PUT e DELETE, bem como boas práticas na criação de APIs:

https://www.youtube.com/watch?v=v_fJ9PZ4Trc

# Instalação pacote mapper linux

Em certo ponto do vídeo, é instalado um padcote para a utilização do mapper. Para linux, rode o seguinte comando no projeto: 
```
dotnet add package AutoMapper.Extensions.Microsoft.DependencyInjection

```

# DTOs

DTOs são classes de data transfer objects. Eles são úteis pois permitem definir quais parametros queremos receber do usuário (não queremos receber ID por exemplo, já que é controlado pelo banco de dados), bem como retornar parâmetros calculados, (horário da requisição, algum calculo com os dados da api).

A ideia consiste basicamente em agrupar um conjunto de atributos numa classe simples de forma a otimizar a comunicação.

Como DTOs são classes, e possuem seus próprios objetos, na hora de guardá-los no banco de dados, ou exibir dados da api através deles, é preciso fazer uma conversão. 

Para realizar esta conversão, são usados os Mappers.

No vídeo tudo isso é explicado com mais detalhes.

# Atividade

Implemente os métodos PUT e DELETE na api de filmes, bem como DTOs e Mappers.