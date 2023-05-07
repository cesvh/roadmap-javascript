# **Arreglos**

---

### **push:**
```js
```

```
```

---

### **pop:**
```js
```

```
```

---

### **shift:**
```js
```

```
```

---

### **unshift:**
```js
```

```
```

---

### **indexOf:**
```js
```

```
```

---

### **slice:**
```js
```

```
```

---

### **Ejercicios:**
```js
function libros(libros, eliminarLibros, nuevosLibros) {
    while (eliminarLibros > 0) {
        libros.pop();
        eliminarLibros--;
    }
    libros.push(nuevosLibros);
    return libros;
}

libros(["aaa", "bbb", "ccc"], 0, "ddd");
```

```
(4) ['aaa', 'bbb', 'ccc', 'ddd']
```

```js
function libros(libros, eliminarLibros, nuevosLibros) {
    while (eliminarLibros > 0) {
        libros.pop();
        eliminarLibros--;
    }
    libros.push(nuevosLibros);
    return libros;
}

libros(["aaa", "bbb", "ccc"], 1, "ddd");
```

```
(3) ['aaa', 'bbb', 'ddd']
```

```js
function libros(libros, eliminarLibros, nuevosLibros) {
    while (eliminarLibros > 0) {
        libros.pop();
        eliminarLibros--;
    }
    libros.push(nuevosLibros);
    return libros;
}

libros(["aaa", "bbb", "ccc"], 2, "ddd");
```

```
(2) ['aaa', 'ddd']
```

```js
function libros(libros, eliminarLibros, nuevosLibros) {
    while (eliminarLibros > 0) {
        libros.pop();
        eliminarLibros--;
    }
    libros.push(nuevosLibros);
    return libros;
}

libros(["aaa", "bbb", "ccc"], 3, "ddd");
```

```
['ddd']
```

---

```js
let my_election = "sci-fi";
let options = ["sci-fi", "filosofía", "astronomía", "matemáticas"];
let authours = ["cixin liu", "jostein garder", "neil degresse tyson", "baldor"];

let my_authour = authours[options.indexOf(my_election)];

console.log(`Mi autor favorito es: ${my_authour}`);
```

```
Mi autor favorito es: cixin liu
```
