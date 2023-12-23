<!-- To preview README.md in VS code use cmd + K V -->

# MySQL container
## To build a container based on the docker-compose.yml file included in this project: 
```
docker-compose up -d
```
- This will create a mysql instance with a DB named MyDB.
- MyDB root password is 'Password' by default.
- mysql_data persistent named volume will be created.
- .sql dump in local db_entrypoint directory will be imported in the DB if no existing data in mysql_data volume.

## To stop and eliminate the container:
```
docker-compose down
```

## To eliminate the sql volume:
- Check volume name using:
```
docker volumes ls
```
- Delete the corresponding volume using:
```
docker volumes rm <volume_namev>
```