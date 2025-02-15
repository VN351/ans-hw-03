# Домашнее задание к занятию 3 «Использование Ansible»

## Подготовка к выполнению

1. Подготовьте в Yandex Cloud три хоста: для `clickhouse`, для `vector` и для `lighthouse`.
2. Репозиторий LightHouse находится [по ссылке](https://github.com/VKCOM/lighthouse).

## Основная часть

1. Допишите playbook: нужно сделать ещё один play, который устанавливает и настраивает LightHouse.
2. При создании tasks рекомендую использовать модули: `get_url`, `template`, `yum`, `apt`.
3. Tasks должны: скачать статику LightHouse, установить Nginx или любой другой веб-сервер, настроить его конфиг для открытия LightHouse, запустить веб-сервер.
4. Подготовьте свой inventory-файл `prod.yml`.
5. Запустите `ansible-lint site.yml` и исправьте ошибки, если они есть.
6. Попробуйте запустить playbook на этом окружении с флагом `--check`.
7. Запустите playbook на `prod.yml` окружении с флагом `--diff`. Убедитесь, что изменения на системе произведены.
8. Повторно запустите playbook с флагом `--diff` и убедитесь, что playbook идемпотентен.
9. Подготовьте README.md-файл по своему playbook. В нём должно быть описано: что делает playbook, какие у него есть параметры и теги.
10. Готовый playbook выложите в свой репозиторий, поставьте тег `08-ansible-03-yandex` на фиксирующий коммит, в ответ предоставьте ссылку на него.

---
---
## Ответ на задание
1.  [Ссылка на конфигурацию Ansible и README.md](https://github.com/VN351/ans-hw-3-code/tree/master)
2.  ![alt text](https://github.com/VN351/ans-hw-03/raw/main/images/task-1-1.png)
3.  ![alt text](https://github.com/VN351/ans-hw-03/raw/main/images/task-1-2.png)
4.  ![alt text](https://github.com/VN351/ans-hw-03/raw/main/images/task-1-3.png)
5.  ![alt text](https://github.com/VN351/ans-hw-03/raw/main/images/task-1-4.png)
6.  ![alt text](https://github.com/VN351/ans-hw-03/raw/main/images/task-1-5.png)
7.  ![alt text](https://github.com/VN351/ans-hw-03/raw/main/images/task-1-6.png)

### Как оформить решение задания

Выполненное домашнее задание пришлите в виде ссылки на .md-файл в вашем репозитории.

---
