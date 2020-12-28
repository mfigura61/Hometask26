# Hometask 26 Динамический веб контент.  

```
Собрать стенд с 3мя проектами на выбор
Варианты стенда
nginx + php-fpm (laravel/wordpress) + python (flask/django) + js(react/angular)
nginx + java (tomcat/jetty/netty) + go + ruby
можно свои комбинации

Реализации на выбор
- на хостовой системе через конфиги в /etc
- деплой через docker-compose

Для усложнения можно попросить проекты у коллег с курсов по разработке

К сдаче принимается
vagrant стэнд с проброшенными на локалхост портами
каждый порт на свой сайт
через нжинкс
```

## В процессе было сделано:
Настроен Vagrantfile и плейбук ansible для развертки следующей конфигурации:
- проект https://github.com/mfigura61/django c django висит на порту localhost:8000 и проксирутся nginx с порта 83
- проект https://github.com/mfigura61/go-http-hello-world с go висит на порту localhost:8800 и проксирутся nginx с порта 81
- проект https://github.com/mfigura61/react-helloworld с react висит на порту localhost:7777 и проксирутся nginx с порта 82


1. GO

![Image 1](https://raw.githubusercontent.com/mfigura61/Hometask26/master/screenshots/scr1.png)

--------
2. React

![Image 2](https://raw.githubusercontent.com/mfigura61/Hometask26/master/screenshots/scr2.png)

--------
3. Django

![Image 3](https://raw.githubusercontent.com/mfigura61/Hometask26/master/screenshots/scr3.png)


## Как проверить работоспособность:
Стенд запускается vagrant up.  После чего можно перейти по ссылкам:
- http://192.168.100.10:83
- http://192.168.100.10:82
- http://192.168.100.10:81

---
