## Gitlab CI

### Montando seu próprio Gitlab CI com Docker

~~~
docker pull gitlab/gitlab-ce:9.5.3-ce.0
~~~

~~~
docker pull gitlab/gitlab-runner:v9.5.0
~~~

Explicar a prática de "taggear" as imagens.

~~~
docker run --detach --hostname gitlab.machine.com --publish 443:443 --publish 80:80 --publish 20:22 --name Gitlab_CI --restart always --volume /srv/gitlab/config:/etc/gitlab --volume /srv/gitlab/logs:/var/log/gitlab --volume /srv/gitlab/data:/var/opt/gitlab gitlab/gitlab-ce:9.5.3-ce.0
~~~

Colocar explicação de cada passo da execução acima.
