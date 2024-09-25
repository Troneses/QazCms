/my_cms/                    # Корневая директория проекта
│
├── /system/                # Системные файлы и конфигурация
│   ├── /admin/             # Административная панель
│   │   ├── dashboard.php   # Главная страница админки
│   │   ├── settings.php    # Настройки админки
│   │   ├── users.php       # Управление пользователями
│   │   └── plugins.php     # Управление плагинами
│   ├── /includes/          # Основные библиотеки и функции
│   │   ├── database.php    # Функции работы с базой данных
│   │   ├── auth.php        # Авторизация пользователей
│   │   └── seo.php         # SEO функции
│   ├── /plugins/           # Плагины
│   │   └── example_plugin/ # Пример плагина
│   │       ├── plugin.php  # Основной файл плагина
│   │       └── config.php  # Конфигурация плагина
│   ├── /themes/            # Темы оформления
│   │   └── default/        # Тема по умолчанию
│   │       ├── header.php  # Шапка сайта
│   │       ├── footer.php  # Подвал сайта
│   │       └── style.css   # Стили темы
│   ├── /uploads/           # Загруженные пользователями файлы
│   │   └── index.html      # Защита от прямого доступа
│   ├── /logs/              # Логи приложения
│   │   └── error.log       # Логи ошибок
│   ├── /config/            # Конфигурационные файлы
│   │   ├── config.php      # Основной конфигурационный файл
│   │   └── database.php    # Настройки базы данных
│   ├── /codeigniter/       # Папка с CodeIgniter
│   │   ├── /app/           # Основные файлы приложения CodeIgniter
│   │   ├── /system/        # Системные файлы CodeIgniter
│   │   ├── /writable/      # Папка для записи (кэш, логи и т.д.)
│   │   └── .env            # Файл конфигурации окружения
│   ├── /summernote/        # Папка для Summernote
│   │   ├── /css/           # CSS файлы Summernote
│   │   │   └── summernote.min.css
│   │   ├── /js/            # JS файлы Summernote
│   │   │   ├── summernote.min.js
│   │   ├── /lang/          # Языковые файлы Summernote
│   │   ├── /plugin/        # Плагины Summernote
│   │   └── /fonts/         # Шрифты Summernote
│   ├── /libraries/         # Папка для сторонних библиотек
│   │   ├── /jquery/        # Библиотека jQuery
│   │   │   └── jquery-3.7.1.min.js
│   │   ├── /bootstrap/     # Библиотека Bootstrap
│   │   │   ├── /css/       # CSS файлы Bootstrap
│   │   │   │   └── bootstrap.min.css
│   │   │   ├── /js/        # JS файлы Bootstrap
│   │   │   │   └── bootstrap.bundle.min.js
│   │   └── /other_libs/    # Папка для других библиотек (по необходимости)
│   ├── init.php            # Инициализация приложения
│
├── /public/                # Публичные ресурсы
│   ├── /css/               # Пользовательские стили
│   │   └── style.css       # Основной CSS файл
│   ├── /js/                # Пользовательские скрипты
│   │   └── scripts.js      # Основной JS файл
│   ├── /images/            # Изображения сайта
│   ├── index.php           # Точка входа для публичных ресурсов
│   ├── .htaccess           # Настройки сервера
│   └── codeigniter.php     # Точка входа CodeIgniter
│
└── README.md               # Документация проекта


Описание ключевых элементов:
/system/admin/: Панель администратора. Здесь находятся страницы админки, например dashboard.php, settings.php, users.php, и plugins.php для управления плагинами.

/system/includes/: В этой папке размещаются основные файлы и функции проекта:

database.php — функции для работы с базой данных.
auth.php — файл авторизации пользователей.
seo.php — функции для SEO-оптимизации.
/system/plugins/: Для добавления плагинов, которые можно будет подключать и отключать, как в WordPress.

Папка example_plugin/ содержит пример плагина, с основным файлом plugin.php и конфигурацией config.php.
/system/themes/: Папка для тем оформления сайта. В примере указана тема default, которая включает в себя header.php, footer.php, и style.css.

/system/uploads/: Папка для загрузок пользователей, защищенная файлом index.html.

/system/logs/: Папка для логов приложения, содержащая, например, файл error.log.

/system/config/: Здесь находятся конфигурационные файлы, такие как:

config.php — основной конфигурационный файл.
database.php — настройки для подключения к базе данных.
/system/codeigniter/: Интеграция CodeIgniter:

/app/ — приложение CodeIgniter.
/system/ — системные файлы CodeIgniter.
.env — конфигурационный файл окружения.
/system/summernote/: Полная интеграция Summernote:

summernote.min.css и summernote.min.js — основные файлы.
/lang/, /plugin/, /fonts/ — дополнительные директории для работы Summernote.
/system/libraries/: Сюда помещаем сторонние библиотеки:

/jquery/ содержит jquery-3.7.1.min.js.
/bootstrap/ содержит файлы Bootstrap (bootstrap.min.css и bootstrap.bundle.min.js).
/public/: Публичные ресурсы:

/css/ — пользовательские стили.
/js/ — пользовательские скрипты.
/images/ — изображения сайта.
index.php — основной файл для публичного доступа.
.htaccess — конфигурация веб-сервера для защиты файлов.
Файлы, которые нужно создать:
/system/admin/dashboard.php — главная страница админки.
/system/admin/settings.php — настройки панели администратора.
/system/admin/users.php — управление пользователями.
/system/admin/plugins.php — управление плагинами.
/system/includes/database.php — функции работы с базой данных.
/system/includes/auth.php — авторизация.
/system/includes/seo.php — SEO функции.
/system/plugins/example_plugin/plugin.php — пример плагина.
/system/plugins/example_plugin/config.php — конфигурация плагина.
/system/themes/default/header.php — шапка сайта.
/system/themes/default/footer.php — подвал сайта.
/system/themes/default/style.css — стили темы.
/system/uploads/index.html — защита папки загрузок.
/system/logs/error.log — логи приложения.
/system/config/config.php — основной конфиг.
/system/config/database.php — настройки базы данных.
/system/init.php — инициализация движка.
/public/css/style.css — стили для публичной части.
/public/js/scripts.js — скрипты для публичной части.
/public/index.php — точка входа.