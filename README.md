
# Django-проект Блогикум
## Версия 3

![image](https://github.com/VilmenAbramian/blogicum-3/assets/58857991/1082ca6b-5305-4ef0-96f8-16186e4a5517)


В данную версию проекта были добавлены:
* Кастомные страницы ошибок (403 CSRF, 404 и 500)
* Добавлена возможность создания пользовательских аккаунтов (для этого добавлены страницы регистрации, смены и восстановления пароля, а также персональная страница пользователя. На странице пользователя можно увидеть все посты автора, а владелец страницы также может изменять личную информацию)
* Настроена пагинация 
* Добавлена возможность добавления изображения к постам
* Теперь пользователи могут самостоятельно добавлять и удалять посты от своего имени. Для этого создана страница добавления поста, на которой, помимо текста и фотографии можно добавить к посту тег и местоположение (новые теги и метки локации может создать только пользователь с admin-правами)
* Можно создавать отложенные посты
* Добавлена возможность редактирования уже созданных и опубликованных постов
* Добавлено комментирование записей. Пользователи могут создавать, редактировать и удалять свои комментарии. Реализована пагинация и сортировка комментариев по дате добавления.

### Установка проекта:
* Скачать репозиторий: git clone proj-name в рабочую папку
* Выполнить команды в директории проекта:
```
python -m venv venvname
pip install -r requirements.txt
python manage.py migrate
python manage.py runserver
```

### Особенности проекта:
* Проект состоит из нескольких приложений, а именно: blog (содержит основную функциональность проекта), pages (описывает работу статичных страниц)
* В данном проекта все view-функции заменены на view-классы. Там, где это требуется, переопределены соответствующие методы view-классов.
* В качестве почтового сервиса, необходимого для возможности изменения пароля, используется специальная папка в директории проекта.
* В проекте присутствует большое количество автотестов.

![GitHub top language](https://img.shields.io/github/languages/top/VilmenAbramian/blogicum-3)

Финальный проект 8го спринта курса Python разработчик плюс.
Изначальное имя: django_sprint4
