## Справочная информация по GIT.

Прежде чем рассматривать тему создания репозитория, обсудим как отобразить в терминале полезную информацию о самом Git, для этого в командной строке наберём ***git help***:

```$ git help```
```
usage: git [--version] [--help] [-C <path>] [-c <name>=<value>]
           [--exec-path[=<path>]] [--html-path] [--man-path] [--info-path]
           [-p | --paginate | -P | --no-pager] [--no-replace-objects] [--bare]
           [--git-dir=<path>] [--work-tree=<path>] [--namespace=<name>]
           <command> [<args>]
...
```

Мы также можем проверить руководство для конкретной команды несколькими способами:

1. $ git --help init
2. $ git help init
3. $ git init --help

Все три приведенных выше варианта возвращают одинаковый результат.

С опцией **-g** можно получить доступ к списку внутренних руководств для развития навыков:

```$ git help -g```
```
The common Git guides are:
   attributes          Defining attributes per path
   cli                 Git command-line interface and conventions
   core-tutorial       A Git core tutorial for developers
...
$ git help core-tutorial
```
Для распечатки учебник, нужно указать его имя в качестве параметра.

---
**[Оглавление](./readme.md)**  << **[предыдущая страница](./installing-git.md)**  |  **[следующая страница](./creating-repository.md)** >>
