###Задание

Выведите на экран значение следующих выражений:

####ArithmeticSolution.php
Произведение двух подвыражений, одно из которых это семь во второй степени, а второе это разность между остатком от деления ста на три и цифрой пять.

####FunctionSolution.php
Квадратный корень из суммы двух подвыражений, одно из которых это косинус pi радиан, а вторая это синус девяноста градусов.

####Решения

```php
<?php

// BEGIN (write your solution here)
echo (7 ** 2) * ((100 % 3) - 5);
// END
```

```php
<?php

// BEGIN (write your solution here)
echo sqrt(cos(pi()) + sin(deg2rad(90)));    
// END
```