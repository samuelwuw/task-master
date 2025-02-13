# Usa a imagem oficial do Node.js
FROM node:18-alpine

# Define o diretório de trabalho
WORKDIR /app

# Copia os arquivos necessários
COPY package.json package-lock.json ./ 

# Instala as dependências
RUN npm install

# Copia o restante dos arquivos
COPY . .

# Expõe a porta 3000
EXPOSE 3000

# Inicia a aplicação
CMD ["npm", "run", "dev"]