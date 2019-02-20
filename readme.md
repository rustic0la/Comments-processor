
Утилита будет брать все файлы с расширением .js в текущей директории, находить в них 
все комментарии с TODO. Искать по ним, фильтровать, сортировать.

Команды

1. exit : завершение работы программы
2. show : показать все todo
3. important : показывать только todo, в которых есть восклицательный знак.
В комментарии может присутствовать восклицательный знак (!), что означает, что это задача с высоким приоритетом.
4. user {username} : показывать только комментарии от указанного пользователя .
Имя пользователя должно быть регистронезависимо. Пример команды: "user veronika"
5. sort {importance | user | date} : выводит отсортированные todo 
Если аргумент importance, то сначала выводятся комментарии с восклицательными знаками, потом все остальные.  Чем больше
восклицательных знаков, тем выше приоритет и тем выше в списке этот комментарий. 
Если аргумент user, то выводятся задачи сгрупированные по пользователям, а в конце безымянные. 
Если аргумент date, то выводятся сначала самые новые, потом постарше, потом без дат. 
Примеры команд: "sort importance", "sort user", "sort date"
6. date {yyyy[-mm-dd]}: показывает все комментарии, созданные после переданной даты (включительно). 
Датой может быть только год, год с месяцем (через дефис) или год с месяцем и днем. 
Примеры команд: "date 2015", "date 2016-02", "date 2018-03-02".
В ответ на команду  "date 2015" ожидается список todo, которые были созданы в 2015 году и позже.

Если введена команда не из этого списка, то в консоль должен выводиться текст "wrong command".
В начале работы приложения, оно должна писать в консоль приглашение ввести команду: "Please, write your command!".

[![asciicast](https://asciinema.org/a/228611.png)](https://asciinema.org/a/228611)
