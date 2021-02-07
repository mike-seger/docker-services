# docker-services 

## Run
```
# from this directory!

# start all services
docker-compose up -d

# or single ones
docker-compose up -d postgres-db
docker-compose up -d oracle-db

# or without compose from any directory
docker run --name oracle-db -d -p 49161:1521 -e ORACLE_ALLOW_REMOTE=true oracleinanutshell/oracle-xe-11g
docker run --name postgres-db -d  -p 15432:5432 -e POSTGRES_PASSWORD=secret postgres
```

## default connection info
### oracle
```
port: 49161
SID: xe
user: system
password: oracle
```

### postgres
```
port: 5432
user: postgres
password: secret
```
