# Dockerfile
- é um arquivo de texto que contém instruções passo a passo para montar a imagem da aplicação.
- ele fica na raiz de um projeto.
- exemplo de Dockerfile:

FROM node:20 (comece minha aplicação com uma imagem que tenha Node 20 instalado. Isso vem do Docker Hub)

WORKDIR /app (define a pasta de trabalho dentro do container, ou seja, tudo vai acontecer dentro de /app)

COPY . /app (copia arquivos da máquina para dentro da imagem Docker)

CMD node app.js (comando que roda quando o container inicia)

RUN yarn install --production (comando que roda configurações do projeto por exemplo, no momento de criação da imagem)

EXPOSE 3000 (expor a porta que a aplicação usará)

ENV API_URL=http://example (definir variáveis de ambiente)

- depois de definido o Dockerfile, pode-se executar o comando: docker build -t meu-app,
serve para fazer o build da imagem docker. 

- depois, para rodar o container: docker run nome-da-imagem