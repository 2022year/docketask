## Задание:
Как системному администратору данной организации вам поставлена задача собрать на докер образ Django 
(Linux, nginx, Django, Postgres, Gunicorn) сервера. Все нужные сервисы должны быть проброшены на хост по стандартным 
портам, реализация HTTPS не требуется, версии Django, nginx и Postgres не имеют значения, как и версия ядра Linux. 
В проекте просто должна работать админка с заранее прописанным логином и паролем.


1.Установить docker,  
2.Загружаем проект командой: 
git clone https://github.com/2022year/docketask.git

3.В командной строке, переходим в директорию проекта и набираем:  
docker build -t dockertask .
		(dockertask - имя контейнера)

4.Запустить контейнер
docker run -it -p 8000:8000 dockertask

5.В браузере открыть
http://localhost:8000

  логин: admin
  пароль: abc
