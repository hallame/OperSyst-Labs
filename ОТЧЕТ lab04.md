# РОССИЙСКИЙ УНИВЕРСИТЕТ ДРУЖБЫ НАРОДОВ

**Факультет физико-математических и естественных наук**




**ОТЧЕТ
ПО ЛАБОРАТОРНОЙ РАБОТЕ № 4**

***Дисциплина: Операционные системы***




**Студент**: Алламе Ормиз

Группа: НФИбд-01-21


МОСКВА
2022 г.






 # *Постановка задачи*


Приобретение практических навыков взаимодействия пользователя с системой посредством командной строки.


# *Выполнение работы*


**1.Определите полное имя вашего домашнего каталога. Далее относительно этого каталога будут выполняться последующие упражнения.**


      Для этого мы будем использовать команду pwd.
      

**2. Выполните следующие действия:
2.1. Перейдите в каталог /tmp.**

 ![](https://github.com/hallame/OperSyst-Labs/blob/main/lab401.jpeg?raw=true)
 


**2.2. Выведите на экран содержимое каталога /tmp. Для этого используйте команду ls
с различными опциями. Поясните разницу в выводимой на экран информации.**



![](https://github.com/hallame/OperSyst-Labs/blob/main/lab402.jpeg?raw=true)


Есть подкаталог, который помещен в когти.



**2.3. Определите, есть ли в каталоге /var/spool подкаталог с именем cron?**


![](https://github.com/hallame/OperSyst-Labs/blob/main/lab402.jpeg?raw=true)

Неподкаталога с именем cron в этом каталоге.


**2.4. Перейдите в Ваш домашний каталог и выведите на экран его содержимое. Опре-
делите, кто является владельцем файлов и подкаталогов?**

hallame является владельцем файлов и подкаталогов.


**3. Выполните следующие действия:
3.1. В домашнем каталоге создайте новый каталог с именем newdir.**

![](https://github.com/hallame/OperSyst-Labs/blob/main/lab403.jpeg?raw=true)


**3.2. В каталоге ~/newdir создайте новый каталог с именем morefun.**


**3.3. В домашнем каталоге создайте одной командой три новых каталога с именами
letters, memos, misk. Затем удалите эти каталоги одной командой.**

![](https://github.com/hallame/OperSyst-Labs/blob/main/lab405.jpeg?raw=true)



     Чтобы создать и удалить эти три каталога одновременно, мы будем использовать команды mkdir и rmdir соответственно, а также их соответствующие имена.


**3.4. Попробуйте удалить ранее созданный каталог ~/newdir командой rm. Проверьте,
был ли каталог удалён.**

![](https://github.com/hallame/OperSyst-Labs/blob/main/lab405.jpeg?raw=true)


 *Команда rm не удалось удалить каталог newdir но и тут команда rm -r*


**3.5. Удалите каталог ~/newdir/morefun из домашнего каталога. Проверьте, был ли
каталог удалён.**

![](https://github.com/hallame/OperSyst-Labs/blob/main/lab406.jpeg?raw=true)


Команда может удалить подкаталог more fun, но каталог "newdir" уже удален командой rm-r, тогда мы получим сообщение : *такого каталога не существует.*


**4. С помощью команды man определите, какую опцию команды ls нужно использо-
вать для просмотра содержимое не только указанного каталога, но и подкаталогов,
входящих в него.**

**5. С помощью команды man определите набор опций команды ls, позволяющий отсорти-
ровать по времени последнего изменения выводимый список содержимого каталога
с развёрнутым описанием файлов.**


![](https://github.com/hallame/OperSyst-Labs/blob/main/lab409.jpeg?raw=true)


     Здесь речь идет о команде ls - l


**6. Используйте команду man для просмотра описания следующих команд: cd, pwd, mkdir, rmdir, rm. Поясните основные опции этих команд.**

   ***man cd***
   
![](https://github.com/hallame/OperSyst-Labs/blob/main/lab410.jpeg?raw=true)


  ***man pwd***
  
![](https://github.com/hallame/OperSyst-Labs/blob/main/lab411.jpeg?raw=true)


***man mkdir***

![](https://github.com/hallame/OperSyst-Labs/blob/main/lab412.jpeg?raw=true)

***man rmdir***

![](https://github.com/hallame/OperSyst-Labs/blob/main/lab417.jpeg?raw=true)



***man rm***

![](https://github.com/hallame/OperSyst-Labs/blob/main/lab413.jpeg?raw=true)



**7. Используя информацию, полученную при помощи команды history, выполните модификацию и исполнение нескольких команд из буфера команд.**

![](https://github.com/hallame/OperSyst-Labs/blob/main/lab414.jpeg?raw=true)

***На уровне строки 82, я изменил команду rm B mkdir***

![](https://github.com/hallame/OperSyst-Labs/blob/main/lab415.jpeg?raw=true)




***Повторная проверка истории***

![](https://github.com/hallame/OperSyst-Labs/blob/main/lab416.jpeg?raw=true)







# *Вывод:*

В данном разделе рассматриваются основные команды по работе с файловой системой и текстами, а также примеры их комплексного использования.

Ключевые термины:pwd, cd, ls, mkdir, rmdir, rm,...





# *Ответы на контрольные вопросы*

1.  Командная строка, также называемая процессором команд, интерпретатором команд и консолью, представляет собой программный инструмент, позволяющий пользователю вводить команды и получать результаты их выполнения на экране.

2.  Чтобы подняться к каталогу dir1, наберите: cd /dir1. Это пример абсолютного пути. Он дает Linux команду начать с верха дерева каталогов (/) и спуститься до каталога dir1. Путь является абсолютным, если он начинается с /. В противном случае это относительный путь.

3.  Для определения расширения файла используйте команду вида: .\trid 'Путь:\до\файла'. Например: .\trid Z:\testfiles\file1. Подстановочные знаки могут использоваться для сканирования групп файлов, целых папок и так далее. Кроме того, использование ключа -ae даст команду TrID добавить предполагаемые расширения к именам файлов. Это удобно, например, при работе с файлами, восстановленными программами для восстановления данных.

4.  Для отображения скрытых файлов и папок сделайте следующее:

Windows 10

   -  В поле поиска на панели задач введите запрос папка и выберите пункт Показыватьскрытые файлы и папки в результатах поиска.
- В разделе Дополнительные параметрыустановите флажок Показывать скрытые файлы, папки и дискии нажмите кнопку ОК.

Windows 8.1 

-  Проведите пальцем влево от правого края экрана и выберите команду Поиск (если вы используете мышь, наведите указатель на правый верхний угол экрана, переместите его вниз, а затем выберите команду Поиск).
-  Введите запрос папка в поле поиска, а затем выберите Параметры папок в результатах поиска.
-  Откройте вкладку Вид.
- В разделе Дополнительные параметрыустановите флажок Показывать скрытые файлы, папки и дискии нажмите кнопку ОК.

Windows 7 

- Нажмите кнопку "Пуск" и выберите пункты Панель управления > Оформление и персонализация.
-  Выберите Параметры папок, а затем откройте вкладку Вид.
-  В разделе Дополнительные параметры выберите Показывать скрытые файлы, папки и диски, а затем нажмите кнопку ОК.


5.  Для удаления файлов используется команда rm.

               Например:
      rm ghost.png. Командой radar можно удалить пустой каталог. Если же каталог не пуст, следует использовать команду rm с ключом -r:
Можно удалить файл и каталог одной и той же командой. Например, команда rm позволяет удалять файлы. Команда rmdir работает аналогично для каталогов или папок.


6.  Работу в командной строке можно сделать немного эффективнее и быстрее, если знать несколько простых хитростей. Рассмотрим, как быстро запускать предыдущие команды, как выполнять поиск по истории команд. Повторный запуск команды без указания аргументов. Используем «!» !команда — используется для выполнения команды с аргументами, которые использовались при последнем запуске. ... Предположим, мы выполняем какие-нибудь команды и дополняем их аргументами. Например, мы решили отредактировать файл myfile.txt в текстовом редакторе nano. Для этого мы выполняем: nano /home/pingvinus/path/to/file/myfile.txt.
Посмотреть историю действий на компьютере можно соответствующим инструментом под названием «Журнал событий». Чтобы его запустить достаточно выполнить следующий ряд действий: Открыть меню «Пуск» и кликнуть на «Панель управления» (в Windows 8 и Windows 10 это делается немного по-другому).

7.  В истории команд используйте стрелки вверх и вниз, полосу прокрутки или любой другой метод прокрутки для поиска и выделения ранее введенных команд, системных переменных и текста.
По умолчанию при нажатии клавиши Cmd-C выделенный текст копируется в буфер обмена. Когда вы нажимаете Cmd-V, текст в буфере обмена вставляется в командную строку.
Чтобы скопировать весь текст истории заказов в буфер обмена, щелкните правой кнопкой мыши и выберите команду копировать историю из контекстного меню или введите команду COPIERHIST. Чтобы автоматически сохранять команды в файле журнала с помощью следующей команды, введите команду FICHJOURNAC.


8.  
В командной строке Linux можно объединять сразу несколько команд в одну строку (в один запуск). Например, вам нужно выполнить сначала одну команду, за ней вторую и так далее. Но вы хотите сразу вбить в командной строке одну инструкцию, которая все сделает. Для этого можно воспользоваться служебными символами. Выполнение команд последовательно. Например, мы хотим выполнить сначала одну команду. Затем, когда она отработает (вернет управление в командную строку), нам нужно запустить вторую команду. Для этого служит символ точка с запятой ;. Таким образом, если вы выполните в терминале: mycommand1...
9.  Экранирование символов — замена в тексте управляющих символов на соответствующие текстовые подстановки. Один из видов управляющих последовательностей. Определение :  Отсутствие экранирования как причина уязвимости. Примеры :  Экранирование одиночного символа, Экранирование группы символов, Экранирование текста с завершающим символом См..
 
Название символа Восклицательный знак Обратный слэш (бэкслэш) Двойная кавычка Знак процента Амперсанд Одинарная кавычка (апостроф) Звёздочка Плюс Минус (тире) Точка Слэш Нижнее подчеркивание Запятая Двоеточие Точка с запятой Равно Меньше Больше Вопросительный зна Открывающая круглая скобка Закрывающая круглая скобка.


10.  Команда ls происходит от слова list — список. Подробный список файлов. Выведем содержимое текущей директории, в которой мы в данной момент находимся. Используем опцию -l, чтобы выводить подробную информацию о файлах. ls -l. Если необходимо вывести содержимое другой директории, то нужно указать путь до директории, например: ls -l /var/log Показать скрытые файлы. По умолчанию команда ls не показывает скрытые файлы.

11.  Относительный путь ссылается на местоположение относительно текущего каталога. Относительные пути используют два специальных символа: точку (.) и двойную точку ( :), которые используются для перехода в текущий и родительский каталог, соответственно. Двойные точки используются для перехода на один уровень вверх.

Абсолютный путь к файлу (иногда говорят полный путь к файлу) или абсолютный адрес работает везде, где прописана ссылка - независимо от имени сайта и его расположения. Например, ссылка https://www.webpupil.ru является абсолютной.
Для перехода между страницами внутри сайта используют относительные ссылки или относительные адреса. Относительный путь к файлу указывают относительно текущего документа или относительно корневого каталога.

                   Например: <a href="index.php">
Относительная ссылка на главную страницу - файл index.php
</a>


12.  Для получения справочной информации, наберите в командной строке команду help. На экран выведется список основных команд. Для того чтобы получить справочную информацию об определенной команде нужно ввести cmd /?. Например, ping /? выдаст все возможные параметры команды отправки пакетов на заданный узел.

13.  На клавиатурах широко используются клавиши «Ctrl (Conrtol)», «Alt (Alternate)» и «Shift», как их еще часто называют клавиши-модификаторы, которые применяются совместно с другими клавишами для выполнения необходимых действий.



