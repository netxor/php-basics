#Задание

Напишите функцию `sumWith`, которая вычисляет сумму последовательности применяя к каждому элементу последовательности функцию переданную как аргумент. Границы последовательности должны быть включены в процесс сложения.

Пример:

```php 
$func = function ($number) {
    return $number * 2;
};

12 == sumWith(1, 3, $func); // 1 * 2 + 2 * 2 + 3 * 2
42 == sumWith(10, 11, $func); // 10 * 2 + 11 * 2
```
