# Postgres Dockerfile
FROM ubuntu

# Install Postgres
RUN apt-get update && apt-get install -y postgresql

# Run the setup script
RUN service postgresql start && su - postgres -c "psql -c \"CREATE USER next WITH PASSWORD 'next';\""

# Expose the Postgres port
EXPOSE 5432

# Start Postgres
USER postgres

CMD ["/usr/lib/postgresql/16/bin/postgres", "-D", "/usr/local/var/postgres"]