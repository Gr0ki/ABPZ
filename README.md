Цей проект розроблений в рамках виконання лабораторної роботи з предмету "Аналіз безпеки програмного 
забезпечення".

__________________________________________________________________________________________________________________________________

Опис файлів та каталогів проекту:

Скрипт “deployment_django_project.sh” необхідний для автоматичного розгортання проекту та запуску серверу, 
детальніше у файлі "SETUP.md".

Файл manage.py необхідний для управління проекту (запуск серверу, створення суперюзера, зміна паролю 
користувача і багато іншого, довідку можна отримати ввівши “python manage.py”).

“db.sqlite3” - це база даних яка зберігає в собі усю інформацію щодо користувачів, необхідну інформацію для 
роботи серверу та користувацьуі моделі.

“requirements.txt” містить в собі інформацію щодо усіх залежностей, для швидкого встановлення їх усіх можна 
використати команду “pip install -r requirements.txt”.

Каталог “static” містить шаблони для frontend частини сайту, в данному проекті створено лише 1 такий, 
“base.html”.

В каталозі “config” зберігаються основні конфігураційні файли проекту (маршрути сайту з основної сторінки, 
налаштування проекту та інше).
Встановлення парольних валідаторів виконується у файлі “config/settings.py”, у змінній 
“AUTH_PASSWORD_VALIDATORS”. Усі  підключені валідатори за замовчуванням були закоментовані і таким чином 
відключенні, а новий, користувацький, розроблений спеціально до індивідуально завдання, був підключений.

Католог “src” містить користувацькі додатки (“home” та “accounts” та папку з додатковою логікою, 
інструментами: “services”, в останній зберігається користувацький парольний валідатор). В кожному додатку 
містяться свої маршрути, які імортуються до тих, які в основних налаштуваннях проекту, своя адмінка, файл 
налаштування додатку “apps.py”, файл з логікою “views.py”, тести моделі форми та шаблони для frontend.

__________________________________________________________________________________________________________________________________
