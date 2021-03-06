[< back](/readme.md)

# git branch

Команда **git branch** покажет все ветки на компьютере.

Команда **git branch** используется для управления ветками в репозитории.

Создать новую ветку, например test

```
git branch test
```

Команда **git branch** только создаёт новую ветку, но не переключает на неё.

```git branch -r``` - (remote – удаленный) Выводятся только удаленные ветки.

```git branch -a``` - (all – все) Выводятся и локальные, и удаленные ветки.

```git branch -d test``` – удалить ветку test. Используется, если изменения ветки test уже влиты в главную ветку. Если выполнить команду удаления до слияния — в результате появится сообщение об ошибке. Это защита – предотвращает потерю доступа к файлам.

Если требуется принудительно удалить ветку test независимо от текущего статуса, без предупреждений – используется флаг **-D** (заглавная буква).

```
git branch -D test
```

Данные команды удаляют только локальную копию ветки. В удалённом репозитории она может сохраниться.

Для того чтобы удалить удалённую ветку test, нужно выполнить команду:

```
git push origin --delete test
```