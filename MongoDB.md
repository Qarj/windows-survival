# MongoDB

## Install Server

Admin command prompt
```
choco install mongodb
```

Add bin folder to system path

```
C:\Program Files\MongoDB\Server\4.0\bin
```

Create data folder
```
mkdir C:\data\db
```

Start with 
```
mongod
```

## Install Client

Download Community edition of Compass from https://www.mongodb.com/download-center/compass

Choose the plain vanilla `Windows 64-bit (7+)` exe file, the MSI doesn't work.


## Import some data

```
mongoimport --db mongo-exercises --collection courses --file exercise-data.json --jsonArray
```
