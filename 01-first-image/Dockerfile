#qual a plataforma 
FROM node:alpine

#na imagem, vai criar um arquivo chamado app e vai grava tudo que tiver nesse ditório atual
COPY . /app

#para não ter que indicar /app/app.js sempre...
#indica diretório na imagem
WORKDIR /app

#comandos para rodar a aplicação
CMD node app.js