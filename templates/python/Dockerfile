FROM python:latest

# Configurar el directorio de trabajo dentro del contenedor
WORKDIR /app

# Copiar y instalar las dependencias
COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt

# Copiar el resto del código del proyecto
COPY . .

# Exponer el puerto por defecto de Flask
EXPOSE 5000

# Comando por defecto para iniciar la aplicación
CMD ["python", "app.py"]