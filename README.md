Задание 1
Запустите два simple python сервера на своей виртуальной машине на разных портах
Установите и настройте HAProxy, воспользуйтесь материалами к лекции по ссылке
Настройте балансировку Round-robin на 4 уровне.
На проверку направьте конфигурационный файл haproxy, скриншоты, где видно перенаправление запросов на разные серверы при обращении к HAProxy.

Решение 1
Балансировка на 4 уровне через round-robin

![ALT TEXT](https://github.com/mezhibo/Balansirovka-HAProxy/blob/a088b338e310c129882b5709570eb1e4dbb3ce07/IMG/2.jpg)

![ALT TEXT](https://github.com/mezhibo/Balansirovka-HAProxy/blob/39a632b6886cd11f0a49a163fc589b8d583c6377/IMG/1.jpg)

Ссылка на конфиг  https://github.com/mezhibo/Balansirovka-HAProxy/blob/f8815387e1b5d19d3bb070f269e037d4b3756ae6/haproxy.cfg

Задание 2
Запустите три simple python сервера на своей виртуальной машине на разных портах
Настройте балансировку Weighted Round Robin на 7 уровне, чтобы первый сервер имел вес 2, второй - 3, а третий - 4
HAproxy должен балансировать только тот http-трафик, который адресован домену example.local
На проверку направьте конфигурационный файл haproxy, скриншоты, где видно перенаправление запросов на разные серверы при обращении к HAProxy c использованием домена example.local и без него.

Настраиваем балансировку на 7 уровне

![ALT TEXT](https://github.com/mezhibo/Balansirovka-HAProxy/blob/3843a33e869f451ee1d9685a7469c8ece015c2e7/IMG/3.jpg)

Проверяем распределение запросов 

![ALT TEXT](https://github.com/mezhibo/Balansirovka-HAProxy/blob/b87b540875d7c639d36cba7813fd5b55d02d3c86/IMG/4.jpg)


Ссылка на конфиг https://github.com/mezhibo/Balansirovka-HAProxy/blob/6976e90b5ba0c0608501998d098cedebf4daa9be/haproxy2.cfg






