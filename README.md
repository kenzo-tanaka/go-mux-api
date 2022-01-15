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
=== RUN   TestEmptyTable
--- PASS: TestEmptyTable (0.01s)
=== RUN   TestGetNonExistentProduct
--- PASS: TestGetNonExistentProduct (0.01s)
=== RUN   TestGetProduct
--- PASS: TestGetProduct (0.01s)
=== RUN   TestCreateProduct
--- PASS: TestCreateProduct (0.01s)
=== RUN   TestUpdateProduct
--- PASS: TestUpdateProduct (0.02s)
=== RUN   TestDeleteProduct
--- PASS: TestDeleteProduct (0.02s)
PASS
ok      github.com/kenzo-tanaka/go-mux-api      0.256s
```
