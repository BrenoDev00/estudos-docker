# Docker Compose
- é uma ferramente para definir e executar múltiplos containers Docker ao mesmo tempo usando um único arquivo de configuração.

# docker-compose.yml
- arquivo que define toda a infraestrutura Docker de um projeto.

# services
- no Compose, tudo gira em torno de services.
- um service representa um container que executa uma responsabilidade.
- exemplo:
 services:
    frontend:
    backend:
    database:
    redis:
cada um vira um container separado.

# comandos
- subir containers: docker compose up -d(roda em background)
- parar containers: docker compose down
- visualizar logs: docker compose logs
- visualizar containers: docker compose ps