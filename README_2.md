# Домашнее задание к занятию «Что такое DevOps. СI/СD - С.Яремко»

1. Инструкция по выполнению домашнего задания.  
2. Сделайте fork репозитория c шаблоном решения к себе в GitHub и переименуйте его по названию или номеру занятия, например, https://github.com/имя-вашего-репозитория/gitlab-hw или https://github.com/имя-вашего-репозитория/8-03-hw.  
3. Выполните клонирование этого репозитория к себе на ПК с помощью команды git clone.  
4. Выполните домашнее задание и заполните у себя локально этот файл README.md:
  впишите сверху название занятия, ваши фамилию и имя;  
  в каждом задании добавьте решение в требуемом виде — текст, код, скриншоты, ссылка.  
  для корректного добавления скриншотов используйте инструкцию «Как вставить скриншот в шаблон с решением»;  
  при оформлении используйте возможности языка разметки md. Коротко об этом можно посмотреть в инструкции по MarkDown.  
5. После завершения работы над домашним заданием сделайте коммит git commit -m "comment" и отправьте его на GitHub git push origin.  
6. Для проверки домашнего задания в личном кабинете прикрепите и отправьте ссылку на решение в виде md-файла в вашем GitHub.  
7. Любые вопросы по выполнению заданий задавайте в чате учебной группы или в разделе «Вопросы по заданию» в личном кабинете.  
Желаем успехов в выполнении домашнего задания!

### Задание 1

Что нужно сделать:

1. Установите себе jenkins по инструкции из лекции или любым другим способом из официальной документации. Использовать Docker в этом задании нежелательно.  
2. Установите на машину с jenkins golang.  
3. Используя свой аккаунт на GitHub, сделайте себе форк репозитория. В этом же репозитории находится дополнительный материал для выполнения ДЗ.  
4. Создайте в jenkins Freestyle Project, подключите получившийся репозиторий к нему и произведите запуск тестов и сборку проекта go test . и docker build ..  
   
В качестве ответа пришлите скриншоты с настройками проекта и результатами выполнения сборки.

### Ответ на Задание 1

Скрины с настройками jenkins:

![Скрин 1](https://github.com/s-bessonniy/netology_hw_git_fors-20/blob/main/img/VirtualBox_Ubuntu_24_03_2024_12_56_07.png)

![Скрин 2](https://github.com/s-bessonniy/netology_hw_git_fors-20/blob/main/img/VirtualBox_Ubuntu_24_03_2024_12_58_35.png)

Лог выполнения:

![Скрин 3](https://github.com/s-bessonniy/netology_hw_git_fors-20/blob/main/img/VirtualBox_Ubuntu_24_03_2024_13_01_38.png)

![Скрин 4](https://github.com/s-bessonniy/netology_hw_git_fors-20/blob/main/img/VirtualBox_Ubuntu_24_03_2024_13_01_48.png)

### Задание 2

Что нужно сделать:

1. Создайте новый проект pipeline.  
2. Перепишите сборку из задания 1 на declarative в виде кода.
   
В качестве ответа пришлите скриншоты с настройками проекта и результатами выполнения сборки.  

### Ответ на Задание 2

Скрин с настройками pipeline

![Скрин1](https://github.com/s-bessonniy/netology_hw_git_fors-20/blob/main/img/VirtualBox_Ubuntu_24_03_2024_13_13_53.png)

Логи выполнения pipeline

![Скрин2](https://github.com/s-bessonniy/netology_hw_git_fors-20/blob/main/img/VirtualBox_Ubuntu_24_03_2024_13_14_22.png)

![Скрин3](https://github.com/s-bessonniy/netology_hw_git_fors-20/blob/main/img/VirtualBox_Ubuntu_24_03_2024_13_14_48.png)

### Задание 3

Что нужно сделать:

1. Установите на машину Nexus.  
2. Создайте raw-hosted репозиторий.  
3. Измените pipeline так, чтобы вместо Docker-образа собирался бинарный go-файл. Команду можно скопировать из Dockerfile.  
4. Загрузите файл в репозиторий с помощью jenkins.
   
В качестве ответа пришлите скриншоты с настройками проекта и результатами выполнения сборки.

### Ответ на Задание 3

Создал pipeline.
![Скрин1](https://github.com/s-bessonniy/netology_hw_git_fors-20/blob/main/img/VirtualBox_Ubuntu_25_03_2024_13_37_55.png)

Вывод консоли jenkins

![Скрин2](https://github.com/s-bessonniy/netology_hw_git_fors-20/blob/main/img/VirtualBox_Ubuntu_25_03_2024_13_44_25.png)

![Скрин3](https://github.com/s-bessonniy/netology_hw_git_fors-20/blob/main/img/VirtualBox_Ubuntu_25_03_2024_13_44_38.png)

![Скрин4](https://github.com/s-bessonniy/netology_hw_git_fors-20/blob/main/img/VirtualBox_Ubuntu_25_03_2024_13_44_48.png)

Файд в репозитории Nexus

![Скрин5](https://github.com/s-bessonniy/netology_hw_git_fors-20/blob/main/img/VirtualBox_Ubuntu_25_03_2024_13_47_18.png)

Помогите разобраться.

