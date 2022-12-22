## Net

Try to create a client and a server, poke some popular website or an open API. Here you might as well experiment with HTML, CSS, and even Java(Type)Script. Who knows, perhaps your choice would be to become a full-stack programmer, combining back- and frontend development.

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
