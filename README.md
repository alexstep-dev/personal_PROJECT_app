**Personal Activity Project**

_Frontend:_

> **build:**

`cd frontend`

`npm run build`

> **develop with WebpackDevServer:**

`cd frontend`

`npm start`

_Backend:_

> **Build application**

`docker-compose -f app.yml build`

> **Run application**

`docker-compose -f app.yml up`

> **Stop application and network**

`docker-compose -f app.yml down`

> **Backend TypeScript transpilation:**

`cd backend`

`npm run watch-ts`

_Database:_

- create **db** directory _(for database file system containing)_
- add **db.env** file which contains Postgress ENV variables _(NodeJS application and Postgress container will use it together for create connection between application and database)_:
  - PGPASSWORD=qwerty
  - PGUSER=somebody
  - PGDATABASE=mydb
  - PGHOST=**db** ! _this name of host is important, it equals to service name in Docker-Compose configuration_