Задание 1
Дана схема для Cisco Packet Tracer, рассматриваемая в лекции.
На данной схеме уже настроено отслеживание интерфейсов маршрутизаторов Gi0/1 (для нулевой группы)
Необходимо аналогично настроить отслеживание состояния интерфейсов Gi0/0 (для первой группы).
Для проверки корректности настройки, разорвите один из кабелей между одним из маршрутизаторов и Switch0 и запустите ping между PC0 и Server0.
На проверку отправьте получившуюся схему в формате pkt и скриншот, где виден процесс настройки маршрутизатора.
![Task1](https://github.com/DmitriyKly/HW_DevOps_Netology/blob/main/Disaster%20recovery%20%D0%B8%20Keepalived/Screen/Task1.png)
![Task1_1](https://github.com/DmitriyKly/HW_DevOps_Netology/blob/main/Disaster%20recovery%20%D0%B8%20Keepalived/Screen/Task1_1.png)
Задание 2
Запустите две виртуальные машины Linux, установите и настройте сервис Keepalived как в лекции, используя пример конфигурационного файла.
Настройте любой веб-сервер (например, nginx или simple python server) на двух виртуальных машинах
Напишите Bash-скрипт, который будет проверять доступность порта данного веб-сервера и существование файла index.html в root-директории данного веб-сервера.
Настройте Keepalived так, чтобы он запускал данный скрипт каждые 3 секунды и переносил виртуальный IP на другой сервер, если bash-скрипт завершался с кодом, отличным от нуля (то есть порт веб-сервера был недоступен или отсутствовал index.html). Используйте для этого секцию vrrp_script
На проверку отправьте получившейся bash-скрипт и конфигурационный файл keepalived, а также скриншот с демонстрацией переезда плавающего ip на другой сервер в случае недоступности порта или файла index.html
Дополнительные задания со звёздочкой*
Эти задания дополнительные. Их можно не выполнять. На зачёт это не повлияет. Вы можете их выполнить, если хотите глубже разобраться в материале.
![Task2](https://github.com/DmitriyKly/HW_DevOps_Netology/blob/main/Disaster%20recovery%20%D0%B8%20Keepalived/Screen/Task2.png)
![Task2_2](https://github.com/DmitriyKly/HW_DevOps_Netology/blob/main/Disaster%20recovery%20%D0%B8%20Keepalived/Screen/Task2_2.png)
![Task2_3](https://github.com/DmitriyKly/HW_DevOps_Netology/blob/main/Disaster%20recovery%20%D0%B8%20Keepalived/Screen/Task2_3.png)