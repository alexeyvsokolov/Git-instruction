[< back](/readme.md)

# git reset
Команда **git reset** убирает из индекса все добавленные в него изменения (в рабочей директории все изменения сохраняются).

Команда **git reset**, используется для отмены изменений. Она изменяет указатель HEAD и, опционально, состояние индекса.

**Эта команда может изменить файлы в рабочем каталоге при использовании параметра --hard, что может привести к потере данных при неправильном использовании!**

**Необходимо убедиться в правильности действий!**

Сбросить весь индекс:

``git reset``

Удалить из индекса определенный файл:

``git reset - file``

Команда git reset используется не только для сбрасывания индекса.
