FROM ubuntu

RUN apt-get update && apt-get install -y mariadb-server

COPY ./my.cnf /etc/mysql/my.cnf

EXPOSE 3306

CMD ["mysqld"]