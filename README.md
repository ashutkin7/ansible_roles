# Ansible-роль: Nginx Virtual Hosts

Проект автоматизирует установку веб-сервера Nginx и развертывание виртуальных хостов (vhosts) из списка переменной `sites` с использованием Jinja2-шаблонов для конфигурационных файлов и индексных страниц.

## Структура
* `playbook.yml` — плейбук вызова роли.
* `inventory.ini` — хосты для установки.
* `roles/nginx_vhosts/` — роль настройки Nginx vhosts.
* `.github/workflows/lint.yml` — CI-проверка кода с помощью `ansible-lint`.
*   `ansible.cfg` — конфигурация логирования.
*   `ansible.log` — лог-файл выполнения команд и плейбуков.

## Запуск
```bash
ansible-playbook ./playbook.yml -i ./inventory.ini 
```

## Логи выполнения
* [ansible.log](./ansible.log)
