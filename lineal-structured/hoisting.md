# **Hoinsting**

```
Es un proceso que realiza el compilador, ejecuta las variables y funciones primero antes de cualquier otro código y luego sigue con el proceso normal.

Si es una variable lo lleva al principio del código y solo lo declara, por lo tanto es una variable del tipo undefined

Primero declara las funciones y luego las variables.

Solo sucede en versiones anteriores a ES6, tras la incorporación de CONST y LET
```

## **Escenario con variables**
```js
console.log(my_variable);
var my_variable = "Mi valor";
```

```js
undefined // Este corresponde al console.log que solo es una variable declarada del tipo undefined
```

```js
console.log(my_variable + " Solo estoy declarada sin inicializar");
var my_variable = "Mi valor";
console.log(my_variable);
```

```js
undefined Solo estoy declarada sin inicializar
Mi valor
```

## **Escenario con funciones**

```js
main();

function main() {
    console.log("Hola");
}
```

```
Hola
```
