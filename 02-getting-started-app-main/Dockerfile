# Utiliza a imagem base Node.js 12-alpine
FROM node:16-alpine

# Define o diretório de trabalho dentro do contêiner
WORKDIR /app

# Copia arquivo de dependências e verifica se realmente tem que instalar novas dependências
COPY package.json .

# Instala dependências do Python 2, G++, e Make sem cache
RUN apk add --no-cache python3 g++ make

# Instala dependências do aplicativo usando Yarn
RUN yarn install --production

# Copia todos os arquivos do diretório atual para o diretório de trabalho no contêiner
COPY . .

# Expor a porta que a aplicação irá rodar
# Porta do Container... Não do notebook
EXPOSE 3000

# Define o comando para executar a aplicação
CMD ["node", "src/index.js"]






# Comentários adicionais e comandos para adicionar conforme necessário:
# 
# Copia arquivos específicos para o diretório de trabalho
# COPY package.json /app/
# COPY yarn.lock /app/
#
# Cria e adiciona um usuário ao grupo 'dev'
# RUN addgroup dev && adduser -S -G dev luiza
#
# Define o usuário que será utilizado
# USER luiza
#
# Copia um arquivo de uma URL externa
# ADD https://microsoft.com/teste.json /app/teste.json
#
# Adiciona e descompacta um arquivo zip
# ADD teste.zip /app/
#
# Define a variável de ambiente para a API
# ENV API_URL=https://api.luizakuze.com/
#
# Define o PATH
# ENV PATH=/app/node_modules/.bin:$PATH
