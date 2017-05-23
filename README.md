# restream study

[![Build Status](https://travis-ci.org/Restream/study.svg?branch=master)](https://travis-ci.org/Restream/study)

## Запуск проекта

```
bundle install
bundle exec rake test
bundle exec rubocop
```

## Задача

1. Сделать форк проекта к себе в аккаунт.

2. В дирректории с вашим именем есть задачи, каждая в отдельной поддиректории.

  По умолчанию все тесты во всех задачах пропускаются. Чтобы начать работу нужно удалить `skip` из тесткейса.

  Далее для каждой из задач реализовать недостающие методы так, чтобы все тесты проходили. Дополнительную информацию можно найти в комментарии к тесту.
  
  Проверять можно запуская `bundle exec rake test`

3. После того как все тесты проходят, нужно создать pull request в основной репозиторий.

|Method|Pros|Cons|Software|
|---|---|---|---|
|With docker-machine and with [virtual box](https://www.virtualbox.org/) as backend for virtualization.|simplest and free way.|rather slowly|docker, docker-compose, docker-machine, virtualbox|
|With docker-machine and with [parallels](http://www.parallels.com/) as backend for virtualization|fast|not free|docker, docker-compose, docker-machine, parallels Pro or Business edition, [parallels driver for docker](https://github.com/Parallels/docker-machine-parallels)
|[Docker for mac](https://docs.docker.com/docker-for-mac/install/) with [docker-sync](http://docker-sync.io/)|without docker machine, all ports bind on local machine, lightweight, close to native speed| difficult to configure |docker, docker-compose, xhyve, docker-sync|
