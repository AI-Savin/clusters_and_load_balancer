# Домашнее задание к занятию "Кластеризация и балансировка нагрузки" - Савин Алексей

### Задание 1
* Запустите два simple python сервера на своей виртуальной машине на разных портах  
* Установите и настройте HAProxy, воспользуйтесь материалами к лекции по ссылке
* Настройте балансировку Round-robin на 4 уровне.
* На проверку направьте конфигурационный файл haproxy, скриншоты, где видно перенаправление запросов на разные серверы при обращении к HAProxy.

### Решение 1

    
  

конфигурационный файл [haproxy](https://github.com/AI-Savin/clusters_and_load_balancer/blob/main/img/task1_haproxy.cfg)  
![task1_haproxy](https://github.com/AI-Savin/clusters_and_load_balancer/blob/main/img/task1_haproxy.png)  
![task1_stat](https://github.com/AI-Savin/clusters_and_load_balancer/blob/main/img/task1_stat.png)

---

### Задание 2
* Запустите три simple python сервера на своей виртуальной машине на разных портах
* Настройте балансировку Weighted Round Robin на 7 уровне, чтобы первый сервер имел вес 2, второй - 3, а третий - 4
* HAproxy должен балансировать только тот http-трафик, который адресован домену example.local
* На проверку направьте конфигурационный файл haproxy, скриншоты, где видно перенаправление запросов на разные серверы при обращении к HAProxy c использованием домена example.local и без него.

 
 ### Решение 2

 конфигурационный файл [haproxy](https://github.com/AI-Savin/clusters_and_load_balancer/blob/main/img/task2_haproxy.cfg)  
![task2_curl](https://github.com/AI-Savin/clusters_and_load_balancer/blob/main/img/task2_curl.png)  
![task2_stat](https://github.com/AI-Savin/clusters_and_load_balancer/blob/main/img/task2_stat.png)  
