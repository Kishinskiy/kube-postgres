# Kube Postgres

StatefullSet For Postgres


## Run
```sh
kube apply -f .
```

## connect to database

```sh
kubectl run -i --tty --rm psql-client --image=postgres:16-alpine -n postgres --env="PGPASSWORD=SuperSecretPassword" --command -- psql -h postgres -U my_user -d my_database
```
