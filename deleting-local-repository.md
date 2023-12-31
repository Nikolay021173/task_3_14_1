## Удаление локального репозитория.

Для этого надо удалить скрытую папку ***«.git»*** в корневом каталоге репозитория. Сделать это можно 3 способами:

Проще всего вручную удалить эту папку ***«.git»*** в корневом каталоге ***«Git Local Warehouse»***.

Также удалить репозиторий можно на **github**. Открываете нужный вам объект и переходите в пункт меню Настройки. Там, прокрутив ползунок вниз, вы попадете в **зону опасности**, где один из пунктов будет называться **«удаление этого хранилища»**.

Последний метод удаления локального хранилища через командную строку, для этого в терминале необходимо ввести следующую команду:
```
cd repository-path/
rm -r .git
```

---
**[Оглавление](./readme.md)**  <<**[предыдущая страница](./requesting-changes-server.md)**  |  **[следующая страница](./branching.md)** >>