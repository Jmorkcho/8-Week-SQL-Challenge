## Setting up

If you wish to follow along these solutions, you might find the best value in running them as you go, and for that you need a working Postgres database environment.

We'll use a Docker container for Postgres so we don't have to install it locally.

First, clone the repository to get the schemas for the challenges into a `schema/` directory.

```sh
git clone https://github.com/aalekhpatel07/8-week-sql-challenge && \
    cd 8-week-sql-challenge
```

Then, run the following command to start a Postgres Docker container in which we will create the necessary schemas/tables.

```sh
docker run -d -e POSTGRES_USER=postgres -e POSTGRES_PASSWORD=postgres --name postgres-server -p 5432:5432 --restart=always postgres
6d2754f36b2491c53080bf871696349ee5bbaf02eebfb8bac860b6d1f16eb3d0
```


-sslmode = allow.