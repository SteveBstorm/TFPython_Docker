FROM postgres:latest

ENV POSTGRES_USER "monuser"
ENV POSTGRES_PASSWORD "test1234"
ENV POSTGRES_DB "tfpython"

WORKDIR "/appdb"

COPY "init.sql" "/docker-entrypoint-initdb.d"

EXPOSE 5432

VOLUME ["/var/postgres/pgdata:mydb_v"]