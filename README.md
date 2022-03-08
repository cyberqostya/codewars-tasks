## Интересные задачи и их решения на JavaScript на [Codewars](https://www.codewars.com/)

#### [Medium](#mediumtasks)
  + [Преобразователь числа в строку с разделителем тысяч](#codewars1);
  + [Заменить {field} в строке на значение в объекте](#codewars3);
#### [Easy](#easytasks)
  + [Наибольшее и наименьшее числа из массива](#codewars2);

***
### <a name="mediumtasks"></a> Medium
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
### <a name="codewars3"></a>Заменить {field} в строке на значение в объекте

```
// Принимает 
//   string = "Hello, {name}! I was born in {year}. I'm from {place}."
//   obj = {
//     name: "Harry Potter",
//     year: 1980,
//     place: "Godric's Hollow"
//   }

function pseudoTemplateString(string, obj) {
  return (
    string.replace(/{\w+}/g, (val) => {
      return obj[val.match(/\w+/)[0]];
    })
  )
}
```




***
### <a name="easytasks"></a> Easy
***
### <a name="codewars2"></a>Наибольшее и наименьшее числа из массива
> _В задаче функция принимала строку типа ```'1 2 -4 5'``` и для преобразования использовалась ```string.split(' ').map(Number)```_

```
function highAndLow(array){
  return `Max: ${Math.max(...array)}, Min: ${Math.min(...array)}`;
}
```

***
