![описание картинки](img/git2.png)

# MARKDOWN
Расширение Markdown имеет .md\
"#" - отвечает за размер текста (используем без ковычек в начале строки)\
Пример вставки ссылок и картинок:

    Мы учимся в [текст ссылки](ссылка) - ссылки

    ![описание картинки](ссылка) – картинки

# GIT - команды настройки

**Git –version** – информация о установленной версии Git\
**git config --global user.name "Name Surname"** – любые изменения будут подписаны именем\
**git config --global user.email email@email.com** – любые изменения будут подписаны почтой\
**git config --global –list** – позволит увидеть список того, что уже настроено\
**git config --global core.autocrlf true** – добавить при установкеgit **config --global core.safecrlf warn** – добавить при устоновке\
**git config --global core.quotepath off** – поможет избежать нечитаемые строки в неправильной кодировке\
**git config --global init.defaultBranch main** – говорит о том, что главная ветка будет называться main\
**git help -g – Git** даст подсказку по всем доступным командам\
**git help команда - Git** даст подсказку к определенной команде\
Чтобы выйти из справки нажать Q\

# GIT - команды для работы с локальным репо

**git init** – создает локальный репозиторий(прикрепляет Git к папке)\
**git status** – проверка текущего состояния репозитория\
**git add + имя файла** – добавляет файл в отслеживаемые Git\
**git commit -m “Имя репозитория(подпись коммита)”** – Git коммитит файл\
**git log –oneline** – Просматривается история проектов в коротком формате\
**git log** – в длинном формате\
**git commit --amend -m ”Правильная подпись”** – исправление подписи\
**git add -A** – Добавление в отслеживание сразу много файлов, в коммит попадут все файлы, из текущей папки, которые изменились с последнего коммита.\
**git checkout +хеш коммита** – Переключение на нужный коммит\
**git log -all (--oneline)** – Git покажет всю историю проекта\
**git checkout – (main)** – Git вернется на последний коммит\

# GIT - работа с удаленным репо на GITHAB

**ssh-keygen** – выведет ключ, на строке Your public key скопировать начиная с /.ssh\
**cat ~скопированный ключ** – далее выведет полноценный ключ, который нужно скопировать\
**git remote -v** – проверка списка связей \
**git remote add origin ссылка на репозиторий** – создание связи между локальным и удаленным репозиторием\
**git remote remove origin** – удаление связи\
**git push -u origin main** – отправка файла в удаленный репозиторий\
**git clone скопированная ссылка** – создает копированные репозиторий\
**cd (..)имя папки** – перемещение между папками не выходя из терминала\
**git clone ссылка на форк** – копирование файла на компьютер\
**git branch** – показывает существующие ветки проекта\
**git branch имя ветки** – создает ветку \
**git checkout имя ветки** – перемещение в другую ветку\
**git log имя ветки –graph –oneline** – просмотреть историю ветки\
**git merge имя ветки** – слияние ветки с основным файлом (делается когда мы на файле main)\
**git push** – обновление проекта на GitHub, вводится в дальнейшем, после его добавления на платформу\
**git checkout -b** имя ветки – позволяет создать ветку и сразу в нее попасть\
**Initial commit** – принятое название первого коммита\
**git commit -a -m “имя коммита”** – позволяет сразу добавить измененные файлы и создать коммит\
**git branch -a** – посмотреть все ветки, включая в удаленном репозитории\
**ls** – позволяет посмотреть как добраться до нужной области через консоль
**esc :wq enter** – разрешение конфликта на консоле с подписью во время слияния файлов в удаленном репозитории\
**git clone** скопированная ссылка имя папки – позволяет клонировать папку и сразу дать ей название\
**git pull** – при конфликте, создает еще один коммит с изменениями и именем подписи\
**git revert хеш коммита** – отменяет изменения, которые были внесены в последний коммит\
**.gitignore** -файл который нужно создать в основной папке и записать в него нужную папку/файл для игнорирования Git (пример папки “private/”, пример файла “README.md”)\
**git rm --cached имя файла** – убирает файл из индекса (git add -A), тем самым удаляет его из отслеживаемых, но оставляет на компьютере\
