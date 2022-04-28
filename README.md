# Healthcheck

monitoring cron jobs

## Getting started

### Project "https://github.com/healthchecks/healthchecks.git"


Заполнить переменный в main.yml 

  vars:
* DOMAIN: "YOUR SITE NAME"
* SCHEMA: "https"
* ssl_fullchain: "crt.cert"
* ssl_key: "key.cert"
  
Используеться уже имеющийся сертификат 
Если сертификатов нет нужно убрать в разделе `roles` 'certs'
В темплейте nginx разкоментить 

`#    include snippets/snakeoil.conf;`

В роли project заполнить переменные /roles/project/defaults/main.yml
