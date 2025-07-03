# Imagen base oficial de Node
FROM node:18

# Crea un directorio de trabajo dentro del contenedor
WORKDIR /app

# Copia tu db.json en el contenedor
COPY server/db.json /app/db.json

# Instala json-server de manera global
RUN npm install -g json-server

# Expone el puerto que usaremos
EXPOSE 10000

# Comando para iniciar json-server
CMD ["json-server", "--watch", "/app/db.json", "--port", "10000"]
