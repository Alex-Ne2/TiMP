# Lab_1
Задание

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
1.  `wget ...` - скачивание файла и сохранение в текущей директории
![image](https://github.com/Alex-Ne2/TiMP/blob/main/lab_1_1.png)
2. распаковка файла
   
    ![image](https://github.com/Alex-Ne2/TiMP/blob/main/lab_1_2.png)

    `tar -xf` - распаковка файла    
    `tar -C` - используется для указания папки
3. считаем количество файлов в директории
   ![image](https://github.com/Alex-Ne2/TiMP/blob/main/lab_1_3.png)
   `find -type f` - искать файлы    
   Команда `find` передаёт список всех файлов в текущем каталоге с каждым именем файла в одной строке команде `wc`, которая подсчитывает количество строк и печатает результат
4. 
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![image](https://github.com/Alex-Ne2/TiMP/blob/main/lab_1_4.png)
 
5.  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![image](https://github.com/Alex-Ne2/TiMP/blob/main/lab_1_5.png) 

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![image](https://github.com/Alex-Ne2/TiMP/blob/main/lab_1_6.png) 

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![image](https://github.com/Alex-Ne2/TiMP/blob/main/lab_1_7.png) 

6.  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![image](https://github.com/Alex-Ne2/TiMP/blob/main/lab_1_8.png) 

7. <small> &nbsp;</small> ![image](https://github.com/Alex-Ne2/TiMP/blob/main/lab_1_9.png) 
`grep` параметр представляет регулярное выражение для поиска, а  `-r` представляет каталог, в котором необходимо искать.
В данном случае имеется в виду текущий каталог 

8. 
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![image](https://github.com/Alex-Ne2/TiMP/blob/main/lab_1_10.png)

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![image](https://github.com/Alex-Ne2/TiMP/blob/main/lab_1_11.png) 

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`./script.sh` - запуск скрипта

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`--prefix=PREFIX` - папка для установки программы

10. 
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![image](https://github.com/Alex-Ne2/TiMP/blob/main/lab_1_12.png)

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![image](https://github.com/Alex-Ne2/TiMP/blob/main/lab_1_13.png) 

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![image](https://github.com/Alex-Ne2/TiMP/blob/main/lab_1_14.png) 

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`mv` - переместить файлы или директории

12. 
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![image](https://github.com/Alex-Ne2/TiMP/blob/main/lab_1_15.png)

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`du -a` - вывод размера папок и файлов

14. 
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![image](https://github.com/Alex-Ne2/TiMP/blob/main/lab_1_16.png)

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`sort -n -r` - сортировка строк по числовому значению в обратном порядке

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`head` - вывод 10 строк

