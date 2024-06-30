# Effective-Mobile_task

Приложение доступно по адресу http://хост_из_/ansible/hosts.ini/ 

Nginx проксирует запросы к Flask приложению.
* Конфиг Nginx: /src/nginx/nginx.conf


Для запуска Ansible плейбука выполните команду в директории ansible:

```bash
ansible-playbook -i hosts.ini playbook_test.yml
```

После запуска плейбука будут выполнены роли необходимые для развертки приложения в докер контейнера на сервере указаном в /ansible/hosts.ini

Для проверки Docker отдельно, запустите команду в директории src:

```bash
sudo docker-compose up --build
```
