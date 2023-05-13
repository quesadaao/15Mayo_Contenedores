# Seleccionamos la imagen base
FROM node:16-alpine

# Establecemos el directorio de trabajo
WORKDIR /app

# Copiamos el archivo package.json y package-lock.json
COPY package*.json ./

# Instalamos las dependencias de la aplicación
RUN npm install

# Copiamos los archivos de la aplicación
COPY . .

# Exponemos el puerto 3000
EXPOSE 3000

# Comando para iniciar la aplicación
CMD ["npm", "start"]
