[< back](/readme.md)

# git clone

Команда **git clon** создает копии локального и удаленного репозитория.

Для начала работы с центральным репозиторием, следует создать копию оригинального проекта со всей его историей локально.

```git clone [url]``` — Клонировать (загрузить) репозиторий, который уже существует на GitHub, включая все файлы, ветви и коммиты в одноименную директорию

Пример:
```
git clone https://github.com/name-example/example
```

Клонировать удаленный репозиторий в директорию «Name»

```
git clone https://github.com/name-example/example.git Name
```

Клонирование определенной ветки репозитория
```
git clone https://github.com/ name-example/example.git -b branch-name
```
