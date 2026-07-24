# Роль развертывания ALDPro 
## aldpro_dc_deploy
Настройка контроллера домена ALDPro.
Перед запуском роли необходимо заполнить файл переменных - aldpro_roles/aldpro_dc_deploy/vars/main.yml
Пример:
```
alse_repo_branch: "frozen" # ветка репозитория frozen или stable
alse_version: "1.7.8" # версия обнолвения astra linux
ald_version : "2.4.2"
domain_name: "test.org" # имя домена
admin_user: "admin" # учетная запись администратора домена для ввода в домен
admin_pass: "P@ssw0rd" # пароль админа
dc_ip: "192.168.0.5" # ip адрес контроллера домена, нужен для инициализации dc
hostname: "{{ ansible_hostname }}" # имя хоста получаемое из фактов ansible
```
