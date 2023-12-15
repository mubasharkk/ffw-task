# FFW Backend Developer Test

<strike>HIDDEN</strike>

## Notes:
* Assuming the scale of the task is smaller
  * I have used a `api-platform/core`.
* As I haven't worked with symfony for some time already. I have tried to keep it simple. 
* I could have created a entity repository and controllers, but they would be doing the exact same thing with addition code.


## Files to assess:

* [src/Entity/Note.php](https://github.com/mubasharkk/ffw-task/blob/main/src/Entity/Note.php)

## Setup & Starting Docker

**Important:** !! Docker must be installed !!

Clone the repository and run the following command:

```
docker-compose up -d --build

```

To tun DB migrations

```
docker exec -it ffw-task-php-1 php bin/console doctrine:schema:update --force
```


---

## API Documentation

[https://localhost/api](https://localhost/api)

### Running tests

```
./vendor/bin/sail artisan test

./vendor/bin/sail artisan test tests/Feature/TestOrdersApiEndpoints.php
```
