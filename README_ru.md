# Пример инфраструктурного репозитория Ansible.

[In English](README.md)

## Описание
* Роли либо хранятся в директории `roles`, либо загружаются из  `ansible-galaxy install -r requirements.yml` при выполнении
* Окружения описаны в директории `environments`, каждое в своей папке и своими `group_vars` при необходимости.
* Все плейбуки находятся в директории `playbooks`.
* По умолчанию используется `inventory` файл типа `ini`. Начиная с версии 2.4 возможно использовать `yml` формат.

## Использование
* Клонировать и зайти в папку репы
* Создать vault.key - `echo 'key' > vault.key`
* Описать используемые роли директории `roles` или указать в `requirements.yml` и скачать их `ansible-galaxy install -r requirements.yml`
* Написать playbooks в папке `playbooks`
* Создать окружение и заполнить inventory and group_vars
* Запустить `ansible-playbook -i environments/env playbooks/your_playbook.yml`
