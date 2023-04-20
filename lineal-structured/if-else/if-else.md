# **if - else - else if**

## **if**

```js
var edad = 17;

if (edad < 18) {
    console.log(`Menor de edad`);
}
```

```
Menor de edad
```

## **if -else**

```js
var edad = 31;

if (edad < 18) {
    console.log(`Menor de edad`);
} else {
    console.log(`Mayor de edad`);
}
```

```
Mayor de edad
```

## **if - else Anidados**

```js
var edad = 31;

if (edad < 18) {
    console.log(`Menor de edad`);
} else {
    if (edad >= 18 && edad <= 31) {
        console.log(`Entre 18 y 31 años`);
    } else {
        if (edad > 31 && edad <= 45) {
            console.log(`Entre 31 y 45 años`);
        } else {
            console.log(`Mayor a 45 años`);
        }
    }
}
```

```
Entre 18 y 31 años
```

## **else if**

```js
var edad = 31;

if (edad < 18) {
    console.log(`Menor de edad`);
} else if (edad >= 18 && edad <= 31) {
    console.log(`Entre 18 y 31 años`);
} else if (edad > 31 && edad <= 45) {
    console.log(`Entre 31 y 45 años`);
} else if (edad > 45) {
    console.log(`Mayor a 45 años`);
}
```

```
Entre 18 y 31 años
```

## **Operador ternario**

```js
var edad = 31;

var resultado = (edad > 18) ? "Mayor" : "Menor";

console.log(resultado);
```

```
Mayor
```
