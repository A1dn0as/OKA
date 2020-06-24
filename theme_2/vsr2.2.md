# Переменные. 
# Объявление целых чисел и чисел с плавающей точкой.

**Для присвоения значения переменной в Scilab используется бинарный оператор "=". Слева от оператора присвоения должно находиться имя переменной, справа - значение этой переменной.**

Если в конце выражения поставить знак точки с запятой ";" - результат присвоения не будет сразу выведен на экран.

### Примеры:

variable1 = 3.5
Переменной variable1 присваивается значение 3.5, результат выводится на экран.

variable2 = 20;
Переменной variable2 присваивается значение 20, результат НЕ выводится на экран.


## Объявление дробей.

**Для объявления дроби необходимо либо записать её представление в обычном виде m/n, где m - числитель, n - знаменатель; либо записать её представление в виде десятичной дроби. Также возможно опускать ноль до точки, если модуль переменной меньше единицы.**

- variable1 = -(4/5);
- variable2 = -0.8;
- variable3 = 16/-20;
- variable4 = -.8;
Различные представления числа -0.8.


### Объявление матриц и множеств.

**Для объявления матрицы или множества необходимо перечислить её элементы внутри квадратных скобок. Во множестве не может быть повторяющихся элементов.**

set = [3, 2, -6];
Множество из трёх элементов.

matrix = [[3, 2, -6]; [1, 5, 3]];
Матрица 3x2.


### Обьявление пользовательских функций.

**Для объявления функции в Scilab существует ключевое слово function, после которого в квадратных скобках идёт возвращаемое значение, знак равенства, имя функции и аргументы в скобках.**

**Пример объявления функции, возводящей числа в квадрат:**

function [ret]=discr(a, b, c)
ret=b^2 - 4*a*c
endfunction

**Пример вызова функции:**

discr(2, 5, -7)
При вызове переданные аргументы подставляются в выражение, затем вычисляется и возвращается результат.