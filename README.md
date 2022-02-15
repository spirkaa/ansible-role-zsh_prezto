# Роль Ansible: zsh Prezto

Роль Ansible, которая устанавливает zsh и [Prezto](https://github.com/sorin-ionescu/prezto).

## Требования

Нет.

## Переменные

    zsh_prezto_repo: https://github.com/sorin-ionescu/prezto.git

Ссылка на репозиторий Prezto

    zsh_prezto_repo_version: HEAD

[Требуемая версия (коммит)](https://docs.ansible.com/ansible/latest/collections/ansible/builtin/git_module.html#parameter-version)

    zsh_prezto_dest: ~/.zprezto

Каталог установки

## Зависимости

Нет.

## Пример плейбука

    - hosts: all
    
      vars:
        zsh_prezto_repo: https://github.com/spirkaa/prezto.git
        zsh_prezto_repo_version: 12f6ac6
    
      roles:
        - spirkaa.zsh_prezto

## Лицензия

MIT / BSD

## Об авторе

2020, [Ilya Pavlov](https://devmem.ru/)
