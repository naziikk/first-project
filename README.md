# first-project
# Git

**VCS -** version control system

**GIT** - global information tracker

- pwd - print working directory
- cd ~ - change directory
- ls - get list of files in directory
- ls ~ - list of files in the home folder
- touch (filename + extension) - create new file
- mkdir new-dir - ***m**a**k**e **dir**ectory*
- cp

```bash
$ cp что_копируем куда_копируем

$ cp index.html src/
# скопировали index.html в папку src
```
---
Пример:

```bash
$ mkdir first-project   
$ touch first-project/data.txt first-project/table.csv
```

Эта запись равноценна поочерёдному вызову следующих команд.

```bash
$ mkdir first-project  
# создали папку

$ touch first-project/data.txt
# создали первый файл

$ touch first-project/table.csv
# создали второй файл
```
---
- mv (from to) - move(works similar to cp)
- mkdir -p - create the structure of a directory
- cat (filename) - concatenate and print
- rm (filename) - remove
- rmdir (dir name) -  remove directory
- rm -r (dir name) - delete folder with all its contents

**Удаление объектов командами `rm` и `rmdir` необратимо — в этом случае файлы и папки не попадают в корзину и исчезают навсегда.**

- **↑ - last command**
- ↓ - return
- (press tab) - automatically offers a list of commands
- ~ - stores a link to the root directory (always)
- git config --global [user.name](http://user.name) - set the user name
- git config --global [user.email](http://user.email) - set email

### Навигация

- `pwd` (от англ. ***p**rint **w**orking **d**irectory*, «показать рабочую папку») — покажи, в какой я папке;
- `ls` (от англ. ***l**i**s**t directory contents*, «отобразить содержимое директории») — покажи файлы и папки в текущей папке;
- `ls -a` — покажи также скрытые файлы и папки, названия которых начинаются с символа `.`;
- `cd first-project` (от англ. ***c**hange **d**irectory*, «сменить директорию») — перейди в папку `first-project`;
- `cd first-project/html` — перейди в папку `html`, которая находится в папке `first-project`;
- `cd ..` — перейди на уровень выше, в родительскую папку;
- `cd ~` — перейди в домашнюю директорию (`/Users/Username`);
- `cd /` — перейди в корневую директорию.

### Работа с файлами и папками

**Создание**

- `touch index.html` (англ. *touch,* «коснуться») — создай файл `index.html` в текущей папке;
- `touch index.html style.css script.js` — если нужно создать сразу несколько файлов, можно напечатать их имена в одну строку через пробел;
- `mkdir second-project` (от англ. ***m**a**k**e **dir**ectory*, «создать директорию») — создай папку с именем `second-project` в текущей папке.

**Копирование и перемещение**

- `cp file.txt ~/my-dir` (от англ. ***c**o**p**y*, «копировать») — скопируй файл в другое место;
- `mv file.txt ~/my-dir` (от англ. ***m**o**v**e*, «переместить») — перемести файл или папку в другое место.

**Чтение**

- `cat file.txt` (от англ. *con**cat**enate and print*, «объединить и распечатать») — распечатай содержимое текстового файла `file.txt`.

**Удаление**

- `rm about.html` (от англ. ***r**e**m**ove*, «удалить») — удали файл `about.html`;
- `rmdir images` (от англ. ***r**e**m**ove **dir**ectory*, «удалить директорию») — удали папку `images`;
- `rm -r second-project` (от англ. ***r**e**m**ove,* «удалить» + ***r**ecursive*, «рекурсивный») — удали папку `second-project` и всё, что она содержит.

### Полезные возможности

- Команды необязательно печатать и выполнять по очереди. Можно указать их списком — разделить двумя амперсандами (`&&`).
- У консоли есть собственная память — буфер с несколькими последними командами. По ним можно перемещаться с помощью клавиш со стрелками вверх (**`↑`**) и вниз (**`↓`**).
- Чтобы не вводить название файла или папки полностью, можно набрать первые символы имени и дважды нажать `Tab`. Если файл или папка есть в текущей директории, командная строка допишет путь сама.
    
    Например, вы находитесь в папке `dev`. Начните вводить `cd first` и дважды нажмите `Tab`. Если папка `first-project` есть внутри `dev`, командная строка автоматически подставит её имя. Останется только нажать `Enter`.
    
- git init - create repository
- rm -rf .git - delete repository
- git status - current status of repository
- git add --all - add all files to repository
- git commit -m ‘message’
- git log - change history
- git remote add origin [git@github.com](mailto:git@github.com):%naziikk%/first-project.git  - link a remote repository to a local repository
- git remote -v - check if they are connected

**SSH key** - security shell key

- ssh-keygen -t ed25519 -C “email” - generate SSH key
- ls -a ~/.ssh - list of SSH’s
- pbcopy < ~/.ssh/id.pab - copy ssh data
