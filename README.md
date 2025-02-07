# git_lesson3

**git clone** - клонирование репозитория

## Работа с удаленным репозиторием

 Для работы с удаленным репозиторием необходимо создать страницу на GitHub.
 
 Далее есть три варианта:

 1. Создание удаленного репозитория на сайте и привязка с локальным, 
с возможностью клонировать данные на GitHub


   Команды: 

	git remote add origin https://github.com/efimkrutikhin/Git-lesson_3.git - Связывает локальный репозиторий с удаленным 

	git branch -M main - Сохраняет основную ветку 

	git push -u origin main - первый перенос информации с локального устройства на удаленным (GItHub)

	Дальнейшие сохранения в удаленный реп. возможно просто через git push 

2. Если необходимо клонировать чужой репозиторий на своё локальное устройство достаточно выполнить пару шагов:


    1. Выбираем вкладку "CODE" в правом углу чужого репозитория
    2. Копируем ссылку 
    3. Переходим в собственный проект.:
    3.1. Если репозиторий не создан, то создаем репозиторий в своей папке через git init
    3.2. Если репозиторий уже создан то переходим к 4 пункту
    4. Вводим команду: git clone "Скопированная ссылка"
    5. Поздравляю ты скопировал проект из GitHub на своё локальное устройство


3. Если необходимо внести изменения в чужом репозитории и отправить через pull request на утверждение нужно:

~~~
    1. Выбрать интересующий репозиторий на GitHub
    2. Нажать в правом углу на кнопку "FORK"
    3. Далее появится страница "Создать новый Fork". Создаем!
    4. Переходим на свою страницу и там жмем на появившийся репозиторий с идентичной копией. 
    5. Далее также через git clone копируем себе на локальное устройство. Через git push загружаем результаты на GitHub
    6. Выбираем pull Request и отправляем на утверждением владельцу
~~~

Это самое главное, что нужно знать про удаленные репозитории.
Также есть такая команда, как:

    git pull. Она позволяет перенести новую информацию из удаленного на локальный