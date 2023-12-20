## Исправление коммита.

Если вы опечатались в комментарии или забыли добавить файл и заметили это сразу после того, как закоммитили изменения, вы легко можете это поправить при помощи **commit —amend**. Эта команда добавит все из последнего коммита в область подготовленных файлов и попытается сделать новый коммит. Это дает вам возможность поправить комментарий или добавить недостающие файлы в область подготовленных файлов.

Для более сложных исправлений, например, не в последнем коммите или если вы успели отправить изменения на сервер, нужно использовать **revert**. Эта команда создаст коммит, отменяющий изменения, совершенные в коммите с заданным идентификатором.
Самый последний коммит может быть доступен по алиасу **HEAD**:

`$ git revert HEAD`

Для остальных будем использовать идентификаторы:

`$ git revert b10cc123`

При отмене старых коммитов нужно быть готовым к тому, что возникнут конфликты. Такое случается, если файл был изменен еще одним, более новым коммитом. И теперь **git** не может найти строчки, состояние которых нужно откатить, так как они больше не существуют.

---
**[Оглавление](./readme.md)**  <<**[предыдущая страница](./returning-file-pre-state.md)**  |  **[следующая страница](./remote-repository.md)** >>