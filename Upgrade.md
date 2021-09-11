![image-20210506104427925](https://tva1.sinaimg.cn/large/008i3skNgy1gq8sv4q7cqj303k03kweo.jpg)

### Deployar nueva versión

**Requisitos**

* nodejs

  https://nodejs.org/it/download/

* docker

  ```
  /bin/bash -c "$(curl -fsSL https://get.docker.com)"
  ```

* git

  ```
  Debian
  apt install git
  CentOS
  yum install git
  ```

  

**Instalar heroku**

```
npm i -g heroku
heroku login -i
heroku container:login
```

**Deployar nueva versión**

```
git clone https://github.com/aitorroma/n8n-heroku
cd n8n-heroku
heroku container:push web --arg N8N_VERSION=0.137.0 --app app-name
heroku container:release web --app app-name
```



## Invitación a mi Canal.

Estás invitado a mi canal de telegram, donde publico más soluciones como esta.

![Telegram-icon](https://tva1.sinaimg.cn/large/008i3skNgy1guctnvd002j600w00w0r202.jpg)https://t.me/aitorroma

----------------------------------------------------------

[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/J3J64AN17)

