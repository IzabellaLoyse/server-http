## HTTP - Hypertext Transfer Protocol

- HTTP é um protocolo de transferência que possibilita que as pessoas que
  inserem a URL do seu site na Web possam ver os conteúdos e dados que nele existem

### Request -> Requisição

- Requisições **HTTP** são mensagens enviadas pelo cliente para iniciar uma ação
  no servidor

- Solicitando um serviço

#### URL/endpoint

- Identificação de recursos

#### Query Params

- Parâmetros na URL

**https://mywebsite.com/products?page=3&orderBy=name**

- **https://mywebsite.com** => URL
- **/products** => Endpoint
- **?page=3&orderBy=name** => Query Params

#### Headers

- Informações adicionais entre cliente e servidor
- Existem headers pré definidos porém também podemos criar headers customizados
- Nome e valor separados por dois pontos `Content-Type: application/json`
- Case Insensitive: `content-type: application/json` `authorization: Bearer usertoken`
- Custom Headers (sempre começam com X): `X-Org-ID: 4485`

#### Body

- Corpo da mensagem
- Apenas para requisições do tipo **POST** e **PUT**

#### Methods (Verbs)

- Indetificação de ação
- **GET**: consulta de dados
- **POST**: criação de registros
- **DELETE**: deleção de registros
- **PUT**: alteração de registros

### Response -> Resposta

- Resposta de uma chamada HTTP( chamada da request)

#### Headers

- Informações adicionais entre cliente e servidor

#### Content Type

- Tipo de conteúdo da resposta

#### Status Code

- Indica o que aconteceu com a **request**

- **100**: Respostas de informação
- **200**: Este é o melhor tipo de código de status HTTP a receber. Uma resposta de
  200 níveis significa que tudo está funcionando exatamente como deveria.
- **400**: No nível 400, os códigos de status HTTP começam a se tornar problemáticos.
  Estes são códigos de erro que especificam que existe uma falha no seu browser
  e/ou pedido.
- **500**: Erros do servidor

#### Principais Status Code

- **200**: OK
- **201**: Created
- **204**: No Content
- **204**:400: Bad Request
- **401/403**: Unauthorized
- **404**: Not Found
- **405**: Method Not Allowed
- **409**: Conflict
- **500**: Internal Server Error

#### Body

- Dados que foram requisitados

## API - Application Programming Interface

- **API** é um conjunto de normas que possibilita a comunicação entre plataformas
  através de uma série de padrões e protocolos

## API REST

- **REST**: Representational State Transfer
- Um padrão para construção de APIs
- Usa o protocolo HTTP
- Retorna uma apresentação do estado

### Nomes de Endpoints

- Nomes dos endpoints em maiúsculo
- GET `/products`
- GET `/products/10`
- POST `/products`
- PUT `/products/10`
- DELETE `/products/10`

### Representação do Estado

- Representação de Estado utilizando JSON

## API RESTFULL

- Documetação de como deve se implementar uma API REST
- Aplicação dos padrões REST
