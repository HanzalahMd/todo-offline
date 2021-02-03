This is a simple todo react app with Hasura GraphQL backend and RxDB frontend. The frontend was bootstrapped with [Create React App]. and the backend is running through docker.

## Available Scripts

In the frontend directory, you can run:

### `yarn start`

Runs the app in the development mode.<br />
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

In the backend directory, you can run:

### `docker compose up`

This Docker Compose setup runs [Hasura GraphQL Engine](https://github.com/hasura/graphql-engine) along with Postgres and [pgAdmin4](https://www.pgadmin.org/) using `docker-compose`.

## Important endpoints

- GraphQL endpoint will be `http://localhost:8080/v1/graphql`
- Hasura Console will be available on `http://localhost:8080/console`
- pgAdmin will be available on `http://localhost:5050`


## Connecting to External Postgres

If you want to connect to an external/existing postgres database, replace `HASURA_GRAPHQL_DATABASE_URL` in `docker-compose.yaml` with your database url.