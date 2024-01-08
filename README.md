Требования
------------

  * PHP 8.2.0 или выше;
  * включенное PHP-расширение PDO-SQLite;
  * и [обычные требования к приложениям Symfony][2].

Установка
------------

Существует 3 варианта установки проекта в зависимости от ваших потребностей:

**Вариант 1.** [Скачайте Symfony CLI][4] и используйте бинарник `symfony`, установленный
на вашем компьютере для выполнения этой команды:

``bash
$ symfony new --demo my_project
```

**Вариант 2.** [Скачайте Composer][6] и используйте бинарник `composer`, установленный
на вашем компьютере для выполнения этих команд:

``bash
# вы можете создать новый проект на основе проекта Symfony Demo...
$ composer create-project symfony/symfony-demo my_project

# ...или вы можете клонировать репозиторий кода и установить его зависимости
$ git clone https://github.com/symfony/demo.git my_project
$ cd my_project/
$ composer install
```

**Опция 3.** Нажмите на следующую кнопку, чтобы развернуть этот проект на Platform.sh,
официальном Symfony PaaS, чтобы вы могли попробовать его, не устанавливая ничего локально:

<p align="center">
<a href="https://console.platform.sh/projects/create-project?template=https://raw.githubusercontent.com/symfonycorp/platformsh-symfony-template-metadata/main/symfony-demo.template.yaml&utm_content=symfonycorp&utm_source=github&utm_medium=button&utm_campaign=deploy_on_platform"><img src="https://platform.sh/images/deploy/lg-blue.svg" alt="Deploy on Platform.sh" width="180px" /></a>
</p>


Использование
-----




Перед запуском приложения не нужно ничего настраивать. Существует
2 варианта запуска этого приложения в зависимости от ваших потребностей:


**Вариант 1.** [Скачайте Symfony CLI][4] и выполните эту команду:


``bash
$ cd my_project/
$ symfony serve
```


Затем откройте приложение в браузере по указанному URL (<https://localhost:8000> по умолчанию).


**Вариант 2.** Используйте веб-сервер, например Nginx или Apache, для запуска приложения
(прочитайте документацию о [настройке веб-сервера для Symfony][3]).


На вашей локальной машине вы можете выполнить эту команду, чтобы использовать встроенный веб-сервер PHP:

``bash
$ cd my_project/
$ php -S localhost:8000 -t public/
```


Тесты
-----

Выполните эту команду для запуска тестов:

``bash
$ cd my_project/
$ ./bin/phpunit
```


[1]: https://symfony.com/doc/current/best_practices.html
[2]: https://symfony.com/doc/current/setup.html#technical-requirements
[3]: https://symfony.com/doc/current/setup/web_server_configuration.html
[4]: https://symfony.com/download
[5]: https://symfony.com/book
[6]: https://getcomposer.org/