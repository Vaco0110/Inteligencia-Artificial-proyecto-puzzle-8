# **Inteligencia-Artificial-proyecto-puzzle-8**
Proyecto de puzzle 8 hecho con python y el algoritmo A estrella 
Integrantes: 
Jesus Hector Roman Vizar
Jose Humberto Gutierrez Beltran


# **Puzzle 8 Solver**
Una aplicación interactiva que resuelve el clásico Puzzle 8 utilizando el algoritmo A* con heurística de distancia Manhattan. Desarrollada en Python con una interfaz gráfica moderna usando Tkinter.

## **Características**
Interfaz gráfica intuitiva: Diseño moderno y fácil de usar

Algoritmo eficiente: Implementación del algoritmo A* con heurística de distancia Manhattan

Modo interactivo: Permite jugar manualmente haciendo clic en las fichas

Solución automática: Resuelve el puzzle automáticamente mostrando cada paso

Contador de movimientos: Muestra el número de movimientos y estados explorados

Estado inicial predefinido: Configurado con un estado desafiante pero solucionable

## **Cómo ejecutar**
Prerrequisitos
Python 3.6 o superior

Tkinter (generalmente incluido en instalaciones estándar de Python)

Instalación y ejecución
Clona o descarga el repositorio

Navega al directorio del proyecto

Ejecuta el script:

bash
python puzzle8_solver.py

## **Cómo usar**

Usar la solución automática
Haz clic en el botón "Resolver" para encontrar la solución óptima

Usa el botón "Siguiente Paso" para avanzar paso a paso por la solución

El botón "Reiniciar" vuelve al estado inicial

## **Estructura del código**
El proyecto está organizado en tres clases principales:

1. EstadoPuzzle8
Representa un estado del tablero con funcionalidades para:

Calcular la heurística de distancia Manhattan

Generar movimientos válidos

Verificar si es el estado objetivo

Realizar movimientos y crear nuevos estados

2. SolucionadorPuzzle8
Implementa el algoritmo A* para:

Explorar estados posibles

Encontrar la solución óptima

Reconstruir el camino solución

3. InterfazPuzzle8
Maneja la interfaz gráfica con:

Representación visual del tablero

Botones de control

Actualización del estado del juego

Interacción con el usuario

## **Personalización**
Puedes modificar el estado inicial editando la variable tablero_fijo en el método __init__ de la clase InterfazPuzzle8:

python
self.tablero_fijo = [1, 2, 3, 4, 5, 6, 7, 0, 8]  # Ejemplo más fácil

## **Detalles técnicos**
Heurística: Distancia Manhattan

Algoritmo: A* (A-star)

Complejidad: O(b^d) donde b es el factor de ramificación y d es la profundidad de la solución

Estados posibles: 9! = 362,880 configuraciones diferentes

## **Estado objetivo**
El estado objetivo que debe alcanzarse es:

text
[1, 2, 3]
[4, 5, 6]
[7, 8, 0]

