# Development environment for xserver with docker

### Image to be used.

<br>

- php:7.4-apache
- mysql:5.7
- phpmyadmin/phpmyadmin:5

<br>

### How to use

<br>

Move to the root directory.

```
# cd Users\[dounload files] 
```

<br>

Build image.

```
# docker-compose build
```

<br>

Lunch docker in the background.
```
# docker-compose up -d
```

<br>

### How to use php or composer

#### php
Go in application container and use bash. Then check the php version.

```
# docker container exec -it application bash
# php -v
```

<br>

#### composer
Go in application container and use bash. Then check the composer version.<br>
If the composer version is out of date, please update it to use update command.

```
# docker container exec -it application bash
# composer -v

// If the composer version is out of date
// Update to the latest version
composer self-update

// Specify the version. Ex)1.10.17
composer self-update 1.10.17

```

<br>

### Links
- [http://localhost(:80)](http://localhost)
- [phpmyadmin(:8080)](http://127.0.0.1:8080)
