FROM ubuntu:20.04
RUN apt-get update && apt-get install -y python3-pip
RUN pip3 install Flask
RUN useradd -ms /bin/bash subrahmanyam1216
USER subrahmanyam1216
COPY . /opt/
EXPOSE 8080
ENTRYPOINT FLASK_APP=/opt/app.py flask run --host=0.0.0.0 --port=8080
