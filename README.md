# Lab_1
Homework

    1.Скачайте библиотеку boost с помощью утилиты wget. Адрес для скачивания:
    https://sourceforge.net/projects/boost/files/boost/1.69.0/boost_1_69_0.tar.gz.
    2.Разархивируйте скаченный файл в директорию ~/boost_1_69_0
    3.Подсчитайте количество файлов в директории ~/boost_1_69_0 не включая вложенные директории.
    4.Подсчитайте количество файлов в директории ~/boost_1_69_0 включая вложенные директории.
    5.Подсчитайте количество заголовочных файлов, файлов с расширением .cpp, сколько остальных файлов (не заголовочных и не .cpp).
    6.Найдите полный пусть до файла any.hpp внутри библиотеки boost.
    7.Выведите в консоль все файлы, где упоминается последовательность boost::asio.
    8.Скомпилирутйе boost. Можно воспользоваться инструкцией или ссылкой.
    9.Перенесите все скомпилированные на предыдущем шаге статические библиотеки в директорию ~/boost-libs.
    10.Подсчитайте сколько занимает дискового пространства каждый файл в этой директории.
    11.Найдите топ 10 самых "тяжёлых".

Выполнение

image wget ... - скачивание файла и сохранение в текущей директории
2. image tar -xf - распаковка файла
tar -C - используется для указания папки
3. image find -type f - искать файлы
Команда find передаёт список всех файлов в текущем каталоге с каждым именем файла в одной строке команде wc, которая подсчитывает количество строк и печатает результат
4. image 5. image image image 6. image 7. image grep -r - Первый параметр представляет регулярное выражение для поиска, а второй представляет каталог, в котором необходимо искать. В данном случае имеется в виду текущий каталог
8. image image ./script.sh - запуск скрипта
--prefix=PREFIX - папка для установки программы
9. image image image mv - переместить файлы или директории
10. image du -a - вывод размера папок и файлов
11. image sort -n -r - сортировка строк по числовому значению в обратном порядке
head -n - вывод 10 строк

