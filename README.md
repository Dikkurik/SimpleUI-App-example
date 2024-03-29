# Приложение "Птицы"

Небольшое приложение "Птицы" сделанное с помощью платформы SimpleUI, Python и json-файла в качестве NoSQL базы данных.

Для запуска необходимо запустить ui-файл BirdsApp.ui через андроид приложение SimpleUI.

# Функции приложения
- Приложения может выводить список и изображение птиц, хранящихся в БД. Для отображения птиц нужно нажать на кнопку "Птицы" в главном меню.

- Приложения может вносить название, описание (цвет перьев, например) и изображение птиц из галереи или фотокамеры устройства. Для внесенния данных нужно нажать кнопку "Птицы" в главное меню и прилистать список вниз.

>Для успешного запуска программы нужно расположить БД с птицами в папку файлов приложения SimpleUI на устройстве (путь для андроид: */storage/emulated/0/Android/data/ru.travelfood.simple_ui/files/*) и изображения в папку **/images** в папке файлов приложения

# Структура БД

Приложение считывает данные из json файла с названием db.json и имеет внутри структуру: <br /> {'имя_массива'
            <br />{[{
            <br />'name':'имя', 
            <br />'desc':'описание', 
            <br />'image':'путь_до _файла', 
            <br />'status':'булево_состояние'} 
            <br />
            <br />... 
            <br />
            <br />{**следущий элемент**}
            <br />]}}

# Ввод данных

В приложении есть два поля для ввода данных: поле **Введите название птицы** и **Введите описание птицы**, после ввода этих данных информация из первого поля отправится в переменную *name*, а данные из второго в переменную *desc*. Если выбрать картинку из галереи или сфотографировать через соответствующюю кнопку в переменную *image* будет передано это изображение. 

> При вводе через приложение, в переменную **image** будет передано изображение в base64 формате.

Для ввода данных используется кнопка **Добавить птицу**. После ввода введеные данные тут же отобразятся в виде карточки. 

> При сохранении фотографий введеных с устройства они сохраняются в папку **Pictures** в папку файлов приложения.

# Процесс Птицы которых я видел


В приложении, в разделе Птицы, можно отметить одну птицу которую видел и в глоабльную переменную будет передана ее инфорация и время. Эту птицу можно будет увидеть через главный экран, раздел "Птицы которых я видел"