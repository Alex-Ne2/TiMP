# Lab_1
Homework

    1.Скачайте библиотеку boost с помощью утилиты wget. Адрес для скачивания:
      https://sourceforge.net/projects/boost/files/boost/1.69.0/boost_1_69_0.tar.gz.
    2.Разархивируйте скаченный файл в директорию ~/boost_1_69_0
    3.Подсчитайте количество файлов в директории ~/boost_1_69_0 не включая вложенные директории.
    4.Подсчитайте количество файлов в директории ~/boost_1_69_0 включая вложенные директории.
    5.Подсчитайте количество заголовочных файлов, файлов с расширением .cpp, сколько остальных файлов
      (не заголовочных и не .cpp).
    6.Найдите полный пусть до файла any.hpp внутри библиотеки boost.
    7.Выведите в консоль все файлы, где упоминается последовательность boost::asio.
    8.Скомпилирутйе boost. Можно воспользоваться инструкцией или ссылкой.
    9.Перенесите все скомпилированные на предыдущем шаге статические библиотеки в директорию ~/boost-libs.
    10.Подсчитайте сколько занимает дискового пространства каждый файл в этой директории.
    11.Найдите топ 10 самых "тяжёлых".

Выполнение
1.  wget ... - скачивание файла и сохранение в текущей директории
![image](https://github.com/Alex-Ne2/TiMP/blob/main/lab_1_1.png)
2. распаковка файла
   
    ![image](https://github.com/Alex-Ne2/TiMP/blob/main/lab_1_2.png)

    tar -xf - распаковка ф&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;айла    
    tar -C - используется для указания папки
3. считаем количество файлов в директории
   ![image](https://github.com/Alex-Ne2/TiMP/blob/main/lab_1_3.png)
   image find -type f - искать файлы    
   Команда find передаёт список всех файлов в текущем каталоге с каждым именем файла в одной строке команде wc, которая подсчитывает количество строк и печатает результат
4. 
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![image](https://github.com/Alex-Ne2/TiMP/blob/main/lab_1_4.png)
 
5.  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![image](https://github.com/Alex-Ne2/TiMP/blob/main/lab_1_5.png) 

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![image](https://github.com/Alex-Ne2/TiMP/blob/main/lab_1_6.png) 

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![image](https://github.com/Alex-Ne2/TiMP/blob/main/lab_1_7.png) 

6. 
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![image](https://github.com/Alex-Ne2/TiMP/blob/main/lab_1_8.png) 

7. 
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; ![image](https://github.com/Alex-Ne2/TiMP/blob/main/lab_1_9.png) 
grep -r -Первый параметр представляет регулярное выражение для поиска, а второй представляет каталог, в котором необходимо искать.
В данном случае имеется в виду текущий каталог
8. ![image](https://github.com/Alex-Ne2/TiMP/blob/main/lab_1_10.png) ![image](https://github.com/Alex-Ne2/TiMP/blob/main/lab_1_11.png)
./script.sh - запуск скрипта
--prefix=PREFIX - папка для установки программы
9. ![image](https://github.com/Alex-Ne2/TiMP/blob/main/lab_1_12.png) ![image](https://github.com/Alex-Ne2/TiMP/blob/main/lab_1_13.png) ![image](https://github.com/Alex-Ne2/TiMP/blob/main/lab_1_14.png) mv - переместить файлы или директории
10. ![image](https://github.com/Alex-Ne2/TiMP/blob/main/lab_1_15.png) du -a - вывод размера папок и файлов
11. ![image](https://github.com/Alex-Ne2/TiMP/blob/main/lab_1_16.png) sort -n -r - сортировка строк по числовому значению в обратном порядке
head -n - вывод 10 строк

