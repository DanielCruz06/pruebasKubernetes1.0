# Usamos una imagen base de Python
FROM python:3.9-slim

# Establecer el directorio de trabajo
WORKDIR /app

# Copiar el archivo de dependencias
COPY requirements.txt requirements.txt

# Instalar las dependencias
RUN pip install --no-cache-dir -r requirements.txt

# Copiar el resto de los archivos de la aplicación
COPY . .

# Exponer el puerto 5002 (donde se ejecuta el servicio Flask)
EXPOSE 5002

# Comando para ejecutar la aplicación Flask
CMD ["python", "app.py"]
