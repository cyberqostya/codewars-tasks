## Интересные задачи и их решения на JavaScript на [Codewars](https://www.codewars.com/)

 + [Преобразователь числа в строку с разделителем тысяч](#codewars1);

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

### <a name="codewars1"></a>Преобразователь числа в строку с разделителем тысяч

> _(**?:** выражение) - не войдет в результаты поиска_

> _q(**?=** u) соответствует q, за которой следует u, которая не войдет в результат поиска_


```
function numberToPrice(number, roundingCount = 0) {
   return number.toFixed(roundingCount).replace(/(\d)(?=(?:\d{3})+\.)/g, '$1,');
}
```

***
