- docker image ls: lista todas as imagens criadas;

- docker run nome-da-imagem: roda um container docker;

- docker build -t nome-imagem: builda uma imagem com base na configuração do Dockerfile;

- docker ps: lista containers ativos;

- docker ps -a: lista todos os containers;

- renomear container em execução: docker run --name meu-container nome-imagem;

- listar logs de um container: docker logs -f id-container;

- docker start nome-container: roda um container existente;

- docker stop nome-container ou id: encerra a execução de um container;

- docker volume ls: lista volumes existentes;