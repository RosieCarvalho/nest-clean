# banco de dados

- docker compose
- orm: prisma
- banco de dados isolados para testes 2e2:test\setup-e2e.ts

# armazenamento de imagem

- Cloudflare R2

# nest

- pipes

  - Um intermediário que manipula as requisições antes que cheguem aos controladores / interceptadores para validar dados antes de chegar nos controlers
  - validação de dados: zod

- guards

  - Um mecanismo para proteger rotas com base em determinadas condições.
  - verificar validação de algum arquivo antes de chamar o controler. Usado muito para proteção de rotas autenticadas. uso: //guards

- criando seus proprios decorators: src\infra\auth\current-user-decorator.ts

# o que foi criado

- autenticação jwt

# uteis

- rest client (extensão vs-code)

  - partilha as rotas e testar pelo arquivo client.http

- variaveis ambiente

  - zod + process.env : uso => // configEnv

- cache
  - banco de dados para cache : redis -> src\infra\cache\redis

# estrutura

- mappers
  -convertem uma entidade do formato de uma camada, para o formato de outra camada
  -Os mappers são responsáveis por converter uma entidade de um formato para outro, permitindo que diferentes camadas da aplicação trabalhem com representações diferentes da mesma entidade.

- presenter - usado na camada infra - http
  - O Presenter é responsável por converter informações de um formato para outro
