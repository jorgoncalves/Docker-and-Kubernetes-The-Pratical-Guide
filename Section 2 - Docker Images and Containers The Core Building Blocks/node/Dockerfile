FROM node 
# Esta imagem deve de existir ou no nosso sistema, ou no dockerhub

WORKDIR /app
# Local onde todos os comandos devem de ser executados (para o docker)

COPY package.json /app

RUN npm install
# comando que deve de ser executado após copiar todos os ficheiros. No caso deve de ser dentro do app

COPY . /app
# Temos que indicar 2 caminhos.
# . para procurar que todos os ficheiros na raiz do Dockerfile devem ser copiados para a image.
# /app ou ./ (o WORKDIR) local dentro da imagem onde esses ficheiros devem de ser armazenados. No caso para dentro de uma pasta app



# RUN node server.js
# uma imagem é a template. o contendor é que deve de correr a servidor.

EXPOSE 80
# indica que porta deve de ser exposta para o sistema local
# é opcional

CMD ["node", "server.js"]
# o comando a executar após a instanciação da image

