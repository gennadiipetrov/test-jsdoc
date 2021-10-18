# Bind, call, apply

Для связи определенного контекста к объекту используют эти функции

```js
person.logInfo.bind(lena, "back", 20)();
```

* *person.logInfo* - функция
* *lena* - объект то что будет this
* *"back", 20* - аргументы


call - без скобок

```js
person.logInfo.call(lena, "back", 20);
```

apply - аргументы в виде массива
```js
person.logInfo.apply(lena, ["back", 20]);
```

То есть все эти функции отличаются передачей аргументов.

# Отличие Bind от Call

```js
obj.bind(obj2)();
```