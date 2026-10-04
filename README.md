# Docker nginx project


## Что это 
Мой первый проект с Docker: nginx в контейнере, который отдает мою HTML-страницу.


## Команда запуска
'''bash
sudo  docker run -d --name my-nginx -p 8080:80 -v "$(pwd)":/usr/share/nginx/html nginx
