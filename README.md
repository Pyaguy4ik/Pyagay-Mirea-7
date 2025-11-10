# Практическое задание № 7

# Подключение и работа с Redis (set/get, TTL). Реализация простого кэша.

Студент группы *ЭФМО-02-25 Пягай Даниил Игоревич*

# Описание

**Цели:**

    • Освоить базовые операции работы с Redis из Go-приложения.
    • Научиться использовать команды SET, GET, задавать время жизни ключей (TTL).
    • Реализовать кэширование данных для ускорения работы API.
    • Понять, в каких случаях кэш помогает снизить нагрузку на базу данных.


## Инициализация проекта

```bash
mkdir pz7-redis
cd pz7-redis
go mod init example.com/pz7-redis
go get github.com/redis/go-redis/v9
```

## Создаём структуру файлов

![structure](img/structure.png)

### Содержимое postgres.go
![cache.go](img/cache.go.png)

### Содержимое main.go
![main.go](img/main.go.png)

# Запуск и проверка
![go.run](img/go_run.png)

# Проверяем

## /Health
![haelth](img/health.png)

## Запрос /Set
![Set](img/set_1.png)
![Set](img/set_2.png)

## Запрос /Get
![Get](img/get.png)

## Запрос /ttl
![ttl](img/ttl_1).png
