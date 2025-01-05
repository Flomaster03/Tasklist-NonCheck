1_6

Описание
Приложения, отслеживающие наши задачи, очень практичны и удобны. В этом проекте мы создадим один такой инструмент.

Начнем с мелочей. Ваша программа должна получать задачи из входных данных, по одной на строку, а затем выводить их на печать. Задачи должны содержать индексный номер.

Цели
Попросите ввести данные, напечатав Input the tasks (enter a blank line to end):. Прочитайте каждое задание, по одному на строку. Избавьтесь от любых начальных или конечных пробелов и табуляций;
Ввод задач должен заканчиваться, когда пользователь вводит пустую строку. То есть строку без текста. Если пользователь вводит строку, содержащую только пробелы и табуляции, считайте ее пустой строкой.
Распечатайте задания в следующем формате:
1  Task1
2  Task2
3  Task3
4  Task4
5  Task5
6  Task6
7  Task7
8  Task8
9  Task9
10 Task10
11 Task11

Список задач начинается с 1. Первые девять задач содержат 2 пробела между номером и задачей. Начиная с задачи 10, оставьте только один пробел (см. раздел Примеры);
Если пользователи не вводят никаких задач (пустая строка), вывести No tasks have been input.
Примеры
Символ "больше" с последующим пробелом ( > ) представляет собой пользовательский ввод. Обратите внимание, что он не является частью ввода.

Пример 1: обычное выполнение

Input the tasks (enter a blank line to end):
> Dentist on 15/1
> Present for friend birthday
> Supermarket. Milk, eggs, butter.
>
1  Dentist on 15/1
2  Present for friend birtday
3  Supermarket. Milk, eggs, butter.

Пример 2: обычное выполнение с 10 и более задачами

Input the tasks (enter a blank line to end):
> Dentist on 15/1
> Present for friend birthday
> Supermarket. Milk, eggs, butter.
> Cinema: get tickets
> Buy book
> Check new software
> Finish hyperskill project
> Change colors at site
> Pay phone bill
> Pay water bill
> Fix the printer.
>
1  Dentist on 15/1
2  Present for friend birthday
3  Supermarket. Milk, eggs, butter.
4  Cinema: get tickets
5  Buy book
6  Check new software
7  Finish hyperskill project
8  Change colors at site
9  Pay phone bill
10 Pay water bill
11 Fix the printer.

Пример 3: лишние детали удалены

Input the tasks (enter a blank line to end):
>         Dentist on 15/1
>    Buy book
>     Change colors at site
>
1  Dentist on 15/1
2  Buy book
3  Change colors at site

Пример 4: нет входных данных

Input the tasks (enter a blank line to end):
>
No tasks have been input

2_6

Описание
На этом этапе мы реализуем новое меню, которое предложит пользователям либо ввести задачу, либо распечатать все задачи. Поскольку каждая задача добавляется индивидуально, можно ввести многострочную задачу.

Ввод каждой задачи должен заканчиваться, когда пользователь вводит пустую строку (или только пробелы и табуляции).

Цели
Измените приветственную строку на Input an action (add, print, end):. Если пользователи вводят:

Все, что не равно add, print, или end(без учета регистра), вывести The input action is invalidи снова запросить ввод;
End— распечатать Tasklist exiting!и завершить;
Add— попросите пользователей добавить задачу со Input a new task (enter a blank line to end):строкой. Ввод завершается пустой строкой. При добавлении задачи удалите все начальные или конечные пробелы или табуляции в задачах;
Print— распечатать задачи, как описано ниже. Если задач нет, распечатать No tasks have been input.
Если в качестве задачи введена пустая строка (или несколько пробелов и табуляции), распечатать The task is blank. Не сохранять эту задачу. Задачи следует распечатать в следующем формате:

1  Task1-line1
   Task1-line2
   Task1-line3

2  Task2-line1

3  Task3-line1

4  Task4-line1
   Task4-line2

5  Task5-line1

6  Task6-line1

7  Task7-line1
   Task7-line2
   Task7-line3

8  Task8-line1

9  Task9-line1

10 Task10-line1

11 Task11-line1

Первая строка каждой задачи начинается с порядкового номера (начиная с 1).

Каждая строка задачи начинается с 4-го столбца.

Разделите задачи пустой строкой.

Примеры
Символ "больше" с последующим пробелом ( > ) представляет собой пользовательский ввод. Обратите внимание, что он не является частью ввода.

Пример 1: обычное выполнение

Input an action (add, print, end):
> add
Input a new task (enter a blank line to end):
> Supermarket
> -----------
> butter
> milk
> meat
>
Input an action (add, print, end):
> add
Input a new task (enter a blank line to end):
> See my dentist on 14/1/22
>
Input an action (add, print, end):
> add
Input a new task (enter a blank line to end):
> Check my report
> a) Grammar errors
> b) Verify numbers
> c) Check citations
>
Input an action (add, print, end):
> print
1  Supermarket
   -----------
   butter
   milk
   meat

2  See my dentist on 14/1/22

3  Check my report
   a) Grammar errors
   b) Verify numbers
   c) Check citations

Input an action (add, print, end):
> end
Tasklist exiting!

Пример 2: обычное выполнение с 10 и более задачами

Input an action (add, print, end):
> add
Input a new task (enter a blank line to end):
> See my dentist on 14/1/22
>
Input an action (add, print, end):
> add
Input a new task (enter a blank line to end):
> Supermarket
> Chocolates, flour, oranges
>
Input an action (add, print, end):
> add
Input a new task (enter a blank line to end):
> Buy book
>
Input an action (add, print, end):
> add
Input a new task (enter a blank line to end):
> Change colors at site
> Use Christmas theme
>
Input an action (add, print, end):
> add
Input a new task (enter a blank line to end):
> Pay phone bill
>
Input an action (add, print, end):
> add
Input a new task (enter a blank line to end):
> Pay water bill
>
Input an action (add, print, end):
add
Input a new task (enter a blank line to end):
> Fix my printer
>
Input an action (add, print, end):
> add
Input a new task (enter a blank line to end):
> Dentist on 15/1
>
Input an action (add, print, end):
> add
Input a new task (enter a blank line to end):
> Cinema: get tickets
> Check movie reviews
>
Input an action (add, print, end):
> add
Input a new task (enter a blank line to end):
> Present for friend birthday
>
Input an action (add, print, end):
> add
Input a new task (enter a blank line to end):
> Check new software
>
Input an action (add, print, end):
> print
1  See my dentist on 14/1/22

2  Supermarket
   Chocolates, flour, oranges

3  Buy book

4  Change colors at site
   Use Christmas theme

5  Pay phone bill

6  Pay water bill

7  Fix my printer

8  Dentist on 15/1

9  Cinema: get tickets
   Check movie reviews

10 Present for friend birthday

11 Check new software

Input an action (add, print, end):
> end
Tasklist exiting!

Пример 3: нет задач

Input an action (add, print, end):
> print
No tasks have been input
Input an action (add, print, end):
> end
Tasklist exiting!

Пример 4: пустая задача

Input an action (add, print, end):
> add
Input a new task (enter a blank line to end):
>
The task is blank
Input an action (add, print, end):
> print
No tasks have been input
Input an action (add, print, end):
> end
Tasklist exiting!

Пример 5: ненужные части удалены

Input an action (add, print, end):
> add
Input a new task (enter a blank line to end):
> Supermarket
> 		butter
> 	  milk
>    flour
>     chocolates
>
Input an action (add, print, end):
> add
Input a new task (enter a blank line to end):
>    Fix my printer
>
Input an action (add, print, end):
> print
1  Supermarket
   butter
   milk
   flour
   chocolates

2  Fix my printer

Input an action (add, print, end):
> end
Tasklist exiting!

Пример 6: Недопустимые действия

Input an action (add, print, end):
> task
The input action is invalid
Input an action (add, print, end):
> input
The input action is invalid
Input an action (add, print, end):
> end
Tasklist exiting!

3_6

Описание
На этом этапе мы добавим еще одну полезную функцию — возможность указывать крайний срок для конкретной задачи. Мы также поработаем над функцией приоритетного тега.

Конечно, задача может быть без крайнего срока. Однако, чтобы не усложнять, для каждой задачи на этом этапе требуется крайний срок.

Когда пользователи добавляют задачу, также просите их ввести дату, время и тег приоритета. Последний — это всего лишь одна буква: C, H, N, L(без учета регистра) на задачу, которая обозначает Критический, Высокий, Нормальный и Низкий соответственно.

Даты и время можно обрабатывать разными способами. Однако в этом проекте мы рекомендуем использовать datetimeбиблиотеку Kotlinx. Kotlinx состоит из ценных библиотек, которые не являются частью стандартной библиотеки. Чтобы получить доступ к datetimeбиблиотеке Kotlinx, ее следует добавить в зависимости вашего проекта, но это уже сделано за вас. Чтобы использовать ее, вам следует просто импортировать ее в свою программу с помощью:

import kotlinx.datetime.*

Ниже приведены некоторые примеры использования datetimeбиблиотеки:

// Create a LocalDate instance for 2017-4-29
val date = LocalDate(2017, 4, 29)

//Create a LocalDateTime instance for 2021-12-21 16:57
val dateTime = LocalDateTime(2021, 12, 31, 16, 57)
val year = dateTime.year         // Get year as an integer
val month = dateTime.monthNumber // Get month as an integer
val day = dateTime.dayOfMonth    // Get day as an integer
val hour = dateTime.hour         // Get hour as an integer
val minutes = dateTime.minute    // Get minutes as an integer

// Create a LocalDateTime instance for the current date and time for UTC+0 timezone
val dateTimeCurrent = Clock.System.now().toLocalDateTime(TimeZone.of("UTC+0"))
// Create a LocalDate instance for the current date and time for UTC+0 timezone
val dateCurrent = dateTimeCurrent.date

// Get the date and time as string
val dateTimeString = dateTime.toString()
// Print the string above
println(dateTimeString)  // Output 2021-12-31T16:57

// Same result as the above
println(dateTime)        // Output 2021-12-31T16:57

Как видно, LocalDateTimeвыходная строка разделяет дату и время символом T.

Оба LocalDateи LocalDateTimeвыдают IllegalArgumentExceptionисключение, если предоставленные данные о дате или времени недействительны. Их можно использовать для проверки допустимости предоставленной даты (на основе високосных лет, количества дней в месяце и т. д.).


Вы можете обратиться к обзору GitHub для получения дополнительной информации о Kotlin/kotlinx-datetime. Обратите внимание, что библиотека совместима со стандартной библиотекой Kotlin, начиная с версии 1.5.0. Поэтому лучше обновить Kotlin в вашей среде IntelliJ IDE до последней версии.


Наконец, предостережение. На этапе 6 данные списка задач будут сохранены в файле в формате JSON с Moshiбиблиотекой. Хотя datetimeобъекты библиотеки являются сериализуемыми, для их использования с Moshiнеобходимо зарегистрировать явный адаптер. Лучше использовать datetimeбиблиотеку для проверки даты, но сохранять данные даты и времени (в списках, классах и т. д.) как строки или целые числа .

Цели
Меню программы осталось прежним.

Когда пользователи вводят данные add, выполните следующие действия:

Спросите у пользователей приоритет задачи с помощьюInput the task priority (C, H, N, L):

Если пользователи не указали ни один из приоритетов C, H, N, L, спросите их еще раз (без учета регистра);

Пригласить на свиданиеInput the date (yyyy-mm-dd):

Если пользователи не ввели допустимую дату, распечатайте The input date is invalidи спросите еще раз;

Спросите время с помощьюInput the time (hh:mm):

Если пользователи не указали правильное время, распечатайте The input time is invalidи спросите еще раз;

Попросите пользователей ввести задачу, Input a new task (enter a blank line to end):как на предыдущем этапе;

Если указана одна пустая строка, распечатайте The task is blankи не сохраняйте задачу.

Обратите внимание, что дата должна быть реальной в следующем формате:

<year (4 digits)>-<number of month>-<number of day in the month>

Время должно быть в следующем формате:

<hour (0 - 23)>:<minutes (0 - 59)>

Когда пользователь вводит print, выведите задачи, как на предыдущем этапе, но с одним отличием — добавьте дату, время и приоритет в первую строку для каждой задачи:

1  Date1 Time1 Priority1
   Task1-line1
   Task1-line2

2  Date2 Time2 Priority2
   Task2-line1

3  Date3 Time3 Priority3
   Task3-line1

4  Date4 Time4 Priority4
   Task4-line1
   Task4-line2

Разделите дату, время и приоритет одним пробелом.

Если число месяцев, число дней в месяце, час или минут состоит только из одной цифры, им должен предшествовать ведущий ноль. Таким образом, каждое из них всегда будет печататься как двузначное число.

Выведите год в виде четырехзначного числа.

Примеры
Символ "больше" с последующим пробелом ( > ) представляет собой пользовательский ввод. Обратите внимание, что он не является частью ввода.

Пример 1: обычное выполнение

Input an action (add, print, end):
> add
Input the task priority (C, H, N, L):
> H
Input the date (yyyy-mm-dd):
> 2021-12-25
Input the time (hh:mm):
> 14:00
Input a new task (enter a blank line to end):
> Christmas meal
>
Input an action (add, print, end):
> add
Input the task priority (C, H, N, L):
> n
Input the date (yyyy-mm-dd):
> 2022-1-12
Input the time (hh:mm):
> 19:15
Input a new task (enter a blank line to end):
> Dentist
>
Input an action (add, print, end):
> add
Input the task priority (C, H, N, L):
> L
Input the date (yyyy-mm-dd):
> 2021-12-23
Input the time (hh:mm):
> 9:0
Input a new task (enter a blank line to end):
> Supermarket
> -----------
> Pasta
> Butter
> Cheese
>
Input an action (add, print, end):
> print
1  2021-12-25 14:00 H
   Christmas meal

2  2022-01-12 19:15 N
   Dentist

3  2021-12-23 09:00 L
   Supermarket
   -----------
   Pasta
   Butter
   Cheese

Input an action (add, print, end):
> end
Tasklist exiting!

Пример 2: неправильный приоритет

Input an action (add, print, end):
> add
Input the task priority (C, H, N, L):
Critical
Input the task priority (C, H, N, L):
> normal
Input the task priority (C, H, N, L):
> n
Input the date (yyyy-mm-dd):
> 2022-1-1
Input the time (hh:mm):
> 12:00
Input a new task (enter a blank line to end):
> Call friends for new year greetings
>
Input an action (add, print, end):
> end
Tasklist exiting!

Пример 3: неправильная дата

Input an action (add, print, end):
> add
Input the task priority (C, H, N, L):
> N
Input the date (yyyy-mm-dd):
> 2021-2-29
The input date is invalid
Input the date (yyyy-mm-dd):
> 2021-13-1
The input date is invalid
Input the date (yyyy-mm-dd):
> 2021-12-32
The input date is invalid
Input the date (yyyy-mm-dd):
> 2021-12-31
Input the time (hh:mm):
> 12:00
Input a new task (enter a blank line to end):
> Supermarket
>
Input an action (add, print, end):
> end
Tasklist exiting!

Пример 4: неправильное время

Input an action (add, print, end):
> add
Input the task priority (C, H, N, L):
> n
Input the date (yyyy-mm-dd):
> 2021-12-23
Input the time (hh:mm):
> 24:00
The input time is invalid
Input the time (hh:mm):
> 17:60
The input time is invalid
Input the time (hh:mm):
> 9:15
Input a new task (enter a blank line to end):
> Supermarket
>
Input an action (add, print, end):
> end
Tasklist exiting!

Пример 5: пустое задание

Input an action (add, print, end):
> add
Input the task priority (C, H, N, L):
> H
Input the date (yyyy-mm-dd):
> 2021-11-11
Input the time (hh:mm):
> 9:15
Input a new task (enter a blank line to end):
>
The task is blank
Input an action (add, print, end):
> print
No tasks have been input
Input an action (add, print, end):
> end
Tasklist exiting!

4_6

Описание
На этом этапе мы реализуем возможность удаления или редактирования задачи. Кроме того, мы также добавим тег, который будет обозначать, наступила ли дата задачи или уже прошла.

Процесс удаления задачи основан на порядковых номерах задач. После удаления порядковые номера меняются.

Редактирование задачи требует изменения приоритета, даты, времени или описания задачи. Из-за ограничений терминала IntelliJ run редактирование данных из старой задачи невозможно. То есть распечатать старые данные и затем отредактировать их невозможно. Поэтому для каждого из полей выше вам нужно создать еще одно и заменить старое.

Тег «срок» укажет, просрочена ли задача или нет. Это всего лишь одна буква — I, T, или O(без учета регистра). Они обозначают «Вовремя», «Сегодня» и «Просрочено». Чтобы определить тег «срок», мы сравним текущий день с датой задачи.

Ниже приведен пример расчета количества дней от текущей даты до определенной даты с использованием daysUntilфункции из KotlinX datetime, применяемой к LocalDateэкземпляру:

val taskDate = LocalDate(2022, 1, 9)
val currentDate = Clock.System.now().toLocalDateTime(TimeZone.of("UTC+0")).date
val numberOfDays = currentDate.daysUntil(taskDate)

Функция daysUntilвозвращает:

0если taskDateсовпадает с currentDate(тегом due T)
положительное целое число, если taskDateпрошло currentDate(тег времени I)
отрицательное целое число, если taskDateнаходится перед currentDate(тегом due O)
Цели
Измените вводную строку на Input an action (add, print, edit, delete, end):.

Если пользователь вводит delete, распечатайте список задач в новом формате (см. ниже), а затем:

Если задач нет, вывести сообщение: No tasks have been input;
В противном случае запросите у пользователей номер задачи с Input the task number (1-<Maximum task number>):сообщением; если номер задачи выходит за пределы диапазона или не является допустимым натуральным числом, выведите Invalid task numberи снова запросите номер задачи;
Когда задача будет удалена, распечатайте The task is deleted.
Если пользователь вводит edit, распечатайте список задач в новом формате (см. ниже), а затем:

Если задач нет, вывести No tasks have been input;
В противном случае запросите у пользователей номер задачи с Input the task number (1-<Maximum task number>):сообщением; если номер задачи выходит за пределы диапазона или не является допустимым натуральным числом, выведите Invalid task numberи снова запросите номер задачи;
Спросите пользователей, какую часть задачи следует редактировать с помощью Input a field to edit (priority, date, time, task):сообщения; Пользователи должны предоставить одно из priority, date, time, task. Если что-то еще, распечатайте Invalid fieldи запросите поле еще раз;
Когда пользователи вводят данные в допустимое поле, запрашивайте данные в этом поле так же, как и на предыдущем этапе; в случае успеха печатайтеThe task is changed
Если пользователи вводят print, распечатать список задач в новом формате, который включает тег due в конце первой строки каждой задачи. Тег due отделяется одним пробелом. Новый формат представлен ниже:

1  Date1 Time1 Priority1 DueTag1
   Task1-line1
   Task1-line2

2  Date2 Time2 Priority2 DueTag2
   Task2-line1

Примеры
Символ "больше" с последующим пробелом ( > ) представляет собой пользовательский ввод. Обратите внимание, что он не является частью ввода.

Пример 1: обычное выполнение (текущий день — 2022-1-8)

Input an action (add, print, edit, delete, end):
> add
Input the task priority (C, H, N, L):
> h
Input the date (yyyy-mm-dd):
> 2021-12-25
Input the time (hh:mm):
> 14:00
Input a new task (enter a blank line to end):
> Christmas meal
>
Input an action (add, print, edit, delete, end):
> add
Input the task priority (C, H, N, L):
> N
Input the date (yyyy-mm-dd):
> 2022-1-8
Input the time (hh:mm):
> 19:15
Input a new task (enter a blank line to end):
> Dentist
>
Input an action (add, print, edit, delete, end):
> add
Input the task priority (C, H, N, L):
> L
Input the date (yyyy-mm-dd):
> 2022-1-10
Input the time (hh:mm):
> 19:00
Input a new task (enter a blank line to end):
> Supermarket
> -----------
> Pasta
> Butter
> Cheese
>
Input an action (add, print, edit, delete, end):
> print
1  2021-12-25 14:00 H O
   Christmas meal

2  2022-01-08 19:15 N T
   Dentist

3  2022-01-10 19:00 L I
   Supermarket
   -----------
   Pasta
   Butter
   Cheese

Input an action (add, print, edit, delete, end):
> end
Tasklist exiting!

Пример 2: удаление задачи

Input an action (add, print, edit, delete, end):
> add
Input the task priority (C, H, N, L):
> n
Input the date (yyyy-mm-dd):
> 2021-12-25
Input the time (hh:mm):
> 14:00
Input a new task (enter a blank line to end):
> Christmas meal
>
Input an action (add, print, edit, delete, end):
> add
Input the task priority (C, H, N, L):
> L
Input the date (yyyy-mm-dd):
> 2022-1-8
Input the time (hh:mm):
> 19:15
Input a new task (enter a blank line to end):
> Dentist
>
Input an action (add, print, edit, delete, end):
> print
1  2021-12-25 14:00 N O
   Christmas meal

2  2022-01-08 19:15 L T
   Dentist

Input an action (add, print, edit, delete, end):
> delete
1  2021-12-25 14:00 N O
   Christmas meal

2  2022-01-08 19:15 L T
   Dentist

Input the task number (1-2):
> 3
Invalid task number
Input the task number (1-2):
> 1
The task is deleted
Input an action (add, print, edit, delete, end):
> print
1  2022-01-08 19:15 L T
   Dentist

Input an action (add, print, edit, delete, end):
> end
Tasklist exiting!

Пример 3: редактирование полей задачи

Input an action (add, print, edit, delete, end):
> add
Input the task priority (C, H, N, L):
> N
Input the date (yyyy-mm-dd):
> 2022-1-7
Input the time (hh:mm):
> 15:00
Input a new task (enter a blank line to end):
> Supermarket
>
Input an action (add, print, edit, delete, end):
> edit
1  2022-01-07 15:00 N O
   Supermarket

Input the task number (1-1):
> 2
Invalid task number
Input the task number (1-1):
> 1
Input a field to edit (priority, date, time, task):
> tag
Invalid field
Input a field to edit (priority, date, time, task):
> field
Invalid field
Input a field to edit (priority, date, time, task):
> priority
Input the task priority (C, H, N, L):
> L
The task is changed
Input an action (add, print, edit, delete, end):
> edit
1  2022-01-07 15:00 L O
   Supermarket

Input the task number (1-1):
> 1
Input a field to edit (priority, date, time, task):
> date
Input the date (yyyy-mm-dd):
> 2022-1-11
The task is changed
Input an action (add, print, edit, delete, end):
> edit
1  2022-01-11 15:00 L I
   Supermarket

Input the task number (1-1):
> 1
Input a field to edit (priority, date, time, task):
> time
Input the time (hh:mm):
> 19:00
The task is changed
Input an action (add, print, edit, delete, end):
> edit
1  2022-01-11 19:00 L I
   Supermarket

Input the task number (1-1):
> 1
Input a field to edit (priority, date, time, task):
> task
Input a new task (enter a blank line to end):
> Supermarket: Salt, milk
>
The task is changed
Input an action (add, print, edit, delete, end):
> print
1  2022-01-11 19:00 L I
   Supermarket: Salt, milk

Input an action (add, print, edit, delete, end):
> end
Tasklist exiting!

Пример 4: нет задач

Input an action (add, print, edit, delete, end):
> print
No tasks have been input
Input an action (add, print, edit, delete, end):
> edit
No tasks have been input
Input an action (add, print, edit, delete, end):
> delete
No tasks have been input
Input an action (add, print, edit, delete, end):
> end
Tasklist exiting!

5_6

Описание
На этом этапе мы поработаем над форматом распечатки списка задач. Давайте изменим его и добавим немного цветов! Ниже приведен пример нового вывода списка задач:

вывод списка задач

Формат таблицы как текста:

+----+------------+-------+---+---+--------------------------------------------+
| N  |    Date    | Time  | P | D |                    Task                    |
+----+------------+-------+---+---+--------------------------------------------+
| 1  | yyyy-MM-dd | hh:mm |   |   |                                            |
|    |            |       |   |   |                                            |
|    |            |       |   |   |                                            |
+----+------------+-------+---+---+--------------------------------------------+

Если индекс задачи достигает двузначного числа, то он должен занять пробел справа.

Пожалуйста, следите за пробелами! Каждая Taskстрока содержит 44 символа. Если текст больше, напишите первые 44 символа и продолжайте на следующей строке, даже если слово разделено, как в следующем примере:

Строка задачи содержит 44 символа

Цвета не видны во фрагментах, поэтому мы используем изображения, как в разделе «Примеры».

В заголовке Pобозначает Dтеги Priority и Due. Они содержат по 3 пробела каждый и обозначены определенными цветами в среднем пространстве первой строки каждой задачи (см. изображение выше).

Цвета могут использоваться в терминалах, если они поддерживают стандарт escape-последовательностей ANSI. Подробнее об этом можно узнать в статье ANSI escape code в Википедии.

Большинство терминалов Linux, Unix и BSD поддерживают его. Windows 10 cmd поддерживает его по умолчанию, но его нужно включить вручную. Intellij IDEA поддерживает его изначально.

Цвета переднего плана и фона текста можно задать с помощью определенных последовательностей символов и цифр. Чтобы отличить их от обычного текста, им предшествуют непечатаемые экранированные символы ASCII (код символа ASCII — 27). Чтобы включить их в println()распечатку Kotlin, следует использовать их код Unicode, то есть \u001B.

Существуют различные цветовые схемы, мы будем использовать 4-битную. Чтобы задать цвет переднего плана или фона, нужно напечатать \u001B[<Color Code>m, где <Color Code>— целое число, обозначающее цвет. Чтобы сбросить цвета, напечатайте u001B[0m.

В качестве примера:

println("\u001B[101m \u001B[0m")

Устанавливает цвет фона на красный, печатает пробел (который красный), а затем сбрасывает цвета на значения по умолчанию ( 101это число для ярко-красного цвета фона). Один пробел с определенным цветом фона обозначает каждый тег.

Приоритетные цвета:

Приоритетные цвета

Цвета тегов:

Цвета тегов

Цели
Когда пользователи вводят одно из значений print, editили delete, то выводится список задач, как описано выше.

Обратите внимание, что в случае неудачного теста соответствующее сообщение об ошибке не будет отображаться цветами.

Примеры
Символ "больше" с последующим пробелом ( > ) представляет собой пользовательский ввод. Обратите внимание, что он не является частью ввода.

Мы используем изображения, на которых невозможно отобразить цвет.

Пример 1: обычное выполнение (текущий день 2022-1-14)

Input an action (add, print, edit, delete, end):
> add
Input the task priority (C, H, N, L):
> N
Input the date (yyyy-mm-dd):
> 2022-1-14
Input the time (hh:mm):
> 19:00
Input a new task (enter a blank line to end):
> Supermarket
> milk
> cookies
> butter
>
Input an action (add, print, edit, delete, end):
> add
Input the task priority (C, H, N, L):
> C
Input the date (yyyy-mm-dd):
> 2022-1-20
Input the time (hh:mm):
> 20:15
Input a new task (enter a blank line to end):
> Dentist
>
Input an action (add, print, edit, delete, end):
> add
> Input the task priority (C, H, N, L):
L
Input the date (yyyy-mm-dd):
> 2022-1-10
Input the time (hh:mm):
> 12:00
Input a new task (enter a blank line to end):
> Buy book
>
Input an action (add, print, edit, delete, end):
> add
Input the task priority (C, H, N, L):
> H
Input the date (yyyy-mm-dd):
> 2022-1-15
Input the time (hh:mm):
> 00:00
Input a new task (enter a blank line to end):
> Pay bills
>
Input an action (add, print, edit, delete, end):
> print

Вывод строки задачи с соответствующими цветами тегов и приоритетов

Input an action (add, print, edit, delete, end):
> end
Tasklist exiting!

Пример 2: обычное выполнение, более длительные задачи (текущий день 2022-1-14)

Input an action (add, print, edit, delete, end):
> add
Input the task priority (C, H, N, L):
> N
Input the date (yyyy-mm-dd):
> 2022-1-25
Input the time (hh:mm):
> 12:00
Input a new task (enter a blank line to end):
> Remember to review the code for the Tasklist project.
>
Input an action (add, print, edit, delete, end):
> add
Input the task priority (C, H, N, L):
> N
Input the date (yyyy-mm-dd):
> 2022-1-25
Input the time (hh:mm):
> 12:00
Input a new task (enter a blank line to end):
> Find resources about Ansi colors and cursor movement.
> Don't forget to look into the stage 6 links about it.
>
Input an action (add, print, edit, delete, end):
> print

Строка задач с тегами и цветами приоритета

Input an action (add, print, edit, delete, end):
> end
Tasklist exiting!

6_6


Описание
Программа для составления списка задач бессмысленна, если каждый раз, когда вы ее завершаете, список задач стирается. Нам нужен метод сохранения задач, когда программа не запущена. Существует множество решений: база данных, несколько файлов или даже облако. На этом этапе мы собираемся сохранить данные списка задач локально в файл.

Сохранение данных в файле также может принимать различные формы. Вы можете сохранять данные в XML, JSON или любом другом пользовательском формате. Для этого проекта мы выберем JSON с помощью библиотеки JSON Moshi. Если вы хотите узнать об этом больше, взгляните на Github Moshi .

Чтобы получить доступ к Moshiбиблиотеке, ее следует добавить в зависимости вашего проекта, но это уже сделано за вас. Чтобы использовать ее, вам следует просто импортировать ее в свою программу с помощью:

import com.squareup.moshi.*

Данные списка задач следует сохранить в файле с именем tasklist.jsonбез указания путей:

val jsonFile = File("tasklist.json")

Как упоминалось на этапе 3, LocalDateи LocalDateTimeклассы должны быть адаптированы для регистрации в Moshi. Будет проще, если вы не попытаетесь сериализовать их сразу, а будете использовать строки и целые числа для даты и времени и только потом сериализовать данные списка задач.

Цели
Перед завершением работы программы она должна создать файл с именем tasklist.jsonи записать в него все данные, относящиеся к задачам, в формате JSON.
При запуске вашей программы она должна проверить, tasklist.jsonсуществует ли файл. Если существует, прочитайте данные JSON с помощью задач.
Пример
Символ "больше" с последующим пробелом ( > ) представляет собой пользовательский ввод. Обратите внимание, что он не является частью ввода.

Мы будем использовать изображения вместо фрагментов, где цвета не могут быть показаны.

Пример 1: данные сохраняются и загружаются после перезапуска

Input an action (add, print, edit, delete, end):
> print
No tasks have been input
Input an action (add, print, edit, delete, end):
> add
Input the task priority (C, H, N, L):
> N
Input the date (yyyy-mm-dd):
> 2022-1-21
Input the time (hh:mm):
> 12:00
Input a new task (enter a blank line to end):
> Pay bills
>
Input an action (add, print, edit, delete, end):
> add
Input the task priority (C, H, N, L):
> L
Input the date (yyyy-mm-dd):
> 2022-1-12
Input the time (hh:mm):
> 20:00
Input a new task (enter a blank line to end):
> Buy new book
>
Input an action (add, print, edit, delete, end):
> print

Список задач

Input an action (add, print, edit, delete, end):
> end
Tasklist exiting!

Input an action (add, print, edit, delete, end):
> print

Список задач

Input an action (add, print, edit, delete, end):
> end
Tasklist exiting!
