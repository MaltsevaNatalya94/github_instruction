 # **Инструкция для работы с Git и удалёнными репозиториями**

## **Что такое Git?**
____
 Git - это одна из реализаций распределённых систем контроля версий, имеющая как и локальные, так и удалённые репозитории. Является самой популярной реализацией систем контроля версий в мире.

## **Подготовка репозитория**
__________________
Для создание репозитория необходимо выполнить команду *git init* в папке с репозиторием и у Вас создаться репозиторий (появится скрытая папка .git)

## **Создание коммитов**
_____________________________
### **Git add**
Для добавления измений в коммит используется команда *git add*. Чтобы использовать команду *git add* напишите *git add <имя файла>*

### **Просмотр состояния репозитория** 
создаем конфликт для pull request

### **Создание коммитов**
Для того, чтобы создать коммит(сохранение) необходимо выполнить команду *git commit*. Выполняется она так: *git commit -m "<сообщение к коммиту>*. Все файлы для коммита должны быть **ДОБАВЛЕНЫ** и сообщение к коммиту писать **ОБЯЗАТЕЛЬНО**.

## **Перемещение между сохранениями**
_____________
Для того, чтобы перемещаться между коммитами, используется команда *git checkout*. Используется она в папке с пепозиторием следующим образом: *git checkout <номер коммита>*

## **Журнал изменений**
__________________
Для того, чтобы посмотреть все сделанные изменения в репозитории, используется команда *git log*. Для этого достаточно выполнить команду *git log* в папке с репозиторием

## **Ветки в Git**
______________
### **Создание ветки**
Для того, чтобы создать ветку, используется команда *git branch*. Делается это следующим образом в папке с репозиторием: *git branch <название новой ветки>*

## **Слияние веток**
_______________________
### **Конфликт слияния**
Для того чтобы дабавить ветку в текущую ветку используется команда *git merge*
Конфликт слияния
Предполагается ситуация: есть ветка master и есть ветка feature. В обеих ветках есть коммиты, сделанные после расхождения веток. В ветку master пытаемся влить ветку feature (git merge feature), получаем конфликт, т.к. в обеих ветках есть изменения одной и той же строки в файле index.html.

При возникновении конфликта, репозиторий находится в состоянии прерванного слияния. Нужно оставить в конфликтующих местах файлов только нужный код, проиндексировать изменения и закоммитить.
## **Удаление веток**
__________________
Здесь формируем конфликт с главной веткой
Создаю конфликт с основной веткой!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!

## Cсылки
Чтобы добавить не нумерованные списка необходимо пункты выделить звездочкой. Например вот так:
* Элемент 1
* Элемент 2
* Элемент 3

Чтобы добавить нумерованные списки, необходимо пункты пронумеровать. 
Например, вот так: 
1. Первый
2. Второй
3. Третий

 # **Картинка**

![<logo>](<https://github.com/adam-p/markdown-here/raw/master/src/common/images/icon48.png>)
# **Оформление текста**
## Выделение текста

Чтобы выделить текст курсивом поставте в * или знак нижнего поддеркивания, например _вот так_
*вот так*

Что бы выделить полужирный в двойные звездочки **вот так** или выделить знаком двойного нижнего подчеркивания, например __вот так__.
Альтернативные способы выделения текста жирным или курсивным чтоб мы могли их совмещать. __*Текст может быть выведен курсивои и при этом быть полужирным.*__

# **Указатели**
 HEAD — указатель на текущий коммит или на текущую ветку (то есть, в любом случае, на коммит). Указывает на родителя коммита, который будет создан следующим.

ORIG_HEAD — указатель на коммит, с которого вы только что переместили HEAD (командой git reset ..., например).
Ветка (master, develop etc.) — указатель на коммит. При добавлении коммита, указатель ветки перемещается с родительского коммита на новый.
Теги — простые указатели на коммиты. Не перемещаются.

# __Управление удаленными репозиториями__
Удаленный (иногда говорят "внешний") репозиторий – это версии вашего проекта, сохраненные на удаленном сервере. Доступ к репозиторию на таком сервере может осуществляться по интернету или по локальной сети.
Чтобы добавить новый удаленный, используйте git remote add команду на терминале в каталоге, в котором хранится ваш репозиторий.

*git remote add*  - Команда принимает два аргумента:

Например, удаленное имя, origin
Например, удаленный URL-адрес, https://github.com/user/repo.git

## **Переименование удаленного репозитория**
Используйте git remote renameкоманду для переименования существующего удаленного хранилища.

*git remote rename* - Команда принимает два аргумента:

Например, существующее удаленное имя, origin
Например, новое имя для удаленного хранилища, destination
