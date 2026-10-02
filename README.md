
1. `# H1` — заголовок 1
2. `## H2` — заголовок 2
3. `### H3` — заголовок 3
4. `#### H4` — заголовок 4
5. `##### H5` — заголовок 5
6. `###### H6` — заголовок 6
7. `**жирный**` — жирный текст
8. `*курсив*` — курсив
9. `***жирный курсив***` — жирный курсив
10. `~~зачёркнутый~~` — зачёркнутый
11. `` `код` `` — код в строке
12. `> цитата` — цитата
13. `- элемент` — маркированный список
14. `1. элемент` — нумерованный список
15. `  - вложенный` — вложенный список
16. `- [ ] задача` — чекбокс не выполнен
17. `- [x] задача` — чекбокс выполнен
18. `[текст](url)` — ссылка
19. `[текст](url "подсказка")` — ссылка с подсказкой
20. `![alt](image.png)` — изображение
21. ` ```язык ... ``` ` — блок кода
22. `| a | b |` — таблица (строка)
23. `|---|---|` — таблица (разделитель)
24. `---` — горизонтальная линия
25. `***` — горизонтальная линия
26. `___` — горизонтальная линия
27. `\*` — экранирование символа
28. `<br>` — перенос строки
29. `&nbsp;` — неразрывный пробел
30. `[^1]` — сноска

---

## 🔧 Git — настройка

31. `git config --global user.name "Имя"` — задать имя
32. `git config --global user.email "email"` — задать email
33. `git config --list` — показать настройки
34. `git config --global core.editor "nano"` — задать редактор
35. `git config --global alias.st status` — создать алиас

## 📁 Git — создание репозитория

36. `git init` — инициализировать репозиторий
37. `git clone <url>` — клонировать репозиторий
38. `git clone <url> <папка>` — клонировать в папку
39. `git clone --depth 1 <url>` — поверхностный клон

## 📊 Git — состояние и история

40. `git status` — статус файлов
41. `git status -s` — краткий статус
42. `git log` — история коммитов
43. `git log --oneline` — краткая история
44. `git log --graph --oneline --all` — граф веток
45. `git log -n 5` — последние 5 коммитов
46. `git log --author="Имя"` — коммиты автора
47. `git log --since="2 weeks ago"` — за период
48. `git log -p <файл>` — история файла с изменениями
49. `git diff` — изменения в рабочей директории
50. `git diff --staged` — изменения в индексе
51. `git diff <ветка1> <ветка2>` — разница между ветками
52. `git show <commit>` — информация о коммите
53. `git blame <файл>` — кто менял строки
54. `git grep "текст"` — поиск в файлах

## 📝 Git — добавление и коммит

55. `git add <файл>` — добавить файл
56. `git add .` — добавить всё в текущей папке
57. `git add -A` — добавить всё (вкл. удаления)
58. `git add -p` — добавить по частям
59. `git commit -m "сообщение"` — коммит
60. `git commit -am "сообщение"` — add + commit
61. `git commit --amend` — изменить последний коммит
62. `git commit --amend -m "новое"` — изменить сообщение
63. `git commit --allow-empty -m "msg"` — пустой коммит

## 🌿 Git — ветки

64. `git branch` — список веток
65. `git branch -a` — все ветки (вкл. удалённые)
66. `git branch <имя>` — создать ветку
67. `git branch -d <имя>` — удалить ветку
68. `git branch -D <имя>` — удалить принудительно
69. `git branch -m <новое>` — переименовать ветку
70. `git checkout <ветка>` — переключиться
71. `git checkout -b <ветка>` — создать и переключиться
72. `git checkout <commit>` — перейти к коммиту
73. `git switch <ветка>` — переключиться (новый синтаксис)
74. `git switch -c <ветка>` — создать и переключиться
75. `git merge <ветка>` — слить ветку в текущую
76. `git merge --no-ff <ветка>` — слить без fast-forward
77. `git rebase <ветка>` — перебазирование
78. `git rebase -i HEAD~3` — интерактивный rebase

## 🌐 Git — удалённые репозитории

79. `git remote -v` — список удалённых
80. `git remote add origin <url>` — добавить remote
81. `git remote remove origin` — удалить remote
82. `git remote rename old new` — переименовать remote
83. `git push origin <ветка>` — отправить ветку
84. `git push -u origin <ветка>` — отправить + связать
85. `git push` — отправить в связанную ветку
86. `git push --force` — принудительный push
87. `git push --force-with-lease` — безопасный force
88. `git push origin --delete <ветка>` — удалить ветку на сервере
89. `git pull` — забрать + слить
90. `git pull origin <ветка>` — забрать конкретную
91. `git pull --rebase` — забрать с rebase
92. `git fetch` — забрать без слияния
93. `git fetch --all` — забрать все remote

## 🔄 Git — отмена изменений

94. `git restore <файл>` — отменить изменения в файле
95. `git restore --staged <файл>` — убрать из индекса
96. `git reset <файл>` — убрать из индекса
97. `git reset --soft HEAD~1` — отменить коммит, оставить изменения
98. `git reset --mixed HEAD~1` — отменить коммит и индекс
99. `git reset --hard HEAD~1` — отменить коммит и изменения ⚠️
100. `git reset --hard <commit>` — вернуться к коммиту ⚠️
101. `git revert <commit>` — создать обратный коммит
102. `git clean -n` — показать, что будет удалено
103. `git clean -fd` — удалить неотслеживаемые файлы
104. `git checkout -- <файл>` — отменить изменения (старый способ)

## 📦 Git — stash

105. `git stash` — спрятать изменения
106. `git stash save "название"` — спрятать с названием
107. `git stash list` — список stash
108. `git stash pop` — вернуть и удалить из stash
109. `git stash apply` — вернуть, оставить в stash
110. `git stash drop` — удалить stash
111. `git stash clear` — очистить все stash
112. `git stash show -p` — показать содержимое stash

## 🏷️ Git — теги

113. `git tag` — список тегов
114. `git tag v1.0.0` — создать тег
115. `git tag -a v1.0.0 -m "версия"` — аннотированный тег
116. `git push origin v1.0.0` — отправить тег
117. `git push --tags` — отправить все теги
118. `git tag -d v1.0.0` — удалить тег
119. `git checkout v1.0.0` — перейти к тегу

## 🆘 Git — прочее

120. `git help <команда>` — справка
121. `git reflog` — история HEAD (спасение)
122. `git cherry-pick <commit>` — применить коммит
123. `git submodule add <url>` — добавить подмодуль
124. `git submodule update --init` — инициализировать подмодули
125. `git archive -o file.zip HEAD` — архив репозитория
126. `git bisect start` — бинарный поиск бага
127. `git gc` — сборка мусора
128. `git fsck` — проверка целостности
129. `git count-objects -v` — размер репозитория
130. `git shortlog -sn` — статистика по авторам

---

## 🔥 Частые сценарии

131. `git init && git add . && git commit -m "first"` — создать и закоммитить
132. `git branch -M main` — переименовать ветку в main
133. `git remote add origin <url> && git push -u origin main` — связать и запушить
134. `git checkout main && git pull && git merge feature && git push` — слить feature
135. `git remote add upstream <url> && git fetch upstream && git merge upstream/main` — обновить форк
136. `git reset --soft HEAD~1` — отменить последний коммит, сохранив изменения
137. `git commit --amend --no-edit` — дополнить последний коммит
138. `git push origin --delete <ветка>` — удалить удалённую ветку
139. `git stash && git checkout main && git pull && git checkout - && git stash pop` — сменить ветку с изменениями
140. `git log --oneline --graph --decorate --all` — красивая история
