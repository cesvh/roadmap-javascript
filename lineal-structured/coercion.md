# **Coerción**

```
Cambio de una variable de un tipo a otro de manera implícita (Cuando el lenguaje lo hace por nosotros) o explícita (Cuando lo hacemos nosotros)
```

## **Coerción implícita**
```js
var suma = 5 + "5";
console.log(suma);
console.log(typeof(suma));
```

```
55
string
```

## **Coerción explícita**
```js
var suma = parseInt("5") + Number("5");
console.log(suma);
console.log(typeof(suma));
```

```
10
number
```
