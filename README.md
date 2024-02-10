# Приложения "Птицы"

Небольшое приложение "Птицы" сделанное с помощью платформы SimpleUI, Python и json-файла в качестве NoSQL базы данных.

Для запуска необходимо запустить ui-файл BirdsApp.ui через андроид приложение SimpleUI.

# Функции приложения
- Приложения может выводить список и изображение птиц, хранящихся в БД. Для отображения птиц нужно нажать на кнопку "Птицы" в главном меню.

- Приложения может вносить название, описание (цвет перьев, например) и изображение птиц из галереи или фотокамеры устройства. 

Для успешного запуска программы нужно расположить БД с птицами в папку файлов приложения SimpleUI на устройстве (путь для андроид: */storage/emulated/0/Android/data/ru.travelfood.simple_ui/files/*) и изображения в папку **/images** в папке файлов приложения

# Структура БД

Приложение считывает данные из json файла с названием db.json и имеет внутри структуру: {'имя_массива'{[{'name':'имя', 'desc':'описание', 'image':'путь_до _файла', 'status':'булево_состояние'} ... {**следущий элемент**}]}}



