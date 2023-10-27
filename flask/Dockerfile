#imagen base
FROM python:3.8-slim-buster

WORKDIR /app
#copiar requeriments.txt e instalar las librerías de Python necesarias
COPY app.py /app
COPY requeriments.txt requeriments.txt


RUN pip3 install -r requeriments.txt

#copia todo el codigo

EXPOSE 5000
ENV MYSQL_ROOT_PASSWORD=p@sswOrd1

CMD [ "python3", "-m", "flask", "run", "--host=0.0.0.0" ]