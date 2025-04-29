<h1 align="center">
  <strong>Domina TypeScript desde sus Bases hasta Conceptos Avanzados</strong>
</h1>

<img src="./Imagenes/typescript banner.png" alt="Banner de Conceptos de TypeScript" width="100%" />

<p align="center">
  Una guía completa y práctica para entender y aplicar los conceptos fundamentales de <strong>TypeScript</strong> 🚀🧠
</p>

<p align="center">
  <img src="https://img.shields.io/badge/TypeScript-Latest-blue?style=for-the-badge&logo=typescript&logoColor=white&labelColor=101010" alt="TypeScript Badge" />
  <img src="https://img.shields.io/badge/Estado-En%20progreso-blue?style=for-the-badge&logo=github&logoColor=white&labelColor=101010" alt="Estado: En progreso" />
  <img src="https://img.shields.io/github/last-commit/jcbalbdev/conceptos-typescript?style=for-the-badge&logo=git&logoColor=white&labelColor=101010" alt="Último commit" />
</p>

---

<img src="https://media.giphy.com/media/WcYnTzdrjQphdu33xs/giphy.gif" alt="Aprende TypeScript" width="100" />

> ##### Si te resulta útil esta recopilación de conceptos, ¡apóyalo haciendo "★ Star" en el repositorio! 🌟

---

## 🗺️ Índice

- [📖 ¿Qué es este proyecto?](#-qué-es-este-proyecto)
- [🧠 TYPESCRIPT](#-typescript)
  - [🧠 ¿Qué es TypeScript?](#-qué-es-typescript)
  - [🔥 ¿Por qué es importante TypeScript?](#-por-qué-es-importante-typescript)
  - [🛠️ Explicación detallada paso a paso](#️-explicación-detallada-paso-a-paso)
  - [✏️ Ejemplo práctico](#️-ejemplo-práctico)
  - [🌎 Analogía con el mundo real](#-analogía-con-el-mundo-real)
  - [⚡ Errores comunes al aprender o aplicar este concepto](#-errores-comunes-al-aprender-o-aplicar-este-concepto)
  - [💡 Consejo práctico para dominar el tema](#-consejo-práctico-para-dominar-el-tema)
- [🧠 Tema 2: Variables y tipos de datos básicos](#-tema-2-variables-y-tipos-de-datos-básicos)
  - [🧠 ¿Que son variables y tipos?](#-que-son-variables-y-tipos)
  - [🔥 ¿Por qué es importante TypeScript?](#-por-qué-es-importante-typescript-1)
  - [🛠️ Explicación detallada paso a paso](#️-explicación-detallada-paso-a-paso-1)

---

# 📖 ¿Qué es este proyecto?

Este repositorio reúne los **conceptos esenciales, intermedios y avanzados de TypeScript**, explicados de manera clara y acompañados de ejemplos prácticos.

- 🎯 Ideal para quien empieza a aprender TypeScript o quiere reforzar su comprensión.
- 📈 Avanza de forma ordenada: desde lo más básico hasta técnicas profesionales.

---
# 🧠 TYPESCRIPT
## 🧠 ¿Qué es TypeScript?
TypeScript es un lenguaje de programación que mejora a JavaScript agregándole reglas para que puedas detectar errores antes de que tu programa se ejecute.
En una frase:
> TypeScript es JavaScript, pero con “superpoderes” para encontrar errores antes de que sea demasiado tarde.
## 🔥 ¿Por qué es importante TypeScript?
Porque nos ayuda a evitar errores que en JavaScript recién veríamos cuando la aplicación ya esté corriendo (¡y eso puede causar fallos o problemas para los usuarios!).
Además, hace que los programas sean más fáciles de entender y mantener a medida que crecen.
## 🛠️ Explicación detallada paso a paso
Vamos paso a paso:
1. JavaScript es flexible, pero peligroso
   JavaScript te deja hacer muchas cosas, pero no te avisa si cometes errores como usar mal un dato (por ejemplo, tratar un número como si fuera un texto). Eso puede causar fallas durante la ejecución.
2. TypeScript agrega "tipos"
   TypeScript te permite decirle al programa qué tipo de datos esperas: ¿es un número? ¿es un texto? ¿es una lista?. Si escribes algo que no concuerda, TypeScript te avisa antes de que el programa corra.
3. TypeScript se convierte en JavaScript
   Las computadoras, los navegadores y los servidores no entienden TypeScript directamente.TypeScript se transforma (compila) en JavaScript normal antes de que se use.
4. ¿Cómo lo usa un programador?
   Escribes tu programa en archivos .ts (TypeScript). Luego, lo “conviertes” en archivos .js (JavaScript) usando una herramienta llamada compilador.
## ✏️ Ejemplo práctico
Supongamos que estamos sumando dos números:

En JavaScript:
```javascript
function suma(a, b) {
  return a + b;
}
```

¿Problema?
Nada te impide hacer esto:
```javascript
suma(5, "hola")  // Resultado: "5hola" (concatena en vez de sumar)
```
💥 ¡Error raro! El programa no falla, pero no hace lo que quieres.

En TypeScript:
```typescript
function suma(a: number, b: number): number {
  return a + b;
}
```
Aquí TypeScript te exige que a y b sean números (number).
Si tratas de hacer suma(5, "hola"), TypeScript te marca un error inmediatamente ❌.

## 🌎 Analogía con el mundo real
Piensa en un aeropuerto:

- JavaScript sería como dejar que cada pasajero aborde cualquier avión sin verificar su boleto.
(¡Algunos terminan en destinos equivocados!)

- TypeScript sería como verificar que cada pasajero tiene el boleto correcto antes de subir al avión.
(¡Todos van a donde deben ir, sin sorpresas!)

Así, TypeScript verifica tu código antes de que lo “pongas en marcha”, igual que un aeropuerto verifica boletos antes de volar.

## ⚡ Errores comunes al aprender o aplicar este concepto
- Pensar que TypeScript reemplaza JavaScript.
  No, TypeScript es una herramienta extra, pero el producto final siempre es JavaScript.

- Olvidar compilar.
  Tienes que convertir (compilar) tu código .ts en .js, ¡si no, tu programa no correrá!

- Poner tipos innecesarios.
  A veces TypeScript puede adivinar tipos solo. Si pones demasiados tipos manualmente, tu código se vuelve más largo y feo.

## 💡 Consejo práctico para dominar el tema
> *Haz pequeños programas en TypeScript y mira cómo detecta los errores.*
> 
> **Intenta provocar errores a propósito** para ver cómo TypeScript te los señala.
> 
> Eso te va a enseñar a **confiar** en sus advertencias y a escribir código **más seguro y limpio**.

# 🧠 Tema 2: Variables y tipos de datos básicos
## 🧠 ¿Que son variables y tipos?
- Variables son cajas donde guardamos información.

- Tipos de datos básicos son formas que puede tener esa información: puede ser un número, un texto, verdadero o falso, entre otros.
En una frase:
> Una variable es como una cajita que guarda algo, y el tipo de dato nos dice qué clase de cosa guarda.
## 🔥 ¿Por qué es importante TypeScript?
Porque en TypeScript no basta con guardar cualquier cosa en cualquier variable:
Debemos ser claros sobre qué tipo de datos vamos a guardar.
Así, el lenguaje puede avisarnos si cometemos errores (por ejemplo, guardar un número donde debería ir un texto).
Esto ayuda a que nuestro programa sea más confiable y más fácil de entender.
## 🛠️ Explicación detallada paso a paso
Vamos paso a paso:
1. ¿Qué es una variable?
    - Una variable es un nombre que le damos a un espacio en la memoria del computador para guardar un valor.

    En TypeScript usamos tres palabras clave para crear variables:
    - let → Para variables que pueden cambiar su valor.
    - const → Para variables que no deben cambiar su valor.
    - var → (se usaba antes, ya no se recomienda).
    En TypeScript:
    ```typescript
    let edad = 25;
    const nombre = "Diana";
    ```
    - edad es una variable que puede cambiar (por eso usamos let).
    - nombre no debe cambiar (por eso usamos const).
2. ¿Qué es un tipo de dato?
   - Un tipo de dato describe qué clase de información guarda una variable.
    En TypeScript, los tipos básicos son:
    | Tipo de dato | Qué representa                | Ejemplo           |
    | ------------ | ----------------------------- | ----------------- |
    | `number`     | Números (enteros o decimales) | `42`, `3.14`      |
    | `string`     | Textos o palabras             | `"Hola"`, `"123"` |
    | `boolean`    | Verdadero o falso             | `true`, `false`   |

    Cómo se usan:
    ```typescript
    let edad = 25;
    const nombre = "Diana";
    ```


