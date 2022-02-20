# DockerRegistry
```
git clone https://github.com/VGIlyin/DockerRegistry
cd docker-registry/auth
htpasswd -Bc registry.password admin
cat registry.password #checking
docker-compose up -d
```
Набор команд, описанный выше, задеплоит собственный docker registry

Также обращаю внимание, что для базовой авторизации в registry необходимо поднять https прослойку между вами и самим регистром.

Пример конфигурации .conf файла для nginx [example](https://github.com/VGIlyin/DockerRegistry/blob/main/registry.conf)
