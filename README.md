[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/aRQGnba4)
# Expresiones Regulares (regex)

## Investiga: 

- qué son las expresiones regulares?
son patrones que se utilizan para hacer coincidir combinaciones de caracteres en cadenas.
- Qué problema resuelven? Por qué es importante conocerlas?
Sirven para:
    - Validar una entrada: validar si una cadena de texto cumple con un formato especifico.
    - Busqueda de patrones: extraer información de un conjunto de datos o para realizar operaciones de búsqueda y reemplazo.
    - Extracción de datos: extraer partes especificas de una cadena de texto.
    - Reemplazo de texto: realizar operaciones de búsqueda y reemplazo. Puedes buscar un patrón específico y reemplazarlo por otro valor.
    - Validación de Formularios:  verificar si un campo de formulario cumple con ciertos criterios antes de enviar los datos al servidor.
    - Análisis de Logs: extraer información específica, como direcciones IP, fechas, nombres de archivos, etc.
    - Manipulación de Texto en General:  eliminar espacios en blanco, cambiar el formato de fechas, o realizar otras transformaciones complejas en cadenas de texto.
    - Tokenización: dividir el código fuente en tokens (componentes básicos del lenguaje de programación y representan elementos individuales como palabras clave, identificadores, operadores, constantes y símbolos)


## Ejercicio 1:

Escribe las expresiones regulares correctas para validar:

- un email
let email = [a-zA-Z0-9_]+([.][a-zA-Z0-9_]+)*@[a-zA-Z0-9_]+([.][a-zA-Z0-9_]+)*[.][a-zA-Z]{2,5}
email.test
- un número de teléfono (español)
let telefono = (\+34|0034|34)?[ -]*(6|7)[ -]*([0-9][ -]*){8}
- un DNI
let dni = 	[0-9] {8} [AZ] {1}

## Ejercicio 2:

Crea un formulario de contacto y utiliza el atributo `pattern` de los elementos `input` para validar los campos usando expresiones regulares. El formulario debe incluir: nombre, apellidos, dni, número de teléfono, email, dni y dirección.

Nota: puedes hacerlo añadiendo un archivo `index.html` en este repositorio.


## Referencias

- [Expresiones Regulares en Javascript](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular_expressions)
- [Online Regex Editor](https://regex101.com/)