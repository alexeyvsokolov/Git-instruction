[< back](/readme.md)

# git init

Команда **git init** создаёт в текущей директории (папке) новую поддиректорию (скрытую папку) **.git**, в которой содержатся все файлы репозитория (структура Git-репозитория - служебные файлы Git). Команда создает пустой репозиторий на компьютере.

**С этой команды начинается работа с Git.** Например, если создан проект на компьютере и требуется отправить его на удаленный репозиторий, используется команда **git init**.

Команда **git init** не изменяет проект в папке, в которой запускается команда, так как все основные файлы, необходимые git, хранятся в каталоге **.git**, который создает команда **git init**.

Не требуется создавать репозиторий на сервере, чтобы начать работать с репозиторием git, можно просто перейти в папку проекта и запустить команду **git init**.

Указать каталог, в котором должен быть инициализирован новый репозиторий

```
git init <папка>
```

Например, требуется инициализировать репозиторий в папке с именем e-project

```
git init e-project
```

Когда запускается данная команда, папка **.git** создается в папке e-project, а не в текущем рабочем каталоге.
