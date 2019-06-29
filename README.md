# Docker Compose for Gogs

Spin Gogs Git repository on your localhost using Docker.

## Start Up

```
docker-compose up -d
```

## Accessing Gogs

Go to http://localhost:10080. 

For first-time use, you need to setup Gogs to point to MySQL database using information below:

Database Host: `gogs_db:3306`
Database Name: `gogs`
Database User: `gogs`
Password: `secret`

## Using SSH

To use SSH, change URL to the following patten:

```
ssh://git@localhost:10022/<username>/<repo_name>
```

## Shutdown

```
docker-compose down
```