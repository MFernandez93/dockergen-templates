FROM node:latest

# Configurar el directorio de trabajo dentro del contenedor
WORKDIR /app

# Copiar los archivos del package.json y package-lock.json (si existen)
COPY package*.json ./

# Instalar las dependencias
RUN npm install

# Copiar el resto del código del proyecto
COPY . .

# Exponer el puerto por defecto de Express
EXPOSE 3000

# Comando por defecto para iniciar la aplicación
CMD ["node", "index.js"]