# UPD: 
Если очень хочется *pipeline project* можете использовать его.

## Задание 1(Minimum):
Создать на jenkins сервере freestyle project который:
* Делает pull с репозитория.
* Собирает docker image и делает push в docker repo (репозиторий на ваше усмторение)

### Для выполения задания 1 вам нужно:
* Сделать форк вот этого репозитория: https://github.com/microsoft/project-nodejs-express-webapp
* Разобраться как стартует веб приложение написанное на NodeJS
* Сделать для него Dockerfile
* Добавить публичный ключ Jenkins(jenkins-pub.key), который находится в репозитории MA, к своему форку.
* Создать freestyle project который будет иметь доступ к вашему репозиторию на github и к вашему docker репозиторию
* Запустить билд и в результате получить docker image в вашем docker repo.

### Результат выполеного задания 1:
* ПР с файлом который содержит имя вашего docker image.`(Пример: 683038831899.dkr.ecr.eu-west-2.amazonaws.com/vadym.tyshchenko:latest)`
* Репозиторий должен быть *публичным* что бы ментор мог сделать pull и локально запустить docker image или *предоставить доступ к приватному* репозиторию.
* Имя вашего проекта в Jenkins
* Freestyle project должен выполнять по нажатию на кпоку "Start build"

### Tip's:
* Можете устанавливать и использовать любые плагины на ваше усмотрение
* Не удалять чужие проекты в Jenkins
* Креды до Jenkins сервера будут доступны в Slack

## Задание 2(Maximum):
Всё пункты с первого задания и плюс:
* Деплой docker image на сервер 3.11.194.230
* Приложение должно быть доступным с "мира"(Ментор может проверить работу docker контейнера через браузер)

### Для выполения задания 2 вам нужно:
* Установить docker-сe если до этого момента никто это не сделал
* Создать свой деплоймент и запустить свой docker image с вашего docker репозитория. 
* Дописать Jenkins freestyle project

### Tip's:
* На серевере для деплоя открытые порты с 3000 по 3100
* ssh доступ к серверу для деплоя открыт для Jenkins сервера

### Результат выполеного задания 2:
* Ссылка на ваше приложение
* Имя вашего проекта в Jenkins
* Freestyle project должен выполнять по нажатию на кпоку "Start build"

# Deadline: 16:00 03.02.2020
P.S. Без исключений :) 
