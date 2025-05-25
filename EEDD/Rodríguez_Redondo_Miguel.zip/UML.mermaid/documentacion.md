# Sudoku en Java - Proyecto de Consola

## 📌 Descripción General

Este proyecto consiste en una aplicación de consola desarrollada en **Java** que permite a los usuarios **jugar al Sudoku manualmente** o **resolver tableros automáticamente** mediante un algoritmo. Está diseñado con un enfoque modular, aplicando principios de **Programación Orientada a Objetos (POO)** y buenas prácticas de diseño.

La aplicación ofrece varios niveles de dificultad para los jugadores y permite también validar y resolver tableros ya definidos. Todo se gestiona desde una interfaz de texto sencilla, ideal para aprender estructuras de programación en Java.

---

## 🛠️ Tecnologías y Herramientas Utilizadas

- **Lenguaje:** Java 8 o superior
- **Entorno de desarrollo:** Eclipse IDE / Visual Studio Code
- **Sistema de control de versiones:** Git (opcional, con `.gitignore` incluido)
- **Sistema operativo:** Compatible con Windows, Linux o macOS (consola)
- **Formato de ejecución:** Consola / Terminal
- **Imágenes de diseño:** Incluidas en carpeta `/images` para referencia visual

---

## 📂 Estructura del Proyecto

sudoku/
├── ProgramaSudoku.java # Clase principal para modo JUGAR
├── ProgramaSudokuResolver.java # Clase principal para modo RESOLVER
├── MetodosParaJugar.java # Lógica del juego manual (entradas, validaciones)
├── ReglasTableroBase.java # Reglas básicas del Sudoku
├── ReglasTableroJugar.java # Reglas específicas del modo jugar
├── TableroSudokuBase.java # Representación base del tablero
├── TableroSudokuJugar.java # Tablero específico para modo jugar
├── ResolverSudoku.java # Algoritmo de resolución automática
├── CoordenadaIncorrecta.java # Excepción personalizada
├── NumeroNoValidoParaJugar.java # Excepción personalizada
├── DificultadIncorrecta.java # Excepción personalizada
├── images/ # Imágenes de niveles y ejemplos visuales
│ ├── muyFacil.png
│ ├── experto.png
│ ├── DFJugar.png
│ └── ...
├── .gitignore # Archivos y carpetas ignorados por Git
└── README.md # Documentación del proyecto

---

## 🎮 Modos de Funcionamiento

### 1. Modo Jugar (`ProgramaSudoku.java`)
- El usuario puede elegir la dificultad: muy fácil, fácil, medio o experto.
- El sistema genera un tablero incompleto.
- El usuario introduce coordenadas (fila, columna) y un número.
- Se validan las jugadas en tiempo real.
- Si hay errores en las coordenadas o en los valores, se lanzan excepciones.

### 2. Modo Resolver (`ProgramaSudokuResolver.java`)
- El usuario puede cargar o visualizar un tablero predefinido.
- El sistema lo resuelve automáticamente utilizando técnicas lógicas (algoritmo de backtracking).
- Se muestra el tablero resuelto por consola.

---

## 🧠 Principales Clases y Funcionalidades

| Clase                     | Función Principal |
|--------------------------|-------------------|
| `ProgramaSudoku`         | Punto de entrada para jugar |
| `ProgramaSudokuResolver` | Punto de entrada para resolver |
| `MetodosParaJugar`       | Contiene lógica interactiva de juego |
| `ReglasTableroBase`      | Valida reglas básicas del Sudoku |
| `ReglasTableroJugar`     | Valida reglas adicionales al jugar |
| `ResolverSudoku`         | Algoritmo para resolver tableros automáticamente |
| `TableroSudokuBase`      | Modelo genérico del tablero |
| `TableroSudokuJugar`     | Modelo específico del tablero en modo juego |
| `*.java (excepciones)`   | Controlan errores comunes en entrada de datos |

---

## ▶️ Cómo Ejecutar el Proyecto

### Opción 1: Desde Eclipse o VS Code
1. Clona o descarga el proyecto.
2. Importa la carpeta del proyecto como un proyecto Java.
3. Ejecuta `ProgramaSudoku.java` o `ProgramaSudokuResolver.java` como aplicación Java.
4. Sigue las instrucciones por consola.

### Opción 2: Desde la terminal
```bash
javac *.java
java ProgramaSudoku         # Para jugar
java ProgramaSudokuResolver # Para resolver
