# Подготовка файлов
В git есть концепция области подготовленных файлов. Можно представить ее как холст, на который наносят изменения, которые нужны в коммите. Сперва он пустой, но затем мы добавляем на него файлы (или части файлов, или даже одиночные строчки) командой add и, наконец, коммитим все нужное в репозиторий (создаем слепок нужного нам состояния) командой commit.
В нашем случае у нас только один файл, так что добавим его:

*$ git add hello.txt*

Если нам нужно добавить все, что находится в директории, мы можем использовать

*$ git add -A*

Проверим статус снова, на этот раз мы должны получить другой ответ:

>git status

>On branch master

>Initial commit

>Changes to be committed:

>(use "git rm --cached ..." to unstage)

>new file: hello.txt