# Usages:

## build docker image
```
cd docker
docker build -t pgrestapi .
```

## pre-install dependencies
```
docker run -v $(pwd):/srv/PGRestAPI pgrestapi npm i
```

## serve
```
mv settings/settings.js.example settings.js # do sth else prefer
docker run -v $(pwd):/srv/PGRestAPI pgrestapi node app.js
```
