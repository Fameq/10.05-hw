# Домашнее задание к занятию "10.5 Балансировка нагрузки. HAProxy/Nginx." - Кувайсков Дмитрий


---

### Задание 1.

Что такое балансировка нагрузки и зачем она нужна? 

*Приведите ответ в свободной форме.*

`Балансировка нагрузки - это процесс распределения нагрузки на кластер серверов, она нужна для улучшения отказоустойчивости и упрощения масштабируемости` 

---

### Задание 2.

Чем отличаются между собой алгоритмы балансировки round robin и weighted round robin? В каких случаях каждый из них лучше применять? 

*Приведите ответ в свободной форме.*

`Алгоритмом Weighted round robin можно указать какое количество трафика отправлять на определенный сервер, так можно лучше сбалансировать нагрузку`

---


### Задание 3.

Установите и запустите haproxy.

*Приведите скриншот systemctl status haproxy, где будет видно, что haproxy запущен.*

![alt text](https://github.com/Fameq/10.05-hw/blob/master/img/task3.png)

---

### Задание 4.

Установите и запустите nginx.

*Приведите скриншот systemctl status nginx, где будет видно, что nginx запущен.*

![alt text](https://github.com/Fameq/10.05-hw/blob/master/img/task4.png)

---

### Задание 5.

Настройте nginx на виртуальной машине таким образом, чтобы при запросе:

`curl http://localhost:8088/ping`

он возвращал в ответе строчку: 

"nginx is configured correctly"

*Приведите скриншот получившейся конфигурации.*

![alt text](https://github.com/Fameq/10.05-hw/blob/master/img/task5.png)

---

## Дополнительные задания (со звездочкой*)

Эти задания дополнительные (не обязательные к выполнению) и никак не повлияют на получение вами зачета по этому домашнему заданию. Вы можете их выполнить, если хотите глубже и/или шире разобраться в материале.

---

### Задание 6*.

Настройте haproxy таким образом, чтобы при ответе на запрос:

`curl http://localhost:8080/`

он проксировал его в nginx на порту 8088, который был настроен в задании 5 и возвращал от него ответ: 

"nginx is configured correctly". 

*Приведите скриншот получившейся конфигурации.*

