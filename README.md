# Домашнее задание к занятию «Кеширование Redis/memcached»

### Инструкция по выполнению домашнего задания

1. Сделайте fork [репозитория c шаблоном решения](https://github.com/netology-code/sys-pattern-homework) к себе в Github и переименуйте его по названию или номеру занятия, например, https://github.com/имя-вашего-репозитория/gitlab-hw или https://github.com/имя-вашего-репозитория/8-03-hw).
2. Выполните клонирование этого репозитория к себе на ПК с помощью команды `git clone`.
3. Выполните домашнее задание и заполните у себя локально этот файл README.md:
   - впишите вверху название занятия и ваши фамилию и имя;
   - в каждом задании добавьте решение в требуемом виде: текст/код/скриншоты/ссылка;
   - для корректного добавления скриншотов воспользуйтесь инструкцией [«Как вставить скриншот в шаблон с решением»](https://github.com/netology-code/sys-pattern-homework/blob/main/screen-instruction.md);
   - при оформлении используйте возможности языка разметки md. Коротко об этом можно посмотреть в [инструкции по MarkDown](https://github.com/netology-code/sys-pattern-homework/blob/main/md-instruction.md).
4. После завершения работы над домашним заданием сделайте коммит (`git commit -m "comment"`) и отправьте его на Github (`git push origin`).
5. Для проверки домашнего задания преподавателем в личном кабинете прикрепите и отправьте ссылку на решение в виде md-файла в вашем Github.
6. Любые вопросы задавайте в чате учебной группы и/или в разделе «Вопросы по заданию» в личном кабинете.

Желаем успехов в выполнении домашнего задания.

---

### Задание 1. Кеширование 

Приведите примеры проблем, которые может решить кеширование. 

*Приведите ответ в свободной форме.*

---

Кеширование может решить следующие проблемы:

1. Увеличение производительности: Когда данные или результаты вычислений часто запрашиваются, кеширование позволяет сохранить их в быстром доступе, что позволяет сократить время выполнения запросов и улучшить общую производительность системы.

2. Снижение нагрузки на сервер: Кеширование позволяет серверу избежать повторной генерации или вычисления данных, которые уже были запрошены и сохранены в кеше. Это позволяет сократить нагрузку на сервер и улучшить его отзывчивость.

3. Сокращение использования сетевого трафика: Кеширование позволяет сократить количество запросов к удаленным серверам или базам данных, так как данные могут быть получены из кеша, что позволяет снизить использование сетевого трафика и ускорить передачу данных.

4. Повышение отказоустойчивости: Кеширование может использоваться для сохранения резервных копий данных или результатов вычислений, что позволяет восстановить систему быстрее в случае сбоев или неполадок.

5. Улучшение масштабируемости: Кеширование может быть использовано для распределения нагрузки между несколькими серверами или узлами, что позволяет улучшить масштабируемость системы и обеспечить более высокую производительность при большом количестве запросов.

---

### Задание 2. Memcached

Установите и запустите memcached.

*Приведите скриншот systemctl status memcached, где будет видно, что memcached запущен.*
![image](https://github.com/Darxmax/git_homework/assets/54942567/c73f2acd-c660-4b4a-8450-c4e278441b92)


---

### Задание 3. Удаление по TTL в Memcached

Запишите в memcached несколько ключей с любыми именами и значениями, для которых выставлен TTL 5. 

*Приведите скриншот, на котором видно, что спустя 5 секунд ключи удалились из базы.*


![image](https://github.com/Darxmax/git_homework/assets/54942567/b8d4532f-f0ad-4b23-a149-cf3b72120f2a)


---

### Задание 4. Запись данных в Redis

Запишите в Redis несколько ключей с любыми именами и значениями. 

*Через redis-cli достаньте все записанные ключи и значения из базы, приведите скриншот этой операции.*

![image](https://github.com/Darxmax/git_homework/assets/54942567/c1659129-0d16-425e-aed4-a0c79897b65e)

---

## Дополнительные задания (со звёздочкой*)
Эти задания дополнительные, то есть не обязательные к выполнению, и никак не повлияют на получение вами зачёта по этому домашнему заданию. Вы можете их выполнить, если хотите глубже разобраться в материале.

### Задание 5*. Работа с числами 

Запишите в Redis ключ key5 со значением типа "int" равным числу 5. Увеличьте его на 5, чтобы в итоге в значении лежало число 10.  

*Приведите скриншот, где будут проделаны все операции и будет видно, что значение key5 стало равно 10.*
