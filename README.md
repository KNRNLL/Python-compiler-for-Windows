
Python packer for Windows - простой упаковщик скриптов Python в .EXE файлы.

Имеет графический интерфейс, создан на основе PyInstaller

Для работы программы потребуется установить модуль [Pyinstaller](https://pypi.org/project/PyInstaller/), PyWin32 и Pypiwin32. 
Если вы устанавливаете PyInstaller с помощью pip, а PyWin32 еще не установлен, pypiwin32 устанавливается автоматически.
PyInstaller также требует пакет pefile .
Возможно понадобится дополнительно установить сопутствующие библиотеки - интерпретатор сообщит вам об этом.

* Где сохраняются скомпилированные проекты?

Сборка производится в папку dist в рабочем каталоге IDLE - она будет создана, если ее нет.​
Открыть ее довольно просто - нажатием кнопки open​
​
* Как собрать проект?
Укажите путь к скрипту, который хотите собрать в exe файл.
Расширение файла должно быть .py
При необходимости отметьте нужные чекбоксы справа - в консоли отобразится статус настройки.
В окне программы появится кнопка "Запустить сборку!" - при ее нажатии запустится процесс сборки скрипта.

** Настройки работы программы

*Отключить запуск терминала.​

Эта настройка отключает отображение консоли при запуске вашего приложения после сборки.
​
*Сборка в один файл​

Эта настройка позволит собрать вашу программу в один exe файл​.

*Сборка в одну папку.​

Эта настройка позволит собрать вашу программу в каталог, внутри которого будут служебные файлы exe файл вашей программы​.
Такой вариант будет быстрее запускаться.

*Задать иконку файлу

Выберите ico иконку для вашего проекта и установите чекбокс на этом пункте - иконка будет добавлена к проекту.
​
*Очистить временные файлы​
Удаление временных файлов, которые создаются в процессе сборки проекта​

* Как добавить собственные меню из функционала Pyinstaller?

Просто добавляйте желаемые пункты в список list_check на 59 строке - я в программе разместил класс, который самостоятельно генерирует отображение, размещение на форме и команды обращения к пункту.
Не забудьте добавить команду на исполнение в функцию file_compilled - только не последним файлом, что бы не ломать логику построения.


[Официальный форум поддержки](https://safezone.cc/threads/python-exe-compiller-programma-dlja-kompiljacii-skriptov-python-v-exe-fajly.34032/#post-278301)

![Графический интерфейс](https://safezone.cc/attachments/1575478644727-png.48058/)

