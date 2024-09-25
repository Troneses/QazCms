/my_cms/                    # Корневая директория проекта
│
├── /Core/                   # Системные файлы проекта и ядро движка (включая CodeIgniter 4)
│   ├── /app/                # Файлы приложения CodeIgniter
│   ├── /system/             # Системные файлы CodeIgniter
│   ├── /writable/           # Папка для кэша, логов и других временных файлов
│   ├── /admin/              # Админка
│   ├── /includes/           # Библиотеки и утилиты
│   ├── /plugins/            # Плагины (включая Summernote)
│   │   └── /example_plugin/ # Пример плагина
│   ├── /libraries/          # Внешние библиотеки
│   │   ├── /jquery/         # Библиотека jQuery
│   │   ├── /bootstrap/      # Библиотека Bootstrap
│   │   └── /other_libs/     # Другие библиотеки
│   └── /themes/             # Темы (как для админки, так и для публичных страниц)
│
├── /public/                 # Публичные файлы (CSS, JS, изображения)
│   ├── /css/
│   ├── /js/
│   └── /images/
│
└── /uploads/                # Загруженные файлы
index.php
env.example
README.md
