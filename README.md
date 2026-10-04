# Docker nginx project


## Что это 
Мой первый проект с Docker: nginx в контейнере, который отдает мою HTML-страницу.


## Команда запуска через монтирование папки(-v)
```bash
sudo  docker run -d --name my-nginx -p 8080:80 -v "$(pwd)":/usr/share/nginx/html nginx


```


## Запуск через Dockerfile
Собрать образ:
```bash
sudo docker build -t my-nginx-image .


```
 
Запустить контейнер:
```bash
sudo docker run -d --name my-nginx-custom -p 9090:80 my-nginx-image


```
