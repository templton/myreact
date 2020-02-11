# Мои конфигурации для react

Как создать с нуля свою конфигурацию для разработки на react.

Здесь приведена полная последовательность действий, разделенная на тематические блоки. Если какие-то блоки не нужны, то их можно пропустить.

## Установка git
Это не обязательный шаг. Его можно пропустить, если git не нужен. В дальнейших шагах будет встречено редактирование файла 
.gitignore. Эти шаги можно будет так же пропустить, если вы не устанавливаете git.

## Установка node.js
В первую очередь необходимо установить [https://nodejs.org/ru](https://nodejs.org/ru/)

## Инициализация
Создаем папку проекта и переходим в нее: `mkdir myreact && cd myreact`

По желанию сразу в этой папке можно сделать или новый репозиторий `git init`, или склонировать существующий, или пропустить этот шаг, если вы не уставливали git.

Команда `npm init` и заполняем введенные поля. В результате получаем package.json в корне проекта

```
> npm init
This utility will walk you through creating a package.json file.
It only covers the most common items, and tries to guess sensible defaults.

See `npm help json` for definitive documentation on these fields
and exactly what they do.

Use `npm install <pkg>` afterwards to install a package and
save it as a dependency in the package.json file.

Press ^C at any time to quit.
> package name: (myreact) 
> version: (1.0.0) 
> description: Конфигурации для разработки приложений react
> entry point: (index.js) 
> test command: 
> git repository: (https://github.com/templton/myreact.git) 
> keywords: 
> author: Salamatov Dmitry
> license: (ISC) 
About to write to /home/dima/react/myreact/package.json:

{
  "name": "myreact",
  "version": "1.0.0",
  "description": "Конфигурации для разработки приложений react",
  "main": "index.js",
  "scripts": {
    "test": "echo \"Error: no test specified\" && exit 1"
  },
  "repository": {
    "type": "git",
    "url": "git+https://github.com/templton/myreact.git"
  },
  "author": "Salamatov Dmitry",
  "license": "ISC",
  "bugs": {
    "url": "https://github.com/templton/myreact/issues"
  },
  "homepage": "https://github.com/templton/myreact#readme"
}


> Is this OK? (yes) 

```

Создать файл .gitignore со следующим содержимым

```json
# Файлы и папки операционной системы
.DS_Store
Thumbs.db

# Файлы редактора
.idea
*.sublime*
.vscode

# Вспомогательные файлы
*.log*
node_modules/
```
Здесь нужно небольшое отступление о том, [где хранить исключения для файлов реадктора](docs/gitignore.md).
