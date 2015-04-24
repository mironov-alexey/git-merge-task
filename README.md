# Тренировка работы с git

### Что это?

Это репозиторий-задача, для тренировки навыков работы с git на очных тренингах с несколькими участниками.

### 0. Познакомьтесь с проектом


1. Сделайте fork этого репозитория.
2. Склонируйте себе свой форк.
3. Перед вами проект консольного калькулятора. Скомпилируйте и запустите его. Наберите там строчку `2+3`.

### 1. Переключение между ветками

1. Перейдите в ветку `twoargs` — это ветка разработки, в которой калькулятору добавляют функциональности. 
2. Выполните задание в файле `Calculator.cs`.
3. Сделайте commit и push

### 2. Merge без конфликтов

1. Влейте ветку `twoargs` в `master`. Учтите, что в `master` уже успели появиться новые изменения, однако скорее всего вам удастся избежать конфликтов при слиянии.
2. Изучите историю коммитов (командой `git log --graph` или в графическом клиенте). Пронаблюдайте ветвление и слияние ветвей истории.
3. Изучите состав изменений в Merge-коммите, в каком-нибудь графическом клиенте.
4. Сделайте push.


### 3. Rebase, Fast-Forward-Merge и удаление ненужной ветки

1. Перейдите в ветку `errorhandling` — там некоторое время назад начали добавлять корректную обработку ошибочного ввода пользователя.
2. Изучите коммиты этой ветки, чтобы понять, что произошло.
3. Сделайте rebase коммитов с рефакторингом поверх ветки `master`. Естественно, придется разрешить конфликты — следуйте инструкциям git в командной строке.
4. Изучите историю коммитов. Есть ли там ветвления или слияния?
5. Влейте ветку `errorhandling` в `master`. Если вы все сделали верно, то должен получиться fast-forward merge без конфликтов.
6. Удалите ветку `errorhandling` — она больше не нужна.
7. Сделайте push.

### 4. Создание и удаление remote-веток

1. Создайте новую ветку `new` и отправьте ее на сервер командой push.
2. Удалите ветку `errorhandling` и на сервере тоже.


### 5. Что еще сделать, чтобы лучше осовить git?

* Прочитать официальную книгу по git: http://git-scm.com/book/ru/v2
* Пройти игру-квест  https://github.com/hgarc014/git-game
* Пройти интерактивную игру про работу с ветками http://pcottle.github.io/learnGitBranching/
