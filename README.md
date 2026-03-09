# Набор команд
## Управление приложением
Остановить все сервисы
```shell
docker compose down
```
Запустить все сервисы
```shell
docker compose up -d
```
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
## Minio
Создать основной бакет и настроить политики (minio-policy.json)
```shell
docker compose run --rm create_minio_bucket
```
