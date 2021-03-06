[< back](/readme.md)

# git commit

На GitHub сохраненные изменения называются фиксациями (commits). Каждая фиксация (commit) имеет сообщение фиксации, описание, объясняющее, почему было сделано конкретное изменение. Сообщения фиксации фиксируют историю изменений, чтобы другие участники могли понять, что сделано и почему.

После того как командой **git add** файлы добавлены в индекс, команда **git commit** берет эти файлы и сохраняет их точку фиксации во внутренней базе данных.

При каждом коммите формируется хеш коммита. **Хеш коммита (SHA-1)** – это набор символов, строка длиной в 40 шестнадцатеричных символов (0-9 и a-f), который уникален для каждого коммита в данном репозитории. Хеш генерируется автоматически и выглядит примерно так:
```
35a8cb9317568241ca321a43e4789bd5f4c13481
```

При фиксации изменений (commit) необходимо указать сообщение или комментарий.

Командой **git commit** изменения всех файлов, внесённые в индекс, переносятся в репозиторий. 

Ключ **-m** позволяет написать сообщение из командной строки.

Сообщения коммитов пишутся на английском языке.

**Коммиты содержат необходимую информацию о точке фиксации изменений.**

Пример:

``git commit -m "сообщение – commit"`` - ввести сообщение, произведенное действие в повелительном наклонении.

Реальные примеры:
```
git commit -m "Update"
git commit -m "Add description"
```

``` git commit --amend -m "new commit" ``` — добавить изменения, новое название к последнему коммиту.

Параметр **-a** в команде **git commit** автоматически индексирует каждый уже отслеживаемый на момент коммита файл, позволяя обойтись без **git add**. *Новые файлы при этом индексироваться не будут. Удаление файлов будет учтено.*

```
git commit -a -m " commit"
```

Внесение в индекс и создание коммита на основе изменений единственного файла. Пример:

```
git commit readme.md
```