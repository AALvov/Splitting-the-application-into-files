# Splitting-the-application-into-files
Базовый php-разработчик работа 13

В этом задании мы разделим код «Телеграфа» на отдельные файлы и реализуем автозагрузку классов.

В папке проекта создайте подпапку entities (сущности) для хранения файлов с классами сущностей.

В подпапке entities создайте файлы для классов сущностей User.php, Storage.php, FileStorage.php, Text.php и TelegraphText.php. Перенесите описания классов User, Storage, TelegraphText и так далее в соответствующие файлы.

В папке проекта создайте подпапку interfaces и поместите туда интерфейсы LoggerInterface и EventListenerInterface.

В файлах User.php и Storage.php реализуйте подключение интерфейсов LoggerInterface и EventListenerInterface, а также необходимых абстрактных классов. Используйте require_once.

В корневой папке проекта создайте файл autoload.php. Реализуйте в нём функцию автозагрузчика классов из папки entities. Для регистрации автозагрузчика используйте spl_autoload_register. 

В корневой папке проекта создайте файл index.php, подключите к нему autoload.php любым удобным способом (include_once, например).

Попробуйте создать объект класса FileStorage.php в index.php. Если всё сделано правильно, код должен работать без ошибок.

Сделайте коммит ваших изменений с помощью Git и отправьте коммит в репозиторий.
