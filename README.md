# LR6
## Лабораторная работа №6

**Цель работы:** изучение базовых возможностей системы управления версиями, опыт работы с Git Api,
опыт работы с локальным и удалённым репозиторием.

**Ход работы**

1. Создан аккаунт на сайте GitHub
![рис.1](screens_OP_LR6/1.png)

2. Создана копия исходного репозитория в личное хранилище
![рис.2](screens_OP_LR6/2.png)

3. Настроен клиент Git (введено имя пользователя и email) с помощью команд `git config --globaluser.name <имя>` и `git config --global user.email <email>`
![рис.3](screens_OP_LR6/3.png)

4. Клонирован личный удалённые репозиторий на компьютер при помощи `git clone`
![рис.4](screens_OP_LR6/4.png)

5. Добавлен файл через интерфейс GitHub 
![рис.5](screens_OP_LR6/5.png)

Изменения подтянуты в локальный репозиторий (переход в локальный репозиторий - `cd LR6`,
подтягивание - `git pull`)
![рис.6](screens_OP_LR6/6.png)

> Далее работа продолжена локально
6. Получена история операций веток с помощью `git log`
для **master**
![рис.7](screens_OP_LR6/7.png)

для **branch1**
![рис.8](screens_OP_LR6/8.png)

7. Просмотрены последние изменения ветки master с помощью `git log --all --graph --oneline`
![рис.9](screens_OP_LR6/9.png)

8. Выполнено слияние веток при помощи `git merge branch1`, просмотрено состояние проекта с использованием
`git status` и разрешён конфликт по данной ситуации `git add <file>`
![рис.10](screens_OP_LR6/10.png)

9. Удаление побочной ветки после слияния с помощью `git branch -d <ветка>`
![рис.11](screens_OP_LR6/11.png)

10. Проведены и зафиксированы изменения

Первое изменение
![рис.12](screens_OP_LR6/12.png)
 
Второе изменение
![рис.13](screens_OP_LR6/13.png)

Просмотр историй операций с помощью `git log -2`
![рис.14](screens_OP_LR6/14.png)

11. Сделан откат коммита с помощью `git reset HEAD~1` и проверена история изменений
с помощью `git log -2`
![рис.15](screens_OP_LR6/15.png)

12. Создана ветка для отчёта branch2 с помощью `git branch branch2`
![рис.16](screens_OP_LR6/16.png)

13. Оформление отчёта
![рис.17](screens_OP_LR6/17.png)

14. История всех операций в форматированном виде
![рис.18](screens_OP_LR6/18.png)

**Лог всех команд:**
git config - настройки
git clone - клонирование репозитория
git pull - извлечение и загрузка содержимого из удаленного репозитория
git log --all --graph --oneline - вывод компактного графа истории коммитов
git checkout - переключениt между ветками
git log -p -2 - просмотр историй коммитов с показом изменений, внесенных в каждом коммите
git merge - объединение изменений из одной ветки в другую
git status - показывает состояния файлов в рабочем каталоге
git add - добавление изменений в индекс
git commit -m Text - делает для проекта снимок текущего состояния изменений, добавленных в раздел проиндексированных файлов
git branch -d - удаление ветки
git log --date=format:'%D' --pretty=format:%h - %cd, %cn : %s - вывод истории коммитов с форматированными данными

**Вывод:** в ходе лабораторной работы были изучены базовые возможности системы управления версиями, также был получен опыт работы с Git Api и опыт работы с локальным и удаленным репозиторием.