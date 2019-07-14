# Docker Compose for Gogs

Spin up [Gogs Git service](https://gogs.io/) on your localhost using Docker.

## Start Up

```
docker-compose up -d
```

## Accessing Gogs

Go to http://localhost:10080. 

For first-time use, you need to setup Gogs to point to MySQL database using information below:

Host: `gogs_db:3306`
User: `gogs`
Password: `secret`
Database Name: `gogs`

Change ports and application URL as follow:

SSH Port: `10022`
HTTP Port: `10080`
Application URL: `http:localhost:10080/`

Click to install and register the first user which will be assumed as the admin.

## Using SSH

To use SSH, change URL to the following patten:

```
ssh://git@localhost:10022/<username>/<repo_name>
```

## Shutdown

```
docker-compose down
```