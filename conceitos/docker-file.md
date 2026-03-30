# Dockerfile
- é um arquivo de texto que contém instruções passo a passo para montar a imagem da aplicação.
- ele fica na raiz de um projeto.
- exemplo de Dockerfile:

FROM node:20 (comece minha aplicação com uma imagem que tenha Node 20 instalado. Isso vem do Docker Hub)
WORKDIR /app (define a pasta de trabalho dentro do container, ou seja, tudo vai acontecer dentro de /app)
COPY ./app (copia arquivos da máquina para dentro da imagem Docker)
CMD node app.js (comando que roda quando o container inicia)

- depois de definido o Dockerfile, pode-se executar o comando: docker build -t meu-app,
serve para fazer o build da imagem docker. 

- depois, para rodar o container: docker run nome-da-imagem