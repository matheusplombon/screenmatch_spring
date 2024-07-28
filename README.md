# Screen Match Spring

Este projeto é uma extensão do projeto Screen Match, desenvolvido em Java com Spring para gerenciar filmes e séries, calcular o tempo total de visualização e fornecer recomendações com base nas classificações. Este projeto foi criado para praticar a lógica de programação e a utilização do framework Spring.

## Funcionalidades

- Gerenciamento de filmes e séries
- Cálculo do tempo total de visualização
- Recomendações baseadas em classificações
- Integração com a API OMDB para buscar dados de filmes
- Serialização de dados de filmes em JSON utilizando a biblioteca Gson
- Tratamento de exceções relacionadas à conversão de ano com a classe de exceção personalizada `ErroDeConversaoDeAnoException`

## Tecnologias Utilizadas

- Java
- Spring Framework
- Spring Boot
- API OMDB
- Gson (para serialização JSON)

## Estrutura do Projeto

- **calculos**: Contém classes para cálculos relacionados a filmes e séries.
- **modelos**: Contém classes de modelo para filmes e séries.
- **principal**: Contém classes principais para execução do projeto, incluindo a classe `PrincipalComBusca` para integração com a API OMDB.

## Integração com a API OMDB

A classe `PrincipalComBusca` é responsável por buscar dados de filmes na API OMDB. Para utilizar esta funcionalidade, é necessário configurar a chave da API no arquivo `application.properties`:

```properties
omdb.api.key=SUA_CHAVE_API
