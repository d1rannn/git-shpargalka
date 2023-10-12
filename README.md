# Краткая шпаргалка для работы с GitBash (в основе бесплатного курса Yandex.Practicum)

### Написал d1rannn и специально для d1rannn 

Краткая шпаргалка для использования кодов Bash чтобы когда забыл посмотреть и сразу же вспомнить как и каким очередностем вводить команды. В общем полезно кратко и ясно. 
В кратце пройдемся что такое Git и почему это надо?

> Git (произносится «гит»[7]) — распределённая система управления версиями. Проект был создан Линусом Торвальдсом для управления разработкой ядра Linux, первая версия выпущена 7 апреля 2005 года. На сегодняшний день его поддерживает Джунио Хамано.

Среди проектов, использующих Git, — ядро Linux, Swift, Android, Drupal, Cairo, GNU Core Utilities, Mesa, Wine, Chromium, Compiz Fusion, FlightGear, jQuery, PHP, NASM, MediaWiki, DokuWiki, Qt, ряд дистрибутивов Linux.

Программа является свободной и выпущена под лицензией GNU GPL версии 2. По умолчанию используется TCP порт 9418.

Вот так и пишет [Википедия](https://ru.wikipedia.org/wiki/Git)

Но, если говоря по проще, Git это система управления версиями. Ты можешь с помощью гит управлять, всяческий манипулировать версиями какого-то иного проекта, просматривать кто, когда сделал изменения и отслеживать ветки версий проекта. Гит особенно хорош при работе с командами, но это не значит то, что ты не можешь урпавлять не работая в команде. Гит также тебе дает возможность работать над своим проектом и также отслеживать версий. Коротко говоря Гит дает тебе очень большые возможности при работе с версиями. ЖЖ

Давайте перейдем какие команды есть в GitBash:

`git init` -> Делает папку в репозиторий

`pwd` -> Показывает где ты находишься сейчас 

`cd (Путь к репозиторию)` -> Смена к репозиторию где ты хочешь быть

`rm -rf .git` -> Разгитить если все пошло хуево 

`git status`-> Статус репозитория

`touch (Название.расширение)` -> Создает файл 

А тут самое нужное. Это вплоть от создания файла + коммита репозитория и до загружения репозитория в ГитХаб.

 `cd ~/dev`

 `mkdir (Name of directory)`

 `cd (Name of directory)`

 `git init`

 `touch README.md`

 `git add README.md`

 `git commit -m 'Добавить README'`

 `git add remote origin (url)`

 `git push -u origin master`

 `git log` - Просмотр списков коммитов 

 `git log --oneline` - Просмотр списков коммитов, но кратко 

	#### Статусы в Git

 В Git есть несколько состояния статусов: 

> untracked / tracked - неотслеживаемый / отслеживаемый 

> modified - измененный 

> staged - подготовленный 

> Если кратко, то каждый коммиченный файл сначало становиться неотслеживаемым, после как мы пишем команду `git add` то оно становиться неотслеживаемо-подготовленным, а если соответственно изменить файл, то после просмотра через `git log` оно будет измененным в зависимости что вы делали. 
Как вы заметили статусы могут быть парами, то есть (modified + staged, untracked + modified)  и так далее. 


	#### HEAD - это голова! А Commit всему голова! 

 Файл `HEAD` (англ. «голова», «головной») — один из служебных файлов папки .git. Он указывает на коммит, который сделан последним (то есть на самый новый). 

 `HEAD` — это файл в .git, в файле — ссылка, по ссылке — хеш. Совсем как в сказке: иголка — в яйце, яйцо — в утке, утка — в зайце.
 
 `HEAD` указывает на последний коммит. Если передать его в качестве параметра, Git поймёт вас.



