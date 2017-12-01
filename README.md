# Sass-Build-SublimeText3
Sass поддерживает 4 стиля вывода CSS:
* `:nested` [вложенный] _-default_
* `:expanded` [развёрнутый]
* `:compact` [компактный]
* `:compressed` [сжатый]

# Примеры стилей
**`:nested`**
```
#content {
  margin: 5px;
  background-color: #666; }
  #content p {
    padding: 10px 20px; }
```

**`:expanded`**
```
#content {
  margin: 5px;
  background-color: #666;
}

#content p {
  padding: 10px 20px;
}
```

**`:compact`**
```
#content { margin: 5px; background-color: #666; }
#content p { padding: 10px 20px; }
```

**`:compressed`**
```
#content{margin:5px;background-color:#666}#content p{padding:10px 20px}
```

# Как применить?
Здесь лежит 4 файла, каждый из которых является системой сборки **для Sublime Text 3**. 
#### Способ #1
Скачать архив репозитория [отсюда](https://github.com/alexshink/Sass-Build-SublimeText3/archive/master.zip) и разархивировать 4 файла с расширением `.sublime-build` в специальную директорию редактора:
* **OS X:** `~\Library\Application Support\Sublime Text 3\Packages\User`
* **Win:** `~\AppData\Roaming\Sublime Text 3\Packages\User`
* **Linux:** `~\.Sublime Text 3\Packages\User`

После чего в редакторе во вкладке `Tools -> Build System` появятся пункты, соответствующие названиям добавленных файлов. Стиль вывода Sass активирутеся сразу после выбора системы сборки из списка.

> _если не можешь найти директорию, то Sublime укажет тебе путь: `Preferences -> Browse Packages...`_
 
 #### Способ #2
 `Tools -> Build System -> New Build System...` - в открывшемся файле заменяем всё содержимое текстом необходимой сборки и сохраняем в предложенную редактором папку. После чего во вкладке `Tools -> Build System` появится пункт, соответствующий названию сохранённого файла.
