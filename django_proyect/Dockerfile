# Usamos la imagen oficial de Python
FROM python:3.8

# Establecemos el directorio de trabajo en /django_proyect
WORKDIR /django_proyect

# Copiamos los archivos de requerimientos (requirements.txt) al contenedor
COPY requirements.txt /django_proyect/

# Instalamos las dependencias
RUN pip install -r requirements.txt

# Copiamos el resto de los archivos del proyecto al contenedor
COPY . /django_proyect/

# Exponemos el puerto en el que se ejecuta la aplicación
EXPOSE 8000

# Comando para ejecutar la aplicación
CMD ["python", "manage.py", "runserver", "127.0.0.1:8000"]
