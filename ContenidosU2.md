
<p align="center">
  <img src="https://unl.edu.ec/sites/default/files/logogris%20copia.png" width="280" alt="Logo UNL"/>
</p>

# *Unidad 2*:

---

## 📂 *Topics:*
 
---

### 1. [📖 *Estructuras Condicionales*](U2/Estructurascondicionales.md)

---

### 2. [📖 *Estructuras Repetitivas*](U2/Estructurasrepetitivas.md)

---

### 3. [🧠 *Ejercicio Aplicado*](U2/Ejercicioaplicado.md)


---

<details>
<summary><b> 4. 🔍 Reflexión Personal </b></summary>
<br>

### Dificultades encontradas

- **Confundir `=` con `==`:** Asignar un valor dentro de una condición en lugar de
  compararlo es un error lógico frecuente que no siempre genera un mensaje de error,
  pero altera el comportamiento del programa de forma silenciosa.

- **Bucles infinitos:** Olvidar actualizar la variable de control en un `while`
  produce una ejecución que nunca termina. Identificar la **condición de parada**
  antes de escribir el bucle es una práctica esencial.

- **Orden en cadenas `else if`:** Las condiciones se evalúan en secuencia; una
  condición mal ordenada puede hacer que ciertos casos nunca sean alcanzados
  (*código muerto*).

- **`do / while` vs `while`:** Determinar cuándo es necesario garantizar al menos
  una ejecución requiere analizar con cuidado las precondiciones del problema.

### Reflexión crítica

Estudiar estas estructuras desde la perspectiva de la lógica proposicional cambia
la forma de escribirlas. Una condición compuesta como `!(a && b)` no es solo
sintaxis: es la Ley de De Morgan, equivalente a `!a || !b`. Reconocer esa
equivalencia permite simplificar expresiones y reducir errores.

Del mismo modo, un bucle no es simplemente "repetir algo": es una proposición que
debe ser verdadera al inicio, mantenerse como **invariante** en cada iteración y
volverse falsa en un punto definido. Pensar así convierte el diseño de bucles en
un ejercicio de razonamiento formal, no de prueba y error.

</details>

---

### [*🔙 Volver al Índice*](index.md)


<div align="center">
  <sub>Pablo Namicela &nbsp;·&nbsp; Teoria de la Programación &nbsp;·&nbsp; Universidad Nacional de Loja &nbsp;·&nbsp; 2026</sub>
</div>

---

<div align="center">
  <sub>Facultad de la Energía, las Industrias y los Recursos Naturales No Renovables &nbsp;·&nbsp; Loja, Ecuador &nbsp;·&nbsp; 2026</sub>
</div>
