# first_ansible_role

Роль генерирует Nginx-конфигурацию на контроллере в
`artifacts/<inventory_hostname>/nginx.conf`. Вызывайте её в play
с `connection: local`, `gather_facts: false`.

Настройки и значения по умолчанию находятся в `defaults/main.yml`.
Переопределяйте их через `group_vars`. Для проверки IP нужна коллекция
`ansible.utils` 6.0.0 и Python-пакет `netaddr`.
Установка роли через Galaxy зафиксирована на теге `v1.0.0` в SPO.
