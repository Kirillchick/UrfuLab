# Запуск из-под Docker с Linux

* Создать образ с помощью команды (в директории, где лежит Dockerfile):
```bash
docker build -t monitor .
```
* Запустить монитор (демон) с помощью команды:
```bash
docker run -it --rm monitor
```
Внутри контейнера выполнить команду:
```bash
./monitor
```



# Если не демон (но тогда надо править исходники)
* Запустить монитор (демон) с помощью команды: ```docker run --rm monitor```
    - ```--rm``` — указывает, что контейнер следует удалить после завершения работы в нём. Образ при этом не будет затронут.
