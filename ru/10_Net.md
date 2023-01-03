## Сеть

Попробуйте сделать клиента и сервер, «подергайте» какой-нибудь популярный сайт или открытое API. Тут вы, кстати, вполне можете поэкспериментировать с HTML, CSS и даже с Java(Type)Script. Кто знает, может быть, ваш вариант — стать фуллстек программистом, сочетающим бек и фронт?

```mermaid
flowchart TD

subgraph Net
direction LR
HTTP -.-> requests -.-> websocket -.-> Frameworks -.-> API

subgraph HTTP
direction LR
HTTPS(HTTPS)
CORS(CORS)
end

requests(requests)
websocket(websocket)

subgraph Frameworks
direction LR
Flask(Flask)
aiohttp(aiohttp)
Django(Django)
end

subgraph API
direction LR
REST(REST)
Postman(Postman)
Authentication(Authentication)
jwt_tokens("JWT tokens")
Swagger(Swagger)
FastAPI(FastAPI)
GraphQL(GraphQL)
end

end

classDef trainee fill:#6ADA6A, stroke-width:3px
classDef middle fill:#FF9900, stroke-width:3px

class HTTPS trainee;
class requests trainee;
class websocket trainee;
class Flask trainee;
class REST trainee;
class Postman trainee;

class Django middle;
class FastAPI middle;
class GraphQL middle;
```
