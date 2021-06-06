# How to run and environment preparation

- To successfully run the project, you need up and running PostgreSQL with database name paypay.
- If you want to change the DB name, you can do that in backend folder in .env file in DB_NAME variable.
- Clone the project and run

```
$ git submodule update --init --recursive
```

I use yarn, but you can run with npm no problem.

Frontend App run

```
$ cd frontend
$ yarn install
$ yarn serve
```

Backend App run
Open another terminal and run

```
$ cd backend
$ yarn install
$ yarn run knex:migrate
$ yarn run knex:seed
$ yarn serve
```

See package.json in backend folder for more scripts.

## There are 2 seeded users

- email: admin@paypay.com password: admin
- email: user@paypay.com password: user

Enjoy!
