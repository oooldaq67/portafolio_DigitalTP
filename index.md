
<img width="324" height="442" alt="image" src= https://inscripciones.unl.edu.ec/images/logo_unl.png />


# PORTAFOLIO DIGITAL DE APRENDIZAJE – TEORÍA DE LA PROGRAMACIÓN.

---

## CARÁTULA

| | |
|---|---|
| **Institución** | Universidad Nacional de Loja |
| **Carrera** | Ingeniería en Ciencias de la Computación |
| **Asignatura** | Programación en C++ |
| **Ciclo y Paralelo** | 1er Ciclo — Paralelo A |
| **Período Académico** | Abril — Agosto 2026 |
| **Docente** | Ing. Lissette Geoconda López Faicán |
| **Estudiante** | Pablo Isaías Namicela Maldonado |

---

## UNIDAD 1

### Contenidos

#### Algoritmo

Un algoritmo es un conjunto ordenado y finito de pasos o instrucciones que permiten resolver un problema o realizar una tarea específica. Sus características principales son: ser preciso, finito y definido.

**Ejemplo:** Para sumar dos números: recibir el primer número, recibir el segundo número, sumar ambos y mostrar el resultado.

---

#### Pseudocódigo

El pseudocódigo es una representación informal de un algoritmo usando lenguaje natural combinado con estructuras de programación. No sigue la sintaxis de ningún lenguaje específico, por lo que es independiente del lenguaje de programación.

**Ejemplo:**
```
INICIO
  LEER a, b
  suma ← a + b
  ESCRIBIR suma
FIN
```

---

#### Diagrama de Flujo

Un diagrama de flujo es una representación gráfica de un algoritmo mediante símbolos estandarizados que muestran la secuencia lógica de los pasos a seguir para resolver un problema.

**Símbolos principales:**

| Símbolo | Descripción |
|---------|-------------|
| Óvalo | Inicio / Fin |
| Paralelogramo | Entrada / Salida de datos |
| Rectángulo | Proceso o cálculo |
| Rombo | Decisión (condición) |
| Flecha | Flujo de dirección |

---

#### Prueba de Escritorio

La prueba de escritorio es una técnica de validación manual que consiste en ejecutar el algoritmo paso a paso en papel, asignando valores a las variables para verificar que el resultado obtenido sea el esperado. Permite detectar errores lógicos antes de codificar.

---

#### Lenguajes de Programación

Un lenguaje de programación es un conjunto de reglas sintácticas y semánticas que permiten escribir instrucciones que una computadora puede interpretar o compilar para ejecutarlas. Se clasifican en:

- **Bajo nivel:** Lenguaje máquina y ensamblador. Cercanos al hardware.
- **Alto nivel:** C++, Python, Java. Más cercanos al lenguaje humano.
- **Interpretados:** Python, JavaScript. Se ejecutan línea a línea.
- **Compilados:** C, C++. Se traducen completamente antes de ejecutarse.

---

#### Programación por Bloques

La programación por bloques es una metodología visual de aprendizaje de programación donde las instrucciones se representan como bloques que se ensamblan entre sí, similar a un rompecabezas. Herramientas como Scratch utilizan este paradigma para introducir conceptos fundamentales de programación sin necesidad de escribir código.

Sus ventajas son: facilita la comprensión de estructuras de control, elimina errores de sintaxis y permite enfocarse en la lógica del problema.

---

### Ejercicio con Estructura Secuencial

#### Planteamiento del Problema

En una concesionaria de vehículos se realizaron tres ventas de vehículos de alta gama a 3 clientes. Cada vehículo cuesta 30.000, 29.000 y 33.000 USD respectivamente. El gerente desea saber cuál es el porcentaje de comisión (4%) que cada vendedor se llevará, y lo que le pagará en conjunto (total) a los tres vendedores.

---

#### Análisis del Problema

**Datos de entrada:**
- Precio vehículo 1: $30.000
- Precio vehículo 2: $29.000
- Precio vehículo 3: $33.000
- Porcentaje de comisión: 4% por vendedor

**Proceso:**
- Comisión de cada vendedor = precio del vehículo × 0.04
- Total = comisión1 + comisión2 + comisión3

**Datos de salida:**
- Comisión individual de cada vendedor
- Total a pagar en conjunto

---

#### Diseño del Algoritmo

**Diagrama de Flujo:**

```
        [INICIO]
           |
           ▼
  [v1=30000, v2=29000, v3=33000, comision=0.04]
           |
           ▼
  [c1 = v1 × comision]
  [c2 = v2 × comision]
  [c3 = v3 × comision]
           |
           ▼
  [total = c1 + c2 + c3]
           |
           ▼
  [MOSTRAR c1, c2, c3, total]
           |
           ▼
         [FIN]
```

**Pseudocódigo:**

```
INICIO
  v1 ← 30000
  v2 ← 29000
  v3 ← 33000
  comision ← 0.04

  c1 ← v1 * comision
  c2 ← v2 * comision
  c3 ← v3 * comision

  total ← c1 + c2 + c3

  ESCRIBIR "Comisión vendedor 1: $", c1
  ESCRIBIR "Comisión vendedor 2: $", c2
  ESCRIBIR "Comisión vendedor 3: $", c3
  ESCRIBIR "Total a pagar: $", total
FIN
```

---

#### Codificación (Código Fuente en C++)

```cpp
#include <iostream>
using namespace std;

int main() {
    // Precios de los vehículos
    double vehiculo1 = 30000;
    double vehiculo2 = 29000;
    double vehiculo3 = 33000;

    double comision = 0.04; // 4% por vendedor

    // Comisión individual por cada vendedor
    double comision1 = vehiculo1 * comision;
    double comision2 = vehiculo2 * comision;
    double comision3 = vehiculo3 * comision;

    // Total a pagar en conjunto
    double total = comision1 + comision2 + comision3;

    cout << "=== CONCESIONARIA DE VEHICULOS ===" << endl;
    cout << "Comision vendedor 1 (vehiculo $30000): $" << comision1 << endl;
    cout << "Comision vendedor 2 (vehiculo $29000): $" << comision2 << endl;
    cout << "Comision vendedor 3 (vehiculo $33000): $" << comision3 << endl;
    cout << "Total pagado en conjunto:              $" << total    << endl;

    return 0;
}
```

---

#### Validación — Prueba de Escritorio

| Paso | Variable | Operación | Resultado |
|------|----------|-----------|-----------|
| 1 | vehiculo1 | = 30000 | 30000 |
| 2 | vehiculo2 | = 29000 | 29000 |
| 3 | vehiculo3 | = 33000 | 33000 |
| 4 | comision | = 0.04 | 0.04 |
| 5 | comision1 | 30000 × 0.04 | **1200.00** |
| 6 | comision2 | 29000 × 0.04 | **1160.00** |
| 7 | comision3 | 33000 × 0.04 | **1320.00** |
| 8 | total | 1200 + 1160 + 1320 | **3680.00** |

**Salida esperada en consola:**
```
=== CONCESIONARIA DE VEHICULOS ===
Comision vendedor 1 (vehiculo $30000): $1200
Comision vendedor 2 (vehiculo $29000): $1160
Comision vendedor 3 (vehiculo $33000): $1320
Total pagado en conjunto:              $3680
```

✅ El programa produce los resultados esperados. La prueba de escritorio es correcta.

---

### Principales Dificultades y Reflexión Crítica

Durante el desarrollo de los contenidos de la Unidad 1 se identificaron las siguientes dificultades:

**Dificultades encontradas:**

- Comprender la diferencia entre pseudocódigo y código fuente real, ya que el pseudocódigo no tiene una sintaxis única y puede variar según el criterio del programador.
- Identificar correctamente el tipo de dato a usar en C++ (int vs double) cuando se trabaja con valores monetarios que pueden tener decimales.
- Traducir el diagrama de flujo directamente a código sin omitir pasos del proceso.

**Reflexión crítica:**

El aprendizaje de la estructura secuencial es fundamental porque constituye la base de cualquier programa. Comprender que un computador ejecuta instrucciones de forma lineal, una por una, ayuda a desarrollar el pensamiento lógico necesario para resolver problemas más complejos. El uso del pseudocódigo y el diagrama de flujo antes de codificar permitió detectar posibles errores en la lógica antes de enfrentarse al compilador, lo cual redujo significativamente el tiempo de depuración del código.

---

## UNIDAD 2

> **No aplica para este período.**

---

## UNIDAD 3

> **No aplica para este período.**

---

## CONCLUSIONES GENERALES

> **No aplica para este período.**

---

## BIBLIOGRAFÍA

> Formato IEEE:

[1] B. Stroustrup, *The C++ Programming Language*, 4th ed. Upper Saddle River, NJ: Addison-Wesley, 2013.

[2] H. Schildt, *C++: The Complete Reference*, 4th ed. New York, NY: McGraw-Hill/Osborne, 2003.

[3] P. Deitel y H. Deitel, *C++ How to Program*, 10th ed. Upper Saddle River, NJ: Pearson, 2017.

[4] R. Sedgewick y K. Wayne, *Algorithms*, 4th ed. Upper Saddle River, NJ: Addison-Wesley, 2011.

---

## DECLARACIÓN DE USO DE INTELIGENCIA ARTIFICIAL GENERATIVA

Yo, **Pablo Isaías Namicela Maldonado**, estudiante de la carrera de Ingeniería en Ciencias de la Computación de la Universidad Nacional de Loja, declaro que durante la elaboración del presente portafolio hice uso de herramientas de Inteligencia Artificial Generativa (Claude — Anthropic) como apoyo en las siguientes actividades:

- Explicación y comprensión de conceptos teóricos de la unidad.
- Revisión y corrección de la lógica del pseudocódigo y código fuente.
- Orientación en la estructura y organización del portafolio.

Declaro que el análisis, la comprensión de los contenidos y el desarrollo del ejercicio propuesto son de mi autoría, y que el uso de la IA fue exclusivamente como herramienta de apoyo al aprendizaje, no como sustituto del mismo.

**Firma:** ___________________________

**Fecha:** ___________________________, 2026

---

*Universidad Nacional de Loja — Período Académico Abril — Agosto 2026*
