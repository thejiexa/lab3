## МИНИСТЕРСТВО НАУКИ И ВЫСШЕГО ОБРАЗОВАНИЯ РОССИЙСКОЙ ФЕДЕРАЦИИ ФЕДЕРАЛЬНОЕ ГОСУДАРСТВЕННОЕ БЮДЖЕТНОЕ ОБРАЗОВАТЕЛЬНОЕ УЧРЕЖДЕНИЕ ВЫСШЕГО ОБРАЗОВАНИЯ «САХАЛИНСКИЙ ГОСУДАРСТВЕННЫЙ УНИВЕРСИТЕТ»
Институт естественных наук и техносферной безопасности
Кафедра информатики
Григораш Алексей Владимирович
Лабораторная работа № 9
“JavaScript”
01.03.02 Прикладная математика и информатика
Научный руководитель
Соболев Евгений Игоревич
Южно-Сахалинск
2022 г. 
 
Введение
С помощью JavaScript Вы сможете создавать интерактивные веб-страницы.
Интерактивные страницы могут взаимодействовать с пользователем (выводить сообщения, изменять содержимое после определенных действий и т.д.)
JavaScript встраивается прямо в веб-страницы и исполняется браузером во время их загрузки.
JavaScript был создан в 1995 году как инструмент, предоставляющий веб-дизайнерам возможности программирования. JavaScript обладает простым синтаксисом и его очень легко изучить.
Все современные браузеры имеют поддержку JavaScript.

Задачи:

1. Что выведет код ниже?
alert( null || 2 || undefined );1

2. Что выведет код ниже?
alert( alert(1) || 2 || alert(3) );

3. Что выведет код ниже?
alert( 1 && null && 2 );

4. Что выведет alert (И)?
alert( alert(1) && alert(2) );

5. Что выведет этот код?
alert( null || 2 && 3 || 4 );

6. Напишите условие if для проверки, что переменная age находится в диапазоне между 14 и 90 включительно. «Включительно» означает, что значение переменной age может быть равно 14 или 90.

7.Напишите условие if для проверки, что значение переменной age НЕ находится в диапазоне 14 и 90 включительно. Напишите два варианта: первый с использованием оператора НЕ !, второй – без этого оператора.

8. Какие из перечисленных ниже alert выполнятся?
Какие конкретно значения будут результатами выражений в условиях if(...)?

if (-1 || 0) alert( 'first' );
if (-1 && 0) alert( 'second' );
if (null || -1 && 1) alert( 'third' );

9. Проверка логина
важность: 3
Напишите код, который будет спрашивать логин с помощью prompt.

Если посетитель вводит «Админ», то prompt запрашивает пароль, если ничего не введено или нажата клавиша Esc – показать «Отменено», в противном случае отобразить «Я вас не знаю».

Пароль проверять так:

![2](https://trueimages.ru/img/e0/55/93854236.png)

Если введён пароль «Я главный», то выводить «Здравствуйте!»,
Иначе – «Неверный пароль»,
При отмене – «Отменено».
Блок-схема:
 
Для решения используйте вложенные блоки if. Обращайте внимание на стиль и читаемость кода.

Подсказка: передача пустого ввода в приглашение prompt возвращает пустую строку ''. Нажатие клавиши Esc во время запроса возвращает null.

10. Какое последнее значение выведет этот код? Почему?
let i = 3;
while (i) {
  alert( i-- );
}

11. Для каждого цикла запишите, какие значения он выведет. Потом сравните с ответом.

Оба цикла выводят alert с одинаковыми значениями или нет?

Префиксный вариант ++i:

let i = 0;
while (++i < 5) alert( i );

Постфиксный вариант i++

let i = 0;
while (i++ < 5) alert( i );

12. Для каждого цикла запишите, какие значения он выведет. Потом сравните с ответом. Оба цикла выведут alert с одинаковыми значениями или нет?

Постфиксная форма:
for (let i = 0; i < 5; i++) alert( i );

Префиксная форма:
for (let i = 0; i < 5; ++i) alert( i );

13. При помощи цикла for выведите чётные числа от 2 до 10.

14. Перепишите код, заменив цикл for на while, без изменения поведения цикла.
for (let i = 0; i < 3; i++) {
  alert( `number ${i}!` );
}

15. Напишите цикл, который предлагает prompt ввести число, большее 100. Если посетитель ввёл другое число – попросить ввести ещё раз, и так далее. Цикл должен спрашивать число пока либо посетитель не введёт число, большее 100, либо не нажмёт кнопку Отмена (ESC). Предполагается, что посетитель вводит только числа. Предусматривать обработку нечисловых строк в этой задаче необязательно.

16. Натуральное число, большее 1, называется простым, если оно ни на что не делится, кроме себя и 1. Другими словами, n > 1 – простое, если при его делении на любое число кроме 1 и n есть остаток. Например, 5 — это простое число, оно не может быть разделено без остатка на 2, 3 и 4. Напишите код, который выводит все простые числа из интервала от 2 до n. Для n = 10 результат должен быть 2,3,5,7.

17. Напишите if..else, соответствующий следующему switch:
switch (browser) {
  case 'Edge':
    alert( "You've got the Edge!" );
    break;
  case 'Chrome':
  case 'Firefox':
  case 'Safari':
  case 'Opera':
    alert( 'Okay we support these browsers too' );
    break;

  default:
    alert( 'We hope that this page looks ok!' );
}

18. Перепишите код с использованием одной конструкции switch:
 const number = +prompt('Введите число между 0 и 3', '');

if (number === 0) {
  alert('Вы ввели число 0');
}

if (number === 1) {
  alert('Вы ввели число 1');
}

if (number === 2 || number === 3) {
  alert('Вы ввели число 2, а может и 3');
}

19. Следующая функция возвращает true, если параметр age больше 18. В ином случае она запрашивает подтверждение через confirm и возвращает его результат:

function checkAge(age) {
  if (age > 18) {
    return true;
  } else {
    // ...
    return confirm('Родители разрешили?');
  }
}
Будет ли эта функция работать как-то иначе, если убрать else?

function checkAge(age) {
  if (age > 18) {
    return true;
  }
  // ...
  return confirm('Родители разрешили?');
}
Есть ли хоть одно отличие в поведении этого варианта?

20. Следующая функция возвращает true, если параметр age больше 18. В ином случае она задаёт вопрос confirm и возвращает его результат.

function checkAge(age) {
  if (age > 18) {
    return true;
  } else {
    return confirm('Родители разрешили?');
  }
}
Перепишите функцию, чтобы она делала то же самое, но без if, в одну строку.

Сделайте два варианта функции checkAge:

Используя оператор ?
Используя оператор ||

21. Напишите функцию min(a,b), которая возвращает меньшее из чисел a и b.

Пример вызовов:
min(2, 5) == 2
min(3, -1) == -1
min(1, 1) == 1

22. Напишите функцию pow(x,n), которая возвращает x в степени n. Иначе говоря, умножает x на себя n раз и возвращает результат.
pow(3, 2) = 3 * 3 = 9
pow(3, 3) = 3 * 3 * 3 = 27
pow(1, 100) = 1 * 1 * ...* 1 = 1
Создайте страницу, которая запрашивает x и n, а затем выводит результат pow(x,n).

23. 7 kyu https://www.codewars.com/kata/highest-and-lowest
24. 7 kyu https://www.codewars.com/kata/disemvowel-trolls
25. 7 kyu https://www.codewars.com/kata/isograms
26. 7 kyu https://www.codewars.com/kata/digits-explosion
27. 6 kyu https://www.codewars.com/kata/handshake-problem
28. 6 kyu https://www.codewars.com/kata/duplicate-encoder
29. 6 kyu https://www.codewars.com/kata/n-th-fibonacci
30. 6 kyu https://www.codewars.com/kata/multiples-of-3-or-5

## Решение:
```JavaScript

<p>1, 2, 3, 4, 5 <br>
    <button onclick="alert(null || 2 || undefined )">null || 2 || undefined </button>
    <button onclick="alert(alert(1) || 2 || alert(3) )">alert(1) || 2 || alert(3) </button>
    <button onclick="alert(1 && null && 2 )">1 && null && 2 </button>
    <button onclick="alert(alert(1) && alert(2))">alert(1) && alert(2)</button>
    <button onclick="alert(null || 2 && 3 || 4 )">null || 2 && 3 || 4 </button>
</p>

<p>6, 7 <br>
    <script>
        function AgeCheck6(age){
            if (!age) alert(`не число`)
            else if (age >= 14 && age <= 90)
                alert(`${age} находится в диапазоне между 14 и 90 включительно`);
            else alert(`${age} НЕ находится в диапазоне между 14 и 90 включительно`);
        }
        function AgeCheck7A(age){
            if (!age) alert(`не число`)
            else if (!(age >= 14 && age <= 90))
                alert(`${age} НЕ находится в диапазоне между 14 и 90 включительно`);
            else alert(`${age} находится в диапазоне между 14 и 90 включительно`);
        }
        function AgeCheck7B(age){
            if (!age) alert(`не число`)
            else if (age < 14 || age > 90)
                alert(`${age} НЕ находится в диапазоне между 14 и 90 включительно`);
            else alert(`${age} находится в диапазоне между 14 и 90 включительно`);
        }
    </script>
    <button onclick="AgeCheck6(+prompt('Введите число'))">6</button>
    <button onclick="AgeCheck7A(+prompt('Введите число'))">7.1</button>
    <button onclick="AgeCheck7B(+prompt('Введите число'))">7.2</button>
</p>

<p>8<br>
    <script>
        function Method8(){
            if (-1 || 0) alert( 'first' );
            if (-1 && 0) alert( 'second' );
            if (null || -1 && 1) alert( 'third' );
        }
    </script>
    <button onclick="Method8()">Какие из перечисленных ниже alert выполнятся</button>
</p>

<p>9<br>
    <script>
        let login = '';
        let thePass = '';
        function Login(){
            login = prompt('Введите логин:')
            if (login == null || login == ''){
                alert('Отменено');
            }
            else if (login.toLowerCase() == 'Админ'.toLowerCase()){
                thePass = prompt('Введите пароль:');
                if (thePass == null || thePass == ''){
                alert('Отменено');
                }
                else if (thePass != 'Я главный'){
                    alert('Неверный пароль');
                }
                else {
                    alert('Здравствуйте!');
                }
            }
            else {
                alert('Я вас не знаю');
            }
        }
    </script>
    <button onclick="Login()">Проверка логина</button>
</p>

<p>10<br>
    <script>
        function Method10(){
            let i = 3;
            while (i) {
                alert( i-- );
            }
        }
    </script>
    <button onclick="Method10()">10</button>
</p>

<p>11<br>
    <script>
        function Method11(b){
            let i = 0;
            if (b) while (++i < 5) alert(i);
            else while (i++ < 5) alert(i);
        }
    </script>
    <button onclick="Method11(true)">Префиксный вариант ++i</button>
    <button onclick="Method11(false)">Постфиксный вариант i++</button>
</p>

<p>12 <br>
    <script>
        function Method12(b){
            if (b) for(let i = 0; i < 5; i++) alert(i);
            else for(let i = 0; i < 5; ++i) alert(i);
        }
    </script>
    <button onclick="Method12(true)">Постфиксная форма</button>
    <button onclick="Method12(false)">Префиксная форма</button>
</p>

<p>13 <br>
    <script>
        function From2to10(){
            let result = "";
            for(let i = 2; i < 11; i++) 
                if (i % 2 == 0) 
                    result += `${i} `;
            return result;
        }
    </script>
    <button onclick="alert(From2to10())">При помощи цикла for выведите чётные числа от 2 до 10.</button>
</p>

<p>14<br>
    <script>
        function WhileInsteadFor(){
            let i = 0;
            while (i < 3){
                i++;
                alert(`number ${i}`);
            }
        }
    </script>
    <button onclick="alert(WhileInsteadFor())">Перепишите код, заменив цикл for на while</button>
</p>

<p>15 <br>
    <script>
        function Method15(n){
            while(!n || n <= 100){
                n = prompt('Введите число больше 100');
                if (n == null) break;
            }
        }
    </script>
    <button onclick="Method15(+prompt('Введите число'))">ввести число, большее 100</button>
</p>

<p>16 <br>
    <script>
        function Method16(n){
            while (!n || n < 2) n = +prompt('Введите число больше 2');
            let s = '';
            /* for (let i = 2; i < n; i++)
                if (i %  2 != 0 && i %  3 != 0 && i %  5 != 0) s += `${i} `
            alert(s); */
            for (let i = 2; i <= n; i++)
            {
                let j;
                for ( j = 2; j <= Math.sqrt(i); j++)
                {
                    if (i % j == 0)
                    {
                        break;
                    }
                }
                if(j > Math.sqrt(i))
                {
                    s += `${i} `;
                }

            }
            alert(s);
        }
    </script>
    <button onclick="Method16(+prompt('Введите число больше 2'))">простые числа из интервала от 2 до n</button>
</p>

<p>17 <br>
    <script>
        function Browser(browser){
            while (browser == '') browser = prompt('Выберите браузер:').toLocaleLowerCase();
            if (browser == 'edge') alert( "You've got the Edge!" );
            else if (browser == 'chrome' || browser == 'firefox' || browser == 'safari' || browser == 'opera' ) alert( 'Okay we support these browsers too' );
            else alert( 'We hope that this page looks ok!' );
        }
    </script>
    <button onclick="Browser(prompt('Выберите браузер:').toLocaleLowerCase())">Выберите браузер</button>
</p>

<p>18<br>
    <script>
        function Method18(){
            const number = +prompt('Введите число между 0 и 3', 0);
            switch(number){
                case 0:
                    alert('Вы ввели число 0');  
                    break;
                case 1:
                    alert('Вы ввели число 1'); 
                    break;
                case 2:
                case 3:
                    alert('Вы ввели число 2 или 3'); 
                    break;
                default:
                    Method18();
                    break;
            }
        }
    </script>
    <button onclick="Method18()">Введите число между 0 и 3</button>
</p>

<p>19, 20<br>
    <script>
        function checkAge1(age) {
            if (age > 18) {
                return true;
            } else {
                // ...
                return confirm('Родители разрешили?');
            }
        }
        function checkAge2(age) {
            if (age > 18) {
                return true;
            }
            // ...
            return confirm('Родители разрешили?');
        }
        function checkAge3(age) {
            age > 18 ? true : confirm('Родители разрешили?')
        };
        function checkAge4(age) {
            age > 18  || confirm('Родители разрешили?')
        };
    </script>
    <button onclick="checkAge1(+prompt('checkAge1'))">checkAge1</button>
    <button onclick="checkAge2(+prompt('checkAge2'))">checkAge2</button>
    <button onclick="checkAge3(+prompt('checkAge3'))">checkAge3</button>
    <button onclick="checkAge4(+prompt('checkAge4'))">checkAge4</button>
</p>

<p>21, 22<br>
    <script>
        function min(a, b) {
            alert(a > b ? b : a);
        }
        function pow(x, n){
            let result = x * 1.0;
            if (n == 0){
                result = 1;
            }
            else if (n > 0){
                for (let i = 1; i < n; i++)
                    result *= x;
            }
            else {
                /* for (let i = 1; i < n; i++)
                    result *= x;
                result = 1 / result; */
                result **= n;
            }
            alert(result);
        }
    </script>
    <button onclick="min(+prompt('a:'), +prompt('b:'))">min(a,b)</button>
    <button onclick="pow(+prompt('x:'), +prompt('n:'))">pow(x,n)</button>
</p>
```



[Задания 23 - 30](https://www.codewars.com/users/thejiexa/completed_solutions)

## Вывод:
В ходе выполнения задач повторил работу c переменными, операторами, способами вывода, циклами, функциями.
