## Как сделать коммит.
Допустим нам нужно добавить пару новых блоков в **html-разметку (index.html)** и стилизовать их в файле **style.css**. Для сохранения изменений, их необходимо закоммитить. Но сначала, мы должны обозначить эти файлы для Гита, при помощи команды **git add**, добавляющей (или подготавливающей) их к коммиту. Добавлять их можно по отдельности:

```
git add index.html
git add css/style.css
```
или вместе - всё сразу:

`git add .`

Конечно добавлять всё сразу удобнее, чем прописывать каждую позицию отдельно. Однако, тут надо быть внимательным, чтобы не добавить по ошибке ненужные элементы. Если же такое произошло изъять оттуда ошибочный файл можно при помощи команды

```
git reset:
git reset css/style.css
```
Теперь создадим непосредственно сам коммит

`git commit -m 'Add some code'`

Флажок **-m** задаст **commit message** - комментарий разработчика. Он необходим для описания закоммиченных изменений. И здесь необходимо соблюдать правило всех комментариев в коде: ***«Максимально ясно, просто и содержательно обозначь написанное!»***

---
**[Оглавление](./readme.md)**  <<**[предыдущая страница](./preparing-files.md)**  |  **[следующая страница](./viewing-commits.md)** >>