# **Recorrer un array**

Filter.
Map.
Find.
ForEach.
Some.

---

Filter: Crea un nuevo arreglo con todos los elementos que cumplen con la condición:
```js
var libros = [
  { nombre: "la joven de las naranjas", costo: 245 },
  { nombre: "el problema de los 3 cuerpos", costo: 459 },
  { nombre: "festin de cuervos", costo: 200 },
  { nombre: "el mundo de sofia", costo: 420 },
  { nombre: "de animales a dioses", costo: 450 },
  { nombre: "arkhan asylum", costo: 350 },
  { nombre: "the sandman", costo: 1700 },
];

var libros_filtrados = libros.filter(item => {
    return item.costo < 400;
});

console.log(libros_filtrados);
```
Nos ha retornado un nuevo arreglo con los elementos que el costo es menor de 400:
```
(3) [{…}, {…}, {…}]
0: {nombre: 'la joven de las naranjas', costo: 245}
1: {nombre: 'festin de cuervos', costo: 200}
2: {nombre: 'arkhan asylum', costo: 350}
length: 3
[[Prototype]]: Array(0)
```

---

Map: Retorna un nuevo arreglo, que recorre cada elemento del arreglo dado y lo transforma en lo que se desee.
```js
var libros = [
  { nombre: "la joven de las naranjas", costo: 245 },
  { nombre: "el problema de los 3 cuerpos", costo: 459 },
  { nombre: "festin de cuervos", costo: 200 },
  { nombre: "el mundo de sofia", costo: 420 },
  { nombre: "de animales a dioses", costo: 450 },
  { nombre: "arkhan asylum", costo: 350 },
  { nombre: "the sandman", costo: 1700 },
];

var librosDecorados1 = libros.map(item => {
    return item.nombre;
});

var librosDecorados2 = libros.map(item => {
    return [item.nombre.toUpperCase(), `$${item.costo}`];
});
```

```js
console.log(librosDecorados1);
```

```
(7) ['la joven de las naranjas', 'el problema de los 3 cuerpos', 'festin de cuervos', 'el mundo de sofia', 'de animales a dioses', 'arkhan asylum', 'the sandman']
0: "la joven de las naranjas"
1: "el problema de los 3 cuerpos"
2: "festin de cuervos"
3: "el mundo de sofia"
4: "de animales a dioses"
5: "arkhan asylum"
6: "the sandman"
length: 7
[[Prototype]]: Array(0)
```

```js
console.log(librosDecorados2);
```

```
(7) [Array(2), Array(2), Array(2), Array(2), Array(2), Array(2), Array(2)]
0: (2) ['LA JOVEN DE LAS NARANJAS', '$245']
1: (2) ['EL PROBLEMA DE LOS 3 CUERPOS', '$459']
2: (2) ['FESTIN DE CUERVOS', '$200']
3: (2) ['EL MUNDO DE SOFIA', '$420']
4: (2) ['DE ANIMALES A DIOSES', '$450']
5: (2) ['ARKHAN ASYLUM', '$350']
6: (2) ['THE SANDMAN', '$1700']
length: 7
[[Prototype]]: Array(0)
```

Find: Retorna el primer elemento que cumpla con la condición
```js
var libros = [
  { nombre: "la joven de las naranjas", costo: 245 },
  { nombre: "el problema de los 3 cuerpos", costo: 459 },
  { nombre: "festin de cuervos", costo: 200 },
  { nombre: "el mundo de sofia", costo: 420 },
  { nombre: "de animales a dioses", costo: 450 },
  { nombre: "arkhan asylum", costo: 350 },
  { nombre: "the sandman", costo: 1700 },
];

var encuentra_articulo = libros.find(item => {
    return item.costo > 300;
});
```

```
{nombre: 'el problema de los 3 cuerpos', costo: 459}
costo: 459
nombre: "el problema de los 3 cuerpos"
[[Prototype]]: Object
```

ForEach: Recorre cada elemento del arreglo:
```js
var libros = [
  { nombre: "la joven de las naranjas", costo: 245 },
  { nombre: "el problema de los 3 cuerpos", costo: 459 },
  { nombre: "festin de cuervos", costo: 200 },
  { nombre: "el mundo de sofia", costo: 420 },
  { nombre: "de animales a dioses", costo: 450 },
  { nombre: "arkhan asylum", costo: 350 },
  { nombre: "the sandman", costo: 1700 },
];

libros.forEach(item => {
    console.log(item.nombre);
});
```

```
la joven de las naranjas
el problema de los 3 cuerpos
festin de cuervos
el mundo de sofia
de animales a dioses
arkhan asylum
the sandman
```

Some: Devuelve true si se cumple la condición:
```js
var libros = [
  { nombre: "la joven de las naranjas", costo: 245 },
  { nombre: "el problema de los 3 cuerpos", costo: 459 },
  { nombre: "festin de cuervos", costo: 200 },
  { nombre: "el mundo de sofia", costo: 420 },
  { nombre: "de animales a dioses", costo: 450 },
  { nombre: "arkhan asylum", costo: 350 },
  { nombre: "the sandman", costo: 1700 },
];

var libros_baratos = libros.some(item => {
    return item.costo <= 700;
});

console.log(libros_baratos);
```

```
true
```

```js
```

```
```
