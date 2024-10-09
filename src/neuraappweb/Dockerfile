# Usar la imagen oficial de Node.js como base
FROM node:18

# Establecer el directorio de trabajo en el contenedor
WORKDIR /app

# Copiar el archivo package.json y package-lock.json (si existe)
COPY package*.json ./

# Instalar las dependencias del proyecto
RUN npm install

# Copiar el resto del código fuente del proyecto
COPY . .

# Exponer el puerto 8080 (o el que tu aplicación utilice)
EXPOSE 8080

# Comando por defecto que ejecuta el servidor de desarrollo de Vue
CMD ["npm", "run", "serve"]
