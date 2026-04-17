FROM mysql:8.0

ENV MYSQL_ROOT_PASSWORD=rootpassword
ENV MYSQL_DATABASE=mydb

# Install a simple HTTP server
RUN apt-get update && apt-get install -y python3

# Expose both ports
EXPOSE 3306
EXPOSE 10000

# Start MySQL + fake HTTP server
CMD sh -c "mysqld & python3 -m http.server 10000"FROM mysql:8.0

ENV MYSQL_ROOT_PASSWORD=rootpassword
ENV MYSQL_DATABASE=mydb

EXPOSE 3306
