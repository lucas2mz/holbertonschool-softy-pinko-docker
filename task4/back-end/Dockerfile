#Imagen de ubuntu
FROM ubuntu:latest
#Runear update,upgrade y instalamos python3
RUN apt-get update && apt-get upgrade -y && apt-get install -y python3 python3-pip && rm -f /usr/lib/python*/EXTERNALLY-MANAGED
#Instalar flask
RUN pip3 install Flask
RUN pip3 install Flask-Cors
#WorkDirectory
WORKDIR /app
# Copiamos api.py
COPY ./api.py /app/api.py
EXPOSE 5252
CMD ["python3", "api.py"]