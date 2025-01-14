# Инструкция по работе с Git 

## Что это и для чего может быть нужно?

**Git** это самая популярная система контроля версий, которая сильно упрощает жизнь. Она помогает отслеживать историю изменений в файлах. Git используют программисты для совместной работы над проектами. Git — один из видов систем контроля версий (или СКВ). Такие системы записывают изменения в набор файлов, а позже позволяют вернуться к определенной версии.


Возможности, кoторые даёт Git:

* хранить различные версии проекта
* возвращаться к различным версиям проекта
* работать в команде

Всё это и есть контроль версий. 

**Git** сохраняет в памяти не файлы целиком, а разницу между файлами.

Итак, что потребуется для начала работы?

- Установить на ПК Git и, например, VS Code
- Настроить их

Первое, что нужно сделать, — настроить имя пользователя и email для идентификации. Эти настройки хранятся в конфигурационном файле. Имя пользователя - git

config --global user.name, а email -  git config --global user.email .

Осваивать Git проще в процессе редактируя текстовые файлы c помощью Markdown – языка разметки и его синтаксиса,

который позволяет форматировать текст в редакторе VS Code.


## Создаём Git-репозиторий

  *Репозиторий*  — это все файлы, находящиеся под контролем версий, вместе с историей их изменения и другой служебной информацией. Репозиторий мы создадим, выбрав любую папку на компьютере. 
  Однако прежде чем создавать репозиторий и инициализировать Git, проверим текущую установленную версию пограммы. Для этого в терминале введём команду: git --version . Если Git установлен на компьютер, мы увидим его текущую версию.

 Команда git init - инициализация: указываем папку, в которой git начнёт отслеживать изменения


 Команда git commit - зафиксировать или сохранить

 ## Что такое коммит?

  По-английски commit значит *«фиксировать»*. Git-коммит — это операция, которая берет все подготовленные изменения и отправляет их в репозиторий как единое целое.

 Зачем нужен коммит, если Git и так следит за всеми изменениями? *Коммиты* разбивают процесс разработки, состоящий из большого количества правок, на отдельные шаги. То есть *коммит* — это некое логически завершенное изменение внутри проекта и понятная (в том числе и другим разработчикам) точка, к которой можно вернуться, если возникнут какие-то проблемы.


 Команда git log - журнал изменений. 

 Переключиться между изменениями поможет git checkout. Для работы нужно указать не только интересующий коммит, но и вернуться в тот, где работаем, при помощи

 команды git checkout master.

 Нажатие клавиши "q" возвращает в исходное окно терминала.

 Команда git diff показывает разницу между текущим файлом и сохранённым. Перед переключением версии файла в Git используйте команду git log, чтобы увидеть количество сохранений. 


# Синтаксис языка разметки Markdown

_*Markdown*_ предназначен для ознакомления пользователя с функциональными возможностями языка разметки Markdown. Markdown – это облегченный язык разметки, который является инструментом преобразования кода в HTML. Главной особенностью данного языка является максимально простой синтаксис, который служит для упрощения написания и чтения кода разметки, что, в свою очередь, позволяет легко его корректировать.

Markdown не является заменой HTML. Синтаксис Markdown достаточно ограничен, и соответствует лишь небольшому подмножеству элементов HTML.

## Параграф

 Для того, чтобы создать параграф с использованием синтаксиса языка Markdown, достаточно отделить строки текста одной (или более) пустой строкой (пустой считается всякая строка, которая не содержит в себе ничего, кроме пробелов и символов табуляции).
 Для того, чтобы вставить видимый перенос строки, необходимо окончить строку двумя пробелами и нажатием клавиши «Enter». Многие элементы синтаксиса Markdown выглядят и работают гораздо лучше в случае, когда их форматируют с помощью жесткого перевода строк. 
                                                                        
## Курсив и полужирный

 Чтобы выделить текст курсивом, необходимо обрамить его звёздочками(*) или знаком нижнего подчёркивания (_).
  Например, *вот так*, или _вот так_.

  Чтобы выделить текст полужирным, необходимо обрамить его двойными звёздочками (**) или двойным знаком нижнего подчёркивания.
  **вот так** или __вот так__.

  ## Заголовки

 Рассмотрим один из вариантов разметки заголовка в Markdown - с помощью символа («#»). Используется от одного до шести данных символов, которые устанавливаются в начале строки (перед заголовком). В данном случае количество символов соответствует уровню заголовка. Кроме того, заголовок возможно снабдить закрывающимися символами («#»), хотя это и не является обязательным. Количество закрывающихся символов не обязано соответствовать количеству начальных символов. Уровень заголовка определяется по количеству начальных символов.

 ## Списки  

Чтобы добавить нумерованные списки - необходимо списки просто 

пронумеровать, например: 

  1. Первый пункт
  2. Второй пункт
  3. Третий пункт


Чтобы добавить ненумерованные списки — необходимо пункты выделить

звёздочкой (*). Например, вот так:

* Элемент 1
* Элемент 2
* Элемент 3
  
Git отслеживает файлы по имени 
Если изменить имя файла, необходимо добавить файл с новый именем + git commit.
  

## Работа с изображениями

Чтобы вставить изображение в текст, достаточно написать следующее:![Привет, это тефтелька!](teftelka.jpg) - и в правом окне уже добавилась картинка:).

# Работа с удалёнными репозиториями. Скачивание из текущего репозитория и слияние со своей версией.

Копировать внешний репозиторий на свой ПК можно с помощью команды 
git clone адрес репозитория, который копируем на свой ПК
Команда git clone составная: она не только загружает изменения, но и сливает ветки на локальном компьютере и в удалённом репозитории. 

git pull скачает всё из текущего репозитория и автоматически сделает merge с нашей версией.

git push отправит нашу версию репозитория на внешний репозиторий (требует авторизации на внешнем репозитории)

## Как настроить совместную работу?

1. Создать аккаунт на github.com
2. Далее создать локальный репозиторий 
3. "Подружить" наш локальный и удалённый репозитории
4. Отправить(push) наш локальный репозиторий в удалённый (на github).
5. Провести изменения с другого компьютера
6. Выкачать (pull) актуальное сосотояние из удалённого репозитория.


## pull request 
- команда для предложения изменений
- запрос на вливание изменений в репозиторий

## Как сделать pull request

* Делаем fork (ответвление) репозитория
* Далее делаем git clone *cвоей* версии репозитория
* Создаём новую ветку и в *неё* вносим свои изменения
* Фиксируем изменения (делаем коммиты)
* Отправляем свою версию в свой GitHub
* На сайте GitHube нажимаем кнопку pull request




