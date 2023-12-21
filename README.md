# LR6
##Лабораторная работа №6

**Цель работы:** изучение базовых возможностей системы управления версиями, опыт работы с Git Api,
опыт работы с локальным и удалённым репозиторием.

**Ход работы**

1. Создан аккаунт на сайте GitHub
![рис.1]("Скрины_ОП_ЛР6\Создание аккаунта.png")

2. Создана копия исходного репозитория в личное хранилище
![рис.2]("Скрины_ОП_ЛР6\Создание форка репозитория.png")

3. Настроен клиент Git (введено имя пользователя и email) с помощью команд 'git config --global
user.name <имя>' и 'git config --global user.email <email>'
![рис.3]("Скрины_ОП_ЛР6\Настройка клиента Git.png")

4. Клонирован личный удалённые репозиторий на компьютер при помощи 'git clone'
![рис.4]("Скрины_ОП_ЛР6\клонирование репозитория при помощи clone.png")

5. Добавлен файл через интерфейс GitHub 
![рис.5]("Скрины_ОП_ЛР6\Добавление файла через интерфес Github.png")

Изменения подтянуты в локальный репозиторий (переход в локальный репозиторий - 'cd LR6',
"подтягивание" - 'git pull')
![рис.6]("Скрины_ОП_ЛР6\Подтягивание изменений в локальный репозиторий.png")

> Далее работа продолжена локально
6. Получена история операций веток с помощью 'git log'
для **master**
![рис.7]("Скрины_ОП_ЛР6\Просмотр изменений для ветки master.png")

для **branch1**
![рис.8]("Скрины_ОП_ЛР6\Просмотр изменений для ветки branch1.png")

7. Просмотрены последние изменения ветки master с помощью 'git log --all --graph --oneline'
![рис.9]("Скрины_ОП_ЛР6\Просмотр изменений для ветки master из ветки branch1.png")

8. Выполнено слияние веток при помощи 'git merge branch1', просмотрено состояние проекта с использованием
'git status' и разрешён конфликт по данной ситуации 'git add <file>'
![рис.10]("Скрины_ОП_ЛР6\Конфликт слияния и его решение.png")

9. Удаление побочной ветки после слияния с помощью 'git branch -d <ветка>'
![рис.11]("Скрины_ОП_ЛР6\Удаление побочной ветки.png")

10. Проведены и зафиксированы изменения

Первое изменение
![рис.12]("Скрины_ОП_ЛР6\Первое изменение.png")

Второе изменение
![рис.13]("Скрины_ОП_ЛР6\Второе изменение.png")

Просмотр историй операций с помощью 'git log -2'
![рис.14]("Скрины_ОП_ЛР6\Просмотр историй операций.png")

11. Сделан откат коммита с помощью 'git reset HEAD~1' и проверена история изменений
с помощью 'git log -2'
![рис.15]("Скрины_ОП_ЛР6\Откат коммита.png")

12. Создана ветка для отчёта branch2 с помощью 'git branch branch2'
![рис.16]("Скрины_ОП_ЛР6\Создание  ветки для отчёта.png")

13. Оформление отчёта
![рис.17]("Скрины_ОП_ЛР6\Оформление отчёта.png")

14. История всех операций в форматированном виде
![рис.18]("Скрины_ОП_ЛР6\История операций в форматированном выводе.png")

Лог всех команд:
git config - настройки
git clone - клонирование репозитория
git pull - извлечение и загрузка содержимого из удаленного репозитория
git log --all --graph --oneline - вывод компактного графа истории коммитов
git checkout - переключениt между ветками
git log -p -2 - просмотр историй коммитов с показом изменений, внесенных в каждом коммите
git merge - объединение изменений из одной ветки в другую
git status - показывает состояния файлов в рабочем каталоге
git add - добавление изменений в индекс
git commit -m "Text" - делает для проекта снимок текущего состояния изменений, добавленных в раздел проиндексированных файлов
git branch -d - удаление ветки
git log --date=format:'%D' --pretty=format:"%h - %cd, %cn : %s" - вывод истории коммитов с форматированными данными

**Вывод:**в ходе лабораторной работы были изучены базовые возможности системы управления версиями, также был получен опыт работы с Git Api и опыт работы с локальным и удаленным репозиторием.