## S2. Хранятся состояния директории, постепенная сборка коммита
#### Хранятся файлы, разница вычисляется на лету
#### Commit index для сборки коммита
- `git add .` — добавить все измененные файлы в индекс
- `git commit -m <msg>` — записать изменения из индекса в репозиторий
- `git status -sb` — вывести состояние директории и индекса кратко с указанием текущей ветки
- `git restore .` или `git checkout .` — отменить изменения в директории по индексу
- `git restore -S .` или `git reset .` — отменить изменения индекса по коммиту (отмена `git add .`)
- `git rm <filename>` — удалить файл из индекса, чтобы перестать хранить его историю в репозитории'
- `git show <commit>` — показать содержимое коммита
- `git log --oneline --decorate --graph` — вывести историю коммитов от HEAD в виде дерева
- `git log --oneline --decorate --graph --all` — вывести историю всех коммитов в виде дерева
-  `gitk` — открыть графическое представление репозитория
-  `git clean` — удалить неотслеживаемые файлы из директории