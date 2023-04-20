# **Scope**

## **Global**
```
No tiene acceso a las variables de tipo local
```

## **Local**
```
Tiene acceso a las variables de tipo global
```

```js
var my_global = "Variable global";

function my_function(){
    var my_local = "Variable local";
    console.log(`Global: ${my_global} - Local: ${my_local}`);
}

console.log(my_global);
my_function();
console.log(my_local);
```

```
Variable global
Global: Variable global - Local: Variable local
Uncaught ReferenceError: my_local is not defined
    at <anonymous>:10:13
```
