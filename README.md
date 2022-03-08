## Интересные задачи и их решения на JavaScript на [Codewars](https://www.codewars.com/)

1. 5 level
 + [Преобразователь числа в строку с разделителем тысяч](#codewars1);
1. 7 level
 + [Наибольшее и наименьшее числа из массива](#codewars2);

***
### <a name="codewars1"></a>Преобразователь числа в строку с разделителем тысяч
> _(**?:** выражение) - не войдет в результаты поиска_
> 
> _q(**?=** u) соответствует q, за которой следует u, которая не войдет в результат поиска_

```
function numberToPrice(number, roundingCount = 0) {
   return number.toFixed(roundingCount).replace(/(\d)(?=(?:\d{3})+\.)/g, '$1,');
}
```

***
### <a name="codewars2"></a>Наибольшее и наименьшее числа из массива
> _В задаче функция принимала строку типа '1 2 -4 5' и для преобразования использовалась ```string.split(' ').map(Number)```_

```
function highAndLow(array){
  return `Max: ${Math.max(...array)}, Min: ${Math.min(...array)}`;
}
```

***
