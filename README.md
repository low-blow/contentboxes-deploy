# Набор команд
## Миграции
Применить миграции
```shell
docker compose run --rm migrate up
```
Откатить одну миграцию
```shell
docker compose run --rm migrate down 1
```
Откатить всё
```shell
docker compose run --rm migrate down
```
Посмотреть статус
```shell
docker compose run --rm migrate version
```
