## Отслеживание изменений, сделанных в коммитах.

У каждого коммита есть свой уникальный идентификатор в виде строки цифр и букв. Просмотреть список всех коммитов и их идентификаторов, можно с помощью команды **log**:

`[spoiler title='Вывод git log']`

```
$ git log
commit ba25c0ff30e1b2f0259157b42b9f8f5d174d80d7
Author: Tutorialzine
Date: Mon May 30 17:15:28 2016 +0300
New feature complete
commit b10cc1238e355c02a044ef9f9860811ff605c9b4
Author: Tutorialzine
Date: Mon May 30 16:30:04 2016 +0300
Added content to hello.txt
commit 09bd8cc171d7084e78e4d118a2346b7487dca059
Author: Tutorialzine
Date: Sat May 28 17:52:14 2016 +0300
Initial commit
[/spoiler]
```
Как можно заметить, идентификаторы довольно длинные, но для работы с ними не обязательно копировать их целиком — первых нескольких символов будет вполне достаточно. Чтобы посмотреть, что нового появилось в коммите, мы можем воспользоваться командой **show [commit]**

**[spoiler title='Вывод git show']**

```
$ git show b10cc123
commit b10cc1238e355c02a044ef9f9860811ff605c9b4
Author: Tutorialzine
Date: Mon May 30 16:30:04 2016 +0300
Added content to hello.txt
diff --git a/hello.txt b/hello.txt
index e69de29..b546a21 100644
--- a/hello.txt
+++ b/hello.txt
@@ -0,0 +1 @@
+Nice weather today, isn't it?
```
[/spoiler]

Чтобы увидеть разницу между двумя коммитами, используется команда **diff** (с указанием промежутка между коммитами):
**[spoiler title='Вывод git diff']**

```
$ git diff 09bd8cc..ba25c0ff
diff --git a/feature.txt b/feature.txt
new file mode 100644
index 0000000..e69de29
diff --git a/hello.txt b/hello.txt
index e69de29..b546a21 100644
--- a/hello.txt
+++ b/hello.txt
@@ -0,0 +1 @@
+Nice weather today, isn't it?
```
[/spoiler]

Мы сравнили первый коммит с последним, чтобы увидеть все изменения, которые были когда-либо сделаны. Обычно проще использовать **git difftool**, так как эта команда запускает графический клиент, в котором наглядно сопоставляет все изменения.

---
**[Оглавление](./readme.md)**  <<**[предыдущая страница](./viewing-commits.md)**  |  **[следующая страница](./returning-file-pre-state.md)** >>