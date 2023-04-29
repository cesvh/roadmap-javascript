# **Objetos**

```js
var my_book = {
    name: "El problema de los 3 cuerpos",
    author: "cixin liu",
    format: "físico",
    genre: "science-fiction",
    detail: function() {
        console.log(`Libro: ${this.name}, autor: ${this.author}.`);
    }
};

my_book;
```

```
{name: 'El problema de los 3 cuerpos', author: 'cixin liu', format: 'físico', genre: 'science-fiction', detail: ƒ}
```

```js

var my_book = {
    name: "El problema de los 3 cuerpos",
    author: "cixin liu",
    format: "físico",
    genre: "science-fiction",
    detail: function() {
        console.log(`Libro: ${this.name}, autor: ${this.author}.`);
    }
};

my_book.name
```

```
'El problema de los 3 cuerpos'
```

```js
var my_book = {
    name: "El problema de los 3 cuerpos",
    author: "cixin liu",
    format: "físico",
    genre: "science-fiction",
    detail: function() {
        console.log(`Libro: ${this.name}, autor: ${this.author}.`);
    }
};

my_book["name"]
```

```
'El problema de los 3 cuerpos'
```

```js
var my_book = {
    name: "El problema de los 3 cuerpos",
    author: "cixin liu",
    format: "físico",
    genre: "science-fiction",
    detail: function() {
        console.log(`Libro: ${this.name}, autor: ${this.author}.`);
    }
};

my_book.name = "El problema de los tres cuerpos";
```

```
'El problema de los tres cuerpos'
```

```js
var my_book = {
    name: "El problema de los 3 cuerpos",
    author: "cixin liu",
    format: "físico",
    genre: "science-fiction",
    detail: function() {
        console.log(`Libro: ${this.name}, autor: ${this.author}.`);
    }
};

my_book.detail;
```

```
ƒ () {
        console.log(`Libro: ${this.name}, autor: ${this.author}.`);
    }
```

```js
var my_book = {
    name: "El problema de los 3 cuerpos",
    author: "cixin liu",
    format: "físico",
    genre: "science-fiction",
    detail: function() {
        console.log(`Libro: ${this.name}, autor: ${this.author}.`);
    }
};

my_book.detail();
```

```
Libro: El problema de los tres cuerpos, autor: cixin liu.
```

```js
var my_book = {
    name: "El problema de los 3 cuerpos",
    author: "cixin liu",
    format: "físico",
    genre: "science-fiction",
    detail: function() {
        console.log(`Libro: ${this.name}, autor: ${this.author}.`);
    }
};

var my_name_property = "detail";
my_book.my_name_property;
```

```
undefined
```

```js
var my_book = {
    name: "El problema de los 3 cuerpos",
    author: "cixin liu",
    format: "físico",
    genre: "science-fiction",
    detail: function() {
        console.log(`Libro: ${this.name}, autor: ${this.author}.`);
    }
};

my_book[my_name_property]();
```

```
Libro: El problema de los tres cuerpos, autor: cixin liu.
```

```js
var my_book = {
    name: "El problema de los 3 cuerpos",
    author: "cixin liu",
    format: "físico",
    genre: "science-fiction",
    detail: function() {
        console.log(`Libro: ${this.name}, autor: ${this.author}.`);
    }
};

my_book.pages = 408;
my_book;
```

```
{name: 'El problema de los tres cuerpos', author: 'cixin liu', format: 'físico', genre: 'science-fiction', detail: ƒ, pages: 408}
```

```js
var my_book = {
    name: "El problema de los 3 cuerpos",
    author: "cixin liu",
    format: "físico",
    genre: "science-fiction",
    detail: function() {
        console.log(`Libro: ${this.name}, autor: ${this.author}.`);
    }
};

delete my_book.pages;
```

```
true
```

```js
var my_book = {
    name: "El problema de los 3 cuerpos",
    author: "cixin liu",
    format: "físico",
    genre: "science-fiction",
    detail: function() {
        console.log(`Libro: ${this.name}, autor: ${this.author}.`);
    }
};

my_book;
```

```
{name: 'El problema de los tres cuerpos', author: 'cixin liu', format: 'físico', genre: 'science-fiction', detail: ƒ}
```

---

### **Función constructor**
```js
class auto{
    constructor(marca, modelo, annio, id) {
        this.marca = marca;
        this.modelo = modelo;
        this.id = id;
    }
}

var my_auto = new auto("Jeep", "2028", 0);
my_auto;
```

```
auto {marca: 'Jeep', modelo: '2028', id: undefined}
```
