FROM mysql:8.0

ENV MYSQL_ROOT_PASSWORD=rootpassword
ENV MYSQL_DATABASE=mydb

RUN apt-get update && apt-get install -y python3

EXPOSE 3306
EXPOSE 10000

CMD sh -c "mysqld & python3 -m http.server 10000"
