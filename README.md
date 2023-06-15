# Configuração do Projeto

## Inicie um novo projeto Spring Boot utilizando o Spring Initializr.
Certifique-se de selecionar as dependências **Spring WebFlux** e **Spring Data Reactive MongoDB** durante a configuração inicial do projeto.

## Modelagem de Dados
Crie uma classe `News` com os seguintes campos: `id`, `title`, `content`, `author`, `publishDate`, `category`, `viewCount`, `commentList`.

## Camada de Repositório
Crie um repositório, `NewsRepository`, estendendo a interface `ReactiveCrudRepository`.

## Camada de Serviço
Crie uma classe de serviço, `NewsService`, que usa `NewsRepository` para fornecer métodos como `findAllNews`, `findNewsByCategory`, `findNewsByAuthor`, `findNewsByKeyword`.

## Camada de Controlador
Crie um controlador, `NewsController`, que usa `NewsService` para expor endpoints e retornar os dados como um fluxo de eventos Server-Sent Events (SSE).

## Testes
Escreva testes unitários e de integração usando JUnit e Mockito.

## Segurança
Use Spring Security para adicionar autenticação e autorização.

## Filtragem de Notícias
Adicione suporte para filtrar notícias por categorias, autor ou palavra-chave.

## Classificação de Notícias
Implemente um sistema para classificar as notícias com base em critérios específicos (por exemplo, mais recentes, mais lidas, mais comentadas).

## Paginação de Notícias
Utilize `PagingAndSortingRepository` para adicionar suporte a paginação e classificação de dados.

## Sistema de Comentários
Crie uma nova entidade `Comment` com campos como `id`, `newsId`, `author`, `content`, `date`.

## Integração com API externa
Use a API de notícias do NewsAPI.org ou outra API de sua escolha. Use o cliente web reativo do Spring.

## Dockerização
Crie um arquivo Dockerfile na raiz do seu projeto para criar uma imagem Docker da sua aplicação.
