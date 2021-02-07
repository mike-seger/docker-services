# docker-services 

## Run
```
docker-compose up -d postgres-db
# or
docker run -d -p 49161:1521 -e ORACLE_ALLOW_REMOTE=true oracleinanutshell/oracle-xe-11g
```