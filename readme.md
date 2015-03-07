# Vagrant box для работы в с окружением Битрикс

Машина для локальной работы с Битрикс. 

На машину устанавливается CentOS 6.5 86x64, затем окружение Битрикс. 

Когда окружение Битрикса установлено, отключается автозагрузка ~/menu.sh для root'а. 
Если нужно что-то сделать в меню окружения, нужно зайти под root'ом (логин: root, пароль:vagrant) и запустить ~/menu.sh вручную.

И после этого активируется XDebug.

Web сервер на виртуальной машине работает на 80 порту.

## Настройка phpStorm для работы

 * Создаем сервер;
 * Ставим галку Use path mappings и прописываем локальный путь к проекту, а Absolute path on server прописываем в "/home/bitrix/www";
 * Редактируем Run/Debug Configurations;
 * Создаем PHP Web Application, все настройки оставляем по-умолчанию;

PhpStorm готов к отладке PHP на виртуальной машине.
