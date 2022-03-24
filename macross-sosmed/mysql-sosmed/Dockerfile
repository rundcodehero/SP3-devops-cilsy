FROM mysql:8.0

ENV MYSQL_USER rundcode
ENV MYSQL_PASSWORD rundcode
ENV MYSQL_ROOT_PASSWORD rundcode
ENV MYSQL_DATABASE dbsosmed

ADD dump.sql /docker-entrypoint-initdb.d
#The ADD command copy the database backup file to /docker-entrypoint-initdb.d directory in the Docker container. 
#The docker-entrypoint.sh file will run any files in this directory ending with “.sql” against the MySQL database. In our example, we have only one sql script file dump.sql.
EXPOSE 3306
