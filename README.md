 # Docker-compose
 ## Описание
 Учебный проект по работе с Docker
 ## Инструкции по запуску

1.  Создайте рабочую директорию для хранения проекта:  
    `mkdir ~/Dev`
2.  Склонируйте репозиторий на ваш компьютер:  
    `git clone https://github.com/Talpik/infra_sp2.git ~/Dev/yamdb`
3.  Установите Docker для запуска приложения:  
    [https://docs.docker.com/engine/install/](https://docs.docker.com/engine/install/)
4.  Перейдите в папку проекта  **yamdb**:  
    `cd ~/Dev/yambd`
5.  Запустите утилиту  **docker-compose**, чтобы развернуть контейнеры:  
    `docker-compose up`
6.  Проверьте запущенные контейнеры:  
    `docker container ls`  и скопируйте занчение  **CONTAINER ID**  контейнера  **web**
7.  Проведите миграции внутри контейнера  **web**:  
    `docker exec -it <container id> python manage.py migrate`
8.  Создайте суперпользователя:  
    `docker exec -it <container id> python manage.py createsuperuser`  

## Автор
*Нестерёнок Георгий Дмитриевич*