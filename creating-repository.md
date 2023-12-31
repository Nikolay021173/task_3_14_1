## Создание нового репозитория.

**Git** хранит свои файлы и историю прямо в папке проекта. Чтобы создать новый репозиторий, нужно открыть терминал, зайти в папку проекта и выполнить команду ***init***. Это включит приложение в этой конкретной папке и создаст скрытую директорию ***.git***, где будет храниться история репозитория и настройки.
Создим на рабочем столе папку под названием ***git_example***. Для этого в окне терминала введем:
```
$ mkdir Desktop/git_example/
$ cd Desktop/git_example/
$ git init
```

Командная строка должна вернуть что-то вроде:

`Initialized empty Git repository in /home/user/Desktop/git_example/.git/`

Это значит, что наш репозиторий был успешно создан, но пока что пуст. Теперь создадим текстовый файл под названием **examp.txt** и сохраним его в директории **git_example**.

---
**[Оглавление](./readme.md)**  << **[предыдущая страница](./git-help.md)**  |  **[следующая страница](./determining-status.md)** >>