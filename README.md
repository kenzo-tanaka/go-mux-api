```shell
export APP_DB_USERNAME=postgres
export APP_DB_PASSWORD=
export APP_DB_NAME=postgres
``` 

```shell
docker run -it -p 5342:5432 -d postgres
go test -v
```
