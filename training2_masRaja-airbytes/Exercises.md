# Exercises

## Understanding Docker Compose Configuration

- What is the purpose of changing the PostgreSQL host port from 5432 to 5435 in the `docker-compose.yml` file?
- How does this impact the `citus-master` container?

## Setting Up Airbyte with Docker

- Execute the command `docker-compose -f airbyte/docker-compose.yml up` and ensure that Airbyte is running.
- What happens when the `.env` file is missing?
- How would you resolve this issue?

## Airbyte Web UI Access and Authentication

- Once Airbyte is running, open [http://localhost:8000](http://localhost:8000).
- What credentials are required to log in?
- If the web UI does not load, what troubleshooting steps would you take?

## Managing PostgreSQL Data Persistence

- Locate the volume mappings in `docker-compose.yml`.
- What is the purpose of the `volumes` section in the `postgre` and `citus-master` containers?
- How would you modify this setup to store the database data in a custom directory on your host machine?

## Customizing Airbyte Deployment

- Modify the `docker-compose.yml` file to:
  - Change the PostgreSQL database name from `store` to `mydatabase`.
  - Update the Airbyte container port from `8000` to `8080`.
- Restart Airbyte and confirm the changes.
