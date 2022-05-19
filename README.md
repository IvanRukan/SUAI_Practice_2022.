# Учебная практика. ГУАП. Весна 2022. Алгоритм сортировки.


## Программа сортировки текстовых файлов.


Программа для сортировки **текстовых файлов**, использующая алгоритм сортировки слиянием. На вход получает текстовый файл, содержащий латинские символы и числа. Программа сортирует слова по длине в порядке убывания, числа так же учитываются и сортируются по убыванию. Ввод пути к файлу осуществляется с клавиатуры. Далее программа выполняет сортировку, измеряет время сортировки и записывает результаты в два файла: *результирующий и аналитический.* В *результирующем* файле записываются слова в соотвествии с их длинной (от большего к меньшему). Например, все слова длиной в 10 букв будут сохранены в одну строчку, слова длиной в 9 букв в другую и так далее. В *аналитический* файл записывается исходный текст, по которому осуществлялась сортировка, а так же особенности варианта, статистика (сколько слов различной длины было найдено, время сортировки) и числа в порядке убывания.


## Пример работы:


Подберём подходящий текст:  
![Пример иходного текста для работы программы.](https://user-images.githubusercontent.com/100718053/169359327-b475fd7b-d27c-45bd-86fd-c17dccb16401.png "Пример иходного текста для работы программы.")
Рисунок 1 - Пример иходного текста для работы программы.  
Отсортируем этот текст.  
![image](https://user-images.githubusercontent.com/100718053/169362485-1277e32a-dd93-4e60-9024-2d323ff3f035.png)
Рисунок 2 - Результат сортировки исходного файла.  
Вуаля. Осталось посмотреть, что там с аналитическим файлом.
![image](https://user-images.githubusercontent.com/100718053/169362755-4c46adf6-4543-456c-a3aa-a36381806eca.png)
Рисунок 3 - Аналитический файл со статистикой.  
Всё работает. Стастика и время сортировки были зафиксированы.


## Технологии:
В проекте использовались две встроенные в Python библиотеки: **string** и **time**.  
**string** использовалась для  упрощения работы со строками. В ней есть методы **.digits**, **.ascii_letters**, **.punctuation**. В методах находятся уже готовы строчки символов(название каждого метода свидетельсвует о символах, что там содержатся), что очень удобно для разделения чисел и слов и удаления пунктуации. Экономит время.  
**time** был необходим для измерения времени сортировки каждого из входных файлов. **.clock()** вызывался в момент начала сортировки и в её конце. А разница между этими параметрами и была искомым временем.
## Установка:
Для запуска исходного кода необходимо, чтобы на компьютере был установлен Python.  
Для установки достаточно скопировать исходный .py файл и запустить его через консоль/открыть в среде программирования :)  
Чтобы запустить файл через командную строку, необходимо переместить файл в текущую рабочую директорию (либо добраться до неё через команду cd или cd/d для перехода на другой диск), после чего прописать команду python **имя файла**.py.  Вуаля.  Программа готова к работе.


