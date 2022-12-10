FROM postgres
ARG DB_PASSWORD DB_HOST DB_PORT DB_USERNAME DB_NAME
RUN PGPASSWORD=$DB_PASSWORD pg_dump --host $DB_HOST --port $DB_PORT --username $DB_USERNAME --dbname $DB_NAME > /docker-entrypoint-initdb.d/bk.sql

