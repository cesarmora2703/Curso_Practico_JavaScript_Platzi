# Curso_Practico_JavaScript_Platzi
Curso práctico de JavaScript de Platzi, repositorio de ejercicios
# Test de Java Script

### 1️⃣ Responde las siguientes preguntas en la sección de comentarios:

- ¿Qué es una variable y para qué sirve?
    - Una variable es un contenedor usado para almacenar un valor, este contenedor tiene asignada una posición de memoria y un tamaño que depende del tipo de dato.
- ¿Cuál es la diferencia entre declarar e inicializar una variable?
    - Una variable se declara indicando su tipo y su nombre pero no su valor.
    - Inicializar la variable impliva asignarle un valor que debbe almacenar.
- ¿Cuál es la diferencia entre sumar números y concatenar strings?
    - La operación suma ejecuta la operación matemática, concatenar strings consiste en unir dos cadenas de texto o unir un numero y una cadena de texto que se mostrarian como texto por pantalla.
- ¿Cuál operador me permite sumar o concatenar?
    - El operador + (dependiendo del contexto).

### 2️⃣ Determina el nombre y tipo de dato para almacenar en variables la siguiente información:

- Nombre : string
- Apellido: string
- Nombre de usuario en Platzi: string
- Edad: number
- Correo electrónico: string
- Mayor de edad: boolean
- Dinero ahorrado: number
- Deudas: number

### 3️⃣ Traduce a código JavaScript las variables del ejemplo anterior y deja tu código en los comentarios.

const Nombre;

const Apellido;

const Edad;

const correoElectronico;

let mayorDeEdad;

let ahorros;

left deudas;

### 4️⃣ Calcula e imprime las siguientes variables a partir de las variables del ejemplo anterior:

const Nombre = "Cesar";

const Apellido = “Mora”

let ahorros = 7000000;

let deudas = 1000000;

let dineroReal = ahorros - deudas;

console.log(”Nombre completo: ${Nombre} ${Apellido}” );

console.log(”Dinero real: ${dineroReal}”);

## Funciones

### 1️⃣ Responde las siguientes preguntas en la sección de comentarios:

- ¿Qué es una función?
    - Una función es un bloque de código que se puede llamar en cualquier momento y es capaz de realizar una tarea específica. Las funciones pueden recibir parámetros y devolver un resultado si es necesario.
- ¿Cuándo me sirve usar una función en mi código?
    - Las funciones son útiles en el código cuando se necesita realizar una tarea específica varias veces o se desea modularizar el código.
- ¿Cuál es la diferencia entre parámetros y argumentos de una función?
    - Los parámetros son los valores que se definen al crear una función y que reciben los valores que se le pasan a la función al llamarla. Los argumentos son los valores que se pasan a una función al llamarla.

### 2️⃣ Convierte el siguiente código en una función, pero, cambiando cuando sea necesario las variables constantes por parámetros y argumentos en una función:

```
const name = "Juan David";
const lastname = "Castro Gallego";
const completeName = name + lastname;
const nickname = "juandc";

console.log("Mi nombre es " + completeName + ", pero prefiero que me digas " + nickname + ".");

```

```
function printName(name, lastName, nickname) {
  const completeName = name + ' ' + lastName;
  console.log("Mi nombre es " + completeName + ", pero prefiero que me digas " + nickname + ".");
}

printName('Juan David', 'Castro Gallego', 'juandc');

```

## Condicionales

### 1️⃣ Responde las siguientes preguntas en la sección de comentarios:

- ¿Qué es un condicional?
    - Un condicional es una estructura de control que permite ejecutar diferentes bloques de código en función de si se cumple o no una condición.
- ¿Qué tipos de condicionales existen en JavaScript y cuáles son sus diferencias?
    - En JavaScript existen dos tipos de condicionales: if/else y switch. El if/else se utiliza para evaluar una condición y ejecutar un bloque de código si la condición es verdadera o un bloque diferente si es falsa. El switch se utiliza para evaluar una variable y ejecutar un bloque de código diferente en función del valor de la variable.
- ¿Puedo combinar funciones y condicionales?
    - Sí, se pueden combinar funciones y condicionales para crear estructuras de control más complejas.

### 2️⃣ Replica el comportamiento del siguiente código que usa la sentencia switch utilizando if, else y else if:

const tipoDeSuscripcion = "Basic";

**switch**(tipoDeSuscripcion) {

**case**"Free":
       console.log("Solo puedes tomar los cursos gratis");

**break**;

**case**"Basic":
       console.log("Puedes tomar casi todos los cursos de Platzi durante un mes");

**break**;

**case**"Expert":
       console.log("Puedes tomar casi todos los cursos de Platzi durante un año");

**break**;

**case**"ExpertPlus":
       console.log("Tú y alguien más pueden tomar TODOS los cursos de Platzi durante un año");

**break**;
}

```
const tipoDeSuscripcion = "Basic";

if (tipoDeSuscripcion === "Free") {
  console.log("Solo puedes tomar los cursos gratis");
} else if (tipoDeSuscripcion === "Basic") {
  console.log("Puedes tomar casi todos los cursos de Platzi durante un mes");
} else if (tipoDeSuscripcion === "Expert") {
  console.log("Puedes tomar casi todos los cursos de Platzi durante un año");
} else if (tipoDeSuscripcion === "ExpertPlus") {
  console.log("Tú y alguien más pueden tomar TODOS los cursos de Platzi durante un año");
}

```

### 3️⃣ Replica el comportamiento de tu condicional anterior con if, else y else if, pero ahora solo con if (sin else ni else if).

```
if (tipoDeSuscripcion === "Free") {
  console.log("Solo puedes tomar los cursos gratis");
}
if (tipoDeSuscripcion === "Basic") {
  console.log("Puedes tomar casi todos los cursos de Platzi durante un mes");
}
if (tipoDeSuscripcion === "Expert") {
  console.log("Puedes tomar casi todos los cursos de Platzi durante un año");
}
if (tipoDeSuscripcion === "ExpertPlus") {
  console.log("Tú y alguien más pueden tomar TODOS los cursos de Platzi durante un año");
}

```

## Ciclos

### 1️⃣ Responde las siguientes preguntas en la sección de comentarios:

- ¿Qué es un ciclo?
    - Un ciclo es una estructura de control que permite ejecutar un bloque de código varias veces.
- ¿Qué tipos de ciclos existen en JavaScript?
    - En JavaScript existen tres tipos de ciclos: for, while y do/while.
- ¿Qué es un ciclo infinito y por qué es un problema?
    - Un ciclo infinito es un ciclo que nunca termina de ejecutarse. Es un problema porque puede hacer que el programa se bloquee o se vuelva inestable.
- ¿Puedo mezclar ciclos y condicionales?
    - Sí, se pueden mezclar ciclos y condicionales para crear estructuras de control más complejas.

### 2️⃣ Replica el comportamiento de los siguientes ciclos for utilizando ciclos while:

**for**(let i = 0; i < 5; i++) {
    console.log("El valor de i es: " + i);
}

**for**(let i = 10; i >= 2; i--) {
    console.log("El valor de i es: " + i);
}

```
let i = 0;
while (i < 5) {
  console.log("El valor de i es: " + i);
  i++;
}

let j = 10;
while (j >= 2) {
  console.log("El valor de j es: " + j);
  j--;
}

```

### 3️⃣ Escribe un código en JavaScript que le pregunte a los usuarios cuánto es `2 + 2`. Si responden bien, mostramos un mensaje de felicitaciones, pero si responden mal, volvemos a empezar.

```
let respuesta = prompt('¿Cuánto es 2 + 2?');

while (respuesta !== '4') {
  respuesta = prompt('Incorrecto. ¿Cuánto es 2 + 2?');
}

console.log('¡Correcto!');

```

## Listas

### 1️⃣ Responde las siguientes preguntas en la sección de comentarios:

- ¿Qué es un array?
- Un array es una estructura de datos que permite almacenar una colección de elementos de diferentes tipos en una única variable.
- ¿Qué es un objeto?
- Un objeto es una estructura de datos que permite almacenar una colección de propiedades y sus valores asociados en una única variable utilizando clave valor.
- ¿Cuándo es mejor usar objetos o arrays?
    - Los arrays son mejores para almacenar colecciones de elementos del mismo tipo, mientras que los objetos son mejores para almacenar colecciones de propiedades y sus valores asociados.
- ¿Puedo mezclar arrays con objetos o incluso objetos con arrays?
    - Sí, se pueden mezclar arrays con objetos y objetos con arrays para crear estructuras de datos más complejas.

### 2️⃣ Crea una función que pueda recibir cualquier array como parámetro e imprima su primer elemento.

```
function printFirstElement(array) {
  console.log(array[0]);
}

const miArray = [1, 2, 3, 4, 5];
printFirstElement(miArray);

```

### 3️⃣ Crea una función que pueda recibir cualquier array como parámetro e imprima todos sus elementos uno por uno (no se vale imprimir el array completo).

```
function printAllElements(array) {
  for (let i = 0; i < array.length; i++) {
    console.log(array[i]);
  }
}

const miArray = [1, 2, 3, 4, 5];
printAllElements(miArray);

```

### 4️⃣ Crea una función que pueda recibir cualquier objeto como parámetro e imprima todos sus elementos uno por uno (no se vale imprimir el objeto completo).

```
function printAllProperties(objeto) {
  for (let propiedad in objeto) {
    console.log(propiedad + ": " + objeto[propiedad]);
  }
}

const miObjeto = {
  nombre: "César",
  edad: 30,
  ciudad: "México"
};

printAllProperties(miObjeto);
