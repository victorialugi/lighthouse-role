# Lighthouse Role

Роль для установки и настройки **Lighthouse**

## Requirements

- Ansible >= 2.10
- Поддерживаемые ОС: CentOS / RHEL / Rocky Linux / AlmaLinux 7, 8, 9
- Установленный и запущенный Nginx

## Role Variables

| Переменная                  | Значение по умолчанию     | Описание |
|-----------------------------|---------------------------|----------|
| `lighthouse_version`        | `0.3.0`                   | Версия Lighthouse |
| `lighthouse_install_dir`    | `/opt/lighthouse`         | Директория установки |
| `lighthouse_nginx_config`   | `true`                    | Создавать конфигурацию nginx |

## Dependencies

- Nginx

## Example Playbook

```yaml
- name: Deploy Lighthouse
  hosts: lighthouse
  roles:
    - lighthouse-role

## License

MIT

## Author Information

Victoria Luginina
