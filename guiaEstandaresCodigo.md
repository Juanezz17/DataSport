# Guía de Estándares de Código - DataSport (Stack MERN)

Este documento define las reglas de estilo y buenas prácticas para mantener un código limpio, consistente y fácil de mantener en el proyecto DataSport, usando exclusivamente JavaScript con el stack MERN.

---

## 1. Reglas de nombres

### Variables
- Usar *camelCase* para variables y funciones.  
  Ejemplo: totalPuntos, obtenerEstadisticas()
- Constantes en *mayúsculas con guiones bajos*.  
  Ejemplo: MAX_INTENTOS
- Evitar abreviaciones ambiguas o poco descriptivas.

### Clases
- Usar *PascalCase* para nombres de clases.  
  Ejemplo: UsuarioAdministrador, PartidoEstadistica
- Nombres descriptivos, en singular.

### Métodos / Funciones
- Usar verbos en infinitivo o imperativo.  
  Ejemplo: calcularPromedio(), actualizarPerfil()

---

## 2. Comentarios y documentación interna

- Explicar el *por qué* del código, no el *qué* (el código debe ser claro).
- Usar *JSDoc* para funciones y métodos.
- Comentar en español, coherente con el equipo.
- Mantener los comentarios cortos y claros.

Ejemplo JSDoc:
```js
/**
 * Obtiene las estadísticas en tiempo real de un partido.
 * @param {string} idPartido - Identificador único del partido.
 * @returns {Object} Estadísticas actuales del partido.
 */
function obtenerEstadisticas(idPartido) {
  // código
}

---

## 3. Identación y estilo de código

- Identación de *2 espacios*.
- Líneas no mayores a *100 caracteres*.
- Llaves {} en la misma línea que la declaración.
- Uso consistente de *comillas simples* para strings ('hola').
- Poner punto y coma al final de cada instrucción.
- Evitar líneas en blanco excesivas.
- Separar bloques de código con una línea en blanco.

---

## 4. Ejemplos aceptados y no aceptados

### Variables
```js
// Aceptado
const maxIntentos = 3;

// No aceptado
const Max_intentos = 3;

// Aceptado
function obtenerEstadisticas() {
  // código
}

// No aceptado
function getstats() {
  // código
}

// Aceptado
// Verificamos que el usuario esté autenticado antes de continuar.

// No aceptado
// Código que verifica la autenticación.