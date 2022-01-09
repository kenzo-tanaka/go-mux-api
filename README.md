```shell
export APP_DB_USERNAME=postgres
export APP_DB_PASSWORD=
export APP_DB_NAME=postgres
``` 

```shell
# docker run
docker run -it -p 5432:5432 -e 'POSTGRES_PASSWORD=postgres' -e 'POSTGRES_HOST_AUTH_METHOD=trust' -d postgres
```

```shell
go test -v
```
