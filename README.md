# diver.vlz — Базовый курс JavaScript.

## Урок 1. Основы языка JavaScript.

__Задание 1__  
Задать температуру в градусах по Цельсию. Вывести в alert соответствующую температуру в градусах по Фаренгейту.  
Подсказка: расчет идет по формуле Tf = (9 / 5) * Tc + 32, где Tf — температура по Фаренгейту, Tc — по Цельсию.

__Задание 2__  
Объявить две переменные: admin и name. Записать в name строку "Василий"; Скопировать значение из name в admin. Вывести admin (должно вывестись «Василий»).

__Задание 3*__  
Чему будет равно JS-выражение 1000 + "108"?

__Задание 4*__  
Самостоятельно разобраться с атрибутами тега script (async и defer).

## Урок 2. Основные операторы JavaScript.

__Задание 1__  
Почему код дает именно такие результаты?  
>var a = 1, b = 1, c, d;  
>c = ++a; alert(c);  // 2  
>d = b++; alert(d);  // 1  
>c = (2+ ++a); alert(c); // 5  
>d = (2+ b++); alert(d); // 4  
>alert(a); // 3  
>alert(b); // 3  

__Задание 2__  
Чему будет равен x?  
>var a = 2;  
>var x = 1 + (a *= 2);

__Задание 3__  
Задание 3. Объявить две целочисленные переменные a и b и задать им произвольные начальные значения.  
Затем написать скрипт, который работает по следующему принципу:  
— если a и b положительные, вывести их разность;  
— если а и b отрицательные, вывести их произведение;  
— если а и b разных знаков, вывести их сумму;  
Ноль можно считать положительным числом.  

__Задание 4__  
Присвоить переменной а значение в промежутке [0..15]. С помощью оператора switch организовать вывод чисел от a до 15.

__Задание 5__  
Реализовать четыре основные арифметические операции в виде функций с двумя параметрами. Обязательно использовать оператор return.

__Задание 6__  
Реализовать функцию с тремя параметрами: function mathOperation(arg1, arg2, operation), где arg1, arg2 — значения аргументов, operation — строка с названием операции.  
В зависимости от переданного значения выполнить одну из арифметических операций (использовать функции из пункта 5) и вернуть полученное значение (применить switch).

__Задание 7*__  
Сравнить null и 0. Объяснить результат.

__Задание 8*__  
С помощью рекурсии организовать функцию возведения числа в степень. Формат:  
>function power(val, pow)  
где val — заданное число, pow –— степень.

## Урок 3. Циклы, массивы, структуры данных.

__Задание 1__  
С помощью цикла while вывести все простые числа в промежутке от 0 до 100.  

__Задание 2__  
С этого урока начинаем работать с функционалом интернет-магазина. Предположим, есть сущность корзины.  
Нужно реализовать функционал подсчета стоимости корзины в зависимости от находящихся в ней товаров.  

__Задание 3__  
Товары в корзине хранятся в массиве. Задачи:  
a. Организовать такой массив для хранения товаров в корзине;  
b. Организовать функцию countBasketPrice, которая будет считать стоимость корзины.  

__Задание 4*__  
Вывести с помощью цикла for числа от 0 до 9, не используя тело цикла. Выглядеть это должно так:  
>for(...){// здесь пусто}  

__Задание 5*__  
Нарисовать пирамиду с 20 рядами с помощью console.log, как показано на рисунке:
>x  
>xx  
>xxx  
>xxxx  
>xxxxx  

## Урок 4. Объекты в JavaScript.  

__Задание 1__  
Написать функцию, преобразующую число в объект. Передавая на вход число от 0 до 999, надо получить на выходе объект, в котором в соответствующих свойствах описаны единицы, десятки и сотни. Например, для числа 245 надо получить следующий объект:  
>{‘единицы’: 5, ‘десятки’: 4, ‘сотни’: 2}  
  Если число превышает 999, необходимо выдать соответствующее сообщение с помощью console.log и вернуть пустой объект.

__Задание 2__  
Продолжить работу с интернет-магазином:  
a. В прошлом домашнем задании вы реализовали корзину на базе массивов. Какими объектами можно заменить их элементы?  
b. Реализуйте такие объекты.  
c. Перенести функционал подсчета корзины на объектно-ориентированную базу.  

__Задание 3*__  
Подумать над глобальными сущностями. К примеру, сущность «Продукт» в интернет-магазине актуальна не только для корзины, но и для каталога. Стремиться нужно к тому, чтобы объект «Продукт» имел единую структуру для различных модулей сайта, но в разных местах давал возможность вызывать разные методы.

## Урок 5. Введение в DOM.  

__Задание 1__  
Создать функцию, генерирующую шахматную доску. Можно использовать любые html-теги. Доска должна быть верно разлинована на черные и белые ячейки. Строки должны нумероваться числами от 1 до 8, столбцы — латинскими буквами A, B, C, D, E, F, G, H.  

__Задание 2__  
Сделать генерацию корзины динамической: верстка корзины не должна находиться в HTML-структуре. Там должен быть только div, в который будет вставляться корзина, сгенерированная на базе JS:  
a. Пустая корзина должна выводить строку «Корзина пуста»;  
b. Наполненная должна выводить «В корзине: n товаров на сумму m рублей».  

__Задание 3*__  
Сделать так, чтобы товары в каталоге выводились при помощи JS:  
a. Создать массив товаров (сущность Product);  
b. При загрузке страницы на базе данного массива генерировать вывод из него. HTML-код должен содержать только div id=”catalog” без вложенного кода. Весь вид каталога генерируется JS.  

## Урок 6. 
__Задание 1__  
Продолжаем реализовывать модуль корзины:  
a. Добавлять в объект корзины выбранные товары по клику на кнопке «Купить» без перезагрузки страницы;  
b. Привязать к событию покупки товара пересчет корзины и обновление ее внешнего	вида.  
__Задание 2*__  
У товара может быть несколько изображений. Нужно:  
a. Реализовать функционал показа полноразмерных картинок товара в модальном окне;  
b. Реализовать функционал перехода между картинками внутри модального окна.  

## Урок 7. 
__Задание 1__  
Реализовать страницу корзины:  
Добавить возможность не только смотреть состав корзины, но и редактировать его, обновляя общую стоимость или выводя сообщение «Корзина пуста».  

__Задание 2__  
На странице корзины:  
a. Сделать отдельные блоки «Состав корзины», «Адрес доставки», «Комментарий»;  
b. Сделать эти поля сворачиваемыми;  
с. Заполнять поля по очереди, то есть давать посмотреть состав корзины, внизу которого есть кнопка «Далее». Если нажать ее, сворачивается «Состав корзины» и открывается «Адрес доставки» и так далее.  

__Задание 3*__  
Для задачи со звездочкой из шестого урока реализовать функционал переключения между картинками по стрелкам на клавиатуре.  
