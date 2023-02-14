# JavaScript-Questions


1. `'use strict'`?

Это директива, указывающая на то, что код JS должен выполняться в строгом режиме. Она располагается в начале всего кода либо в начале блока кода.

Отменить строгий режим невозможно.

***

2. "Строгий режим"?

Строгий режим:
- запрещает использование недекларированных переменных;
- преобразует "тихие" ошибки в исключения, например при попытке:
  * присваивания значения свойству, предназначенному только для чтения, вроде некоего неперезаписываемого глобального свойства;
  * записи значения в свойство, у которого есть лишь геттер;
  * записи чего-либо в свойство нерасширяемого объекта;
- защищает программиста от непреднамеренного создания глобальных переменных.

***

3. `var`, `const` и `let` - в чем разница?

- переменные с `let` нельзя объявить повторно;
- `const` и `let` имеют блочную видимость;
- `var` можно объявлять глобальные переменные, но это не рекомендуется;
- попытка изменить `const` приведет к ошибке (но не попытка изменить поле объекта).

***

4. ECMAScript6

Глобальное обновление JS, датируемое 2015г - стандарт написания кода на JS.

***

5. Область видимости?

Ограниченная часть программы, в которой можно обратиться к переменной, функции или объекту -функция, блок или вся программа в целом.

***

6. Типизация в JS?

JS - слабо-типизируемый язык - тип переменной не указывается явно. 

Во время выполнения программы переменные могут принимать любой тип данных, а операции - тип переменных. Результат операций может приводиться к другому типу данных.

***

7. Иммутабельность?

Неизменяемость объекта.

Чтобы сделать объект иммутабельным, используется метод объекта `freeze()`.

Проверка объекта на изменяемость - `isFrozen()`.

***

8. Типы данных в JS?

- undefined
- Boolean
- Number
- String
- BigInt
- Symbol
- Null
- object

***

9. Проверка, является ли объект массивом?

Применяется метод объекта `isArray()`.

***

10. Проверка, является ли число конечным?

Применяется метод объекта `isFinite()`: `false`, если NaN, +♾️ или -♾️; иначе - `true`.

***

11. Метод `eval()`?

Позволяет выполнить в программе JS-код, представленный строкой. Если код не возвращает ничего, так же как всегда вернется `undefined`.

***

12. Проверка на NaN?

Применяется метод объекта `inNaN()`. **ВАЖНО**: Он преобразует значение в число, затем проверяет.

`Number.isNaN` не преобразует значение в число и не возвращает `true` для любого значения, не являющегося числом. 

Предпочтительнее последний вариант.

***

13. Immediately Invoked Function Expression?

JS-функция, которая выполняется сразу после объявления.

***

14. Деструктуризация?

Особый синтаксис присваивания сразу нескольким переменным значения элементов массива:
```javascript
const namesArray = new Array['Sergei', 'Ivan'];
let [firstName, secondName] = namesArray;
```

***

15. Оператор `in` и метод `hasOwnProperty` - разница?

Каждый Объект, пришедший от object, наследует метод `hasOwnProperty`. Метод используется для определения того, содержит ли Объект указанное свойство в качестве собственного свойства Объекта.

В отличие от оператора `in` он не проверяет существующие свойства в цепочке прототипов Объекта.

***

16. Проверка, существует ли подстрока в строке?



***

17. Временная мёртвая зона?

Часть программы между определением переменной и присвоением ему значения

***

18. Замыкание в JS?



***

19. Методы `setTimeout` и setInterval?


***



***



***



***

