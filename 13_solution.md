### Задание

Реализуйте функцию `uniq`, которая принимает, как аргумент, массив, и возвращает массив, в котором оставлены только уникальные значения из исходного массива.

Пример:

```php
[12, 1, 3, 5, 10] == uniq([12, 1, 1, 3, 5, 10, 3, 10])
```

#### Подсказки

Создайте внутри новый массив и заполняйте его уникальными значениями.

#### Решение

```php
<?php

namespace App\Solution;

// BEGIN (write your solution here)
function uniq(array $arr)
{
    $arr2 = [];
    for ($i = 0; $i < sizeof($arr); $i++) {
        if (in_array($arr[$i], $arr2)) {
            continue;
        }
        $arr2[] = $arr[$i];
    };

    return $arr2;
}
// END
```
#### Альтернативное решение

```php
<?php

namespace App\Solution;

// BEGIN (write your solution here)
function uniq(array $arr)
{
    $arr2 = [];
    
    for ($i = 0; $i < sizeof($arr); $i++) {
        if(!in_array($arr[$i], $arr2)) {
            $arr2[] = $arr[$i];
        }
    }
    
    
    return $arr2;
}
// END
```
