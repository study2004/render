FROM mysql:8.0

ENV MYSQL_ROOT_PASSWORD=rootpassword
ENV MYSQL_DATABASE=mydb

RUN microdnf install -y python3 || true

EXPOSE 3306
EXPOSE 10000

CMD sh -c "mysqld & python3 -m http.server 10000"
