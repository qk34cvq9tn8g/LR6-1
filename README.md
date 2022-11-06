# Лабораторная работа №6

Копирование репозитория(https://github.com/Kurtyanik/LR6/) в свое личное хранилище 
![image](https://user-images.githubusercontent.com/117490646/200180759-b997b603-4448-4b91-8b4a-bd9bf1d98696.png)

Затем нужно настроить клиент git, для этого вводим имя пользователя и email. Комманды: git config --global user.name <username>; git config --global user.email <email>.

![Screenshot_3](https://user-images.githubusercontent.com/117490646/200180770-4b867c08-3bab-461f-beec-2fc0315b893d.png)

Теперь клонируем удалённый репозиторий на компьютер. Комманда: git clone <url>.
![Screenshot_1](https://user-images.githubusercontent.com/117490646/200180789-e2873242-7c3f-4d97-9a85-1ad0c993c545.png)

Переходим в директорию. Комманда: cd LR6/.
Поддтягиваем изменения в локальный репозиторий. Комманда: git pull.
Посмотрим коммиты ветки master. Комманда: git log.

![3](https://user-images.githubusercontent.com/117490646/200180820-7f76cf00-055b-4731-9cc9-81d28bb6229f.png)

Просмотрим существующие ветки в текущем репозитории, затем перейдем в ветку branch1. Комманды: git branch; git checkout branch1.

![4](https://user-images.githubusercontent.com/117490646/200180835-3e4b8399-b2e1-4072-98ce-f065a3b06f36.png)

Посмотрим коммиты ветки branch1. Комманда: git log.

![5](https://user-images.githubusercontent.com/117490646/200180857-68308d66-01c0-44db-af16-e6460275b426.png)

Подробно рассмотрим коммиты. Комманда: git log -p.

![6](https://user-images.githubusercontent.com/117490646/200180869-0d5600fe-8f55-496b-bf2d-579fd12afab8.png)

Выполняем слияние в ветку master. Комманда: git merge branch1.

Разрешаем возникший конфликт: в теории конфликт возник из-за того, что файл mergefile.txt не отслеживается. Проверив это и убедившись, добавляем файл для отслеживания, оставляем коммит. Команды:git status; git add mergefile.txt; git commit -m "Branches".

![7](https://user-images.githubusercontent.com/117490646/200180897-bfef20e3-6d6d-4be6-99a4-eefbf47a56cd.png)

![8](https://user-images.githubusercontent.com/117490646/200180904-c17545be-77d5-4eea-8868-80102b2a5389.png)

Удаляем побочную ветку после успешного слияния. Комманда: git branch -d branch1

![9](https://user-images.githubusercontent.com/117490646/200180919-ac4ce0d3-5990-48fc-bff2-544f486b7441.png)

Создаем изменения и фиксируем их, оставляя комментарии,несколько раз. Команды:echo hello > new.txt/new2.txt; git add new.txt/new2.txt; git commit -m "NEW.txt/NEW2.txt"

![10](https://user-images.githubusercontent.com/117490646/200180932-de87427e-e842-4f3c-9388-21daee71a3a3.png)![11](https://user-images.githubusercontent.com/117490646/200180998-a9a2b893-3696-4f40-abe2-3df48d094381.png)

Просмотр комментариев.

![12](https://user-images.githubusercontent.com/117490646/200181005-a3383b35-642c-47ec-a6b9-1d50844d2d90.png)

Делаем «хард» откат коммита. Комманда: git reset --hard HEAD~1 И создаем ветку для отчёта. Комманда: git branch report

![13](https://user-images.githubusercontent.com/117490646/200181061-be7c0030-ce84-4d19-b761-ed9d289de850.png)

Получаем итоговую историю операций. Комманда: git log

![14](https://user-images.githubusercontent.com/117490646/200181083-3ad966cd-ab1b-4717-bec7-9cb08126481e.png)

После редактирования отчета, его нужно будет сохранить и произвести команды git add и git commit.
В конце работы необходимо будет отправить все локальные изменения в сетевое хранилище GitHub командой git push.

![15](https://user-images.githubusercontent.com/117490646/200181156-6505ccab-63f2-4553-a22d-55f8d55d0626.png)

