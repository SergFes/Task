Необходимо создать простое приложение по работе с информацией о пользователях.
В процессе задействовать redux, react-router, компоненты из библиотеки antd


Исходники для старта можно забрать тут
Либо сделать fork + pull request по завершении
Либо прислать результат архивом на  xmeranuxapbx@gmail.com с темой “Тестовое задание Yakutia”


1 Данные загружать запросом к /api/users, реализовать показ лоадера до момента загрузки данных
2 Создать страницы со следующим функционалом:

роут /users

Вывести в таблицу поля
id, name, age, gender, registered, а также колонку с кнопкой "Удалить пользователя"
Для age добавить сортировку по убыванию \ по возрастанию (По умолчанию сортировать по убыванию)
Поле registered форматировать при выводе, формат "DD.MM.YYYY"

Добавить фильтр по полю gender
Добавить фильтр по полю registered (DateRangePicker, отфильтровывать записи, не попавшие в выбранный диапазон дат)

роут /users/add

форма добавления пользователя
Поля для ввода
name - добавить валидацию - длина значения больше 5 символов
age - добавить валидацию - значение больше 18
gender задавать с помощью select (male \ female)

id генерировать с помощью middleware (timestamp или, например uuid)
в качестве значения для поля registered при создании нового пользователя использовать new Date()
в качестве значения для поля friends использовать пустой массив

роут /users/:id

просмотр информации о конкретном пользователе

вывести значения полей name, about
так же вывести список друзей:
name, age

если пользователя с указанным id не существует, делать редирект на /users

p.s.

Важно, чтобы код не только работал, но и был чистым. Грамотное название переменных и функций, лаконичные функции, малое число уровней вложенности, вменяемая длина строки. В общем код должен читаться легко. Внешний вид в браузере вторичен, стилизовать можно по желанию.

Вопросы можно задавать
тут - xmeranuxapbx@gmail.com 
или
тут- https://t.me/knownAim