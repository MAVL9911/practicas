+++Add commentMore actions
date = '2025-02-21T10:19:37-08:00'
draft = false
title = 'Practica1'
+++

# Elementos Fundamentales de los Lenguajes de Programación en Python

Este documento describe los elementos clave que forman parte de los lenguajes de programación, ilustrados con ejemplos en **Python**.

## 1. Nombres (Identifiers)

Los **nombres** son etiquetas simbólicas que usamos para referirnos a variables, funciones, clases, etc.

```python
nombre = "Juan"
edad = 25
```

## 2. Marcos de Activación (Activation Records / Call Stack)

Los **marcos de activación** almacenan información de cada llamada a una función, incluyendo variables locales y el punto de retorno. Python maneja esto automáticamente usando la **pila de llamadas** (*call stack*).

```python
def saludar():
    mensaje = "Hola"
    print(mensaje)

saludar()
```

Cada vez que se llama a `saludar`, se crea un nuevo marco de activación.

## 3. Bloques de Alcance (Scope)

El **alcance** define dónde una variable es accesible. Python tiene alcance local, no local, global y built-in.

```python
x = 10  # Variable global

def funcion():
    x = 5  # Variable local
    print(x)

funcion()  # Imprime 5
print(x)   # Imprime 10
```

## 4. Administración de Memoria

Python maneja la **memoria automáticamente** con un recolector de basura. Las variables se almacenan en el heap, y las referencias se cuentan para liberar memoria cuando ya no se usan.

```python
a = [1, 2, 3]
b = a  # Ambas variables apuntan al mismo objeto en memoria
```

## 5. Expresiones

Una **expresión** es una combinación de valores, variables y operadores que se evalúan a un resultado.

```python
resultado = (3 + 5) * 2
```

## 6. Comandos (Statements)

Los **comandos** realizan acciones como asignar valores, llamar funciones o controlar el flujo del programa.

```python
print("Hola mundo")
```

## 7. Control de Secuencia

### a) Selección (Condicionales)

Permite ejecutar código dependiendo de una condición.

```python
if edad >= 18:
    print("Eres mayor de edad")
else:
    print("Eres menor de edad")
```

### b) Iteración (Bucles)

Ejecuta un bloque de código repetidamente.

```python
for i in range(5):
    print(i)

while condicion:
    hacer_algo()
```

### c) Recursión

Una función que se llama a sí misma para resolver un problema.

```python
def factorial(n):
    if n == 0:
        return 1
    return n * factorial(n - 1)
```

## 8. Subprogramas (Funciones)

Permiten encapsular lógica reutilizable.

```python
def sumar(a, b):
    return a + b
```

## 9. Tipos de Datos

Python tiene tipos de datos **primitivos** y **estructurados**.

- Primitivos: `int`, `float`, `str`, `bool`
- Estructurados: `list`, `tuple`, `dict`, `set`

```python
numero = 42
texto = "Python"
lista = [1, 2, 3]
diccionario = {"clave": "valor"}
```

---

> Python facilita el aprendizaje de estos conceptos gracias a su sintaxis clara y su enfoque en la legibilidad.

