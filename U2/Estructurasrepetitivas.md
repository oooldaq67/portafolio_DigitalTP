# Estructuras condicionales

Una **estructura condicional** permite que un programa tome decisiones: ejecuta ciertas instrucciones solo si se cumple una condición determinada.

---

## 1. Condicional simple (Si–Entonces)

Ejecuta un bloque de instrucciones **únicamente si** la condición es verdadera. Si es falsa, no hace nada y continúa.

### *Pseudocódigo*

```
Si <condición> Entonces
    <acción>
Fin_Si
```

### *Ejemplo*

```
Si edad >= 18 Entonces
    Escribir "Eres mayor de edad"
Fin_Si
```

### *Código en C*

```c
if (edad >= 18) {
    printf("Eres mayor de edad\n");
}
```

---

## 2. Condicional doble (Si–Entonces–Sino)

Ofrece **dos caminos alternativos**: uno cuando la condición es verdadera y otro cuando es falsa.

### *Pseudocódigo*

```
Si <condición> Entonces
    <acción A>
Sino
    <acción B>
Fin_Si
```

### *Ejemplo*

```
Si nota >= 10 Entonces
    Escribir "Aprobado"
Sino
    Escribir "Reprobado"
Fin_Si
```

### *Código en C*

```c
if (nota >= 10) {
    printf("Aprobado\n");
} else {
    printf("Reprobado\n");
}
```

---

## 3. Condicional anidado (Si–Sino Si)

Se usan cuando hay **más de dos condiciones en cadena**, donde cada alternativa puede contener a su vez otro condicional.

### *Pseudocódigo*

```
Si <condición 1> Entonces
    <acción 1>
Sino Si <condición 2> Entonces
    <acción 2>
Sino Si <condición 3> Entonces
    <acción 3>
Sino
    <acción por defecto>
Fin_Si
```

### *Ejemplo*

```
Si nota >= 18 Entonces
    Escribir "Excelente"
Sino Si nota >= 14 Entonces
    Escribir "Bueno"
Sino Si nota >= 10 Entonces
    Escribir "Regular"
Sino
    Escribir "Reprobado"
Fin_Si
```

### *Código en C*

```c
if (nota >= 18) {
    printf("Excelente\n");
} else if (nota >= 14) {
    printf("Bueno\n");
} else if (nota >= 10) {
    printf("Regular\n");
} else {
    printf("Reprobado\n");
}
```

---

## 4. Condicional múltiple (Según–Sea / Switch–Case)

Evalúa una **variable o expresión** y ejecuta el bloque correspondiente al valor que coincida. Es más limpio que varios Si–Sino Si cuando se compara la misma variable con múltiples valores concretos.

### *Pseudocódigo*

```
Según <variable> Hacer
    Caso <valor 1>: <acción 1>
    Caso <valor 2>: <acción 2>
    Caso <valor 3>: <acción 3>
    De_otro_modo: <acción por defecto>
Fin_Según
```

### *Ejemplo*

```
Según dia Hacer
    Caso 1: Escribir "Lunes"
    Caso 2: Escribir "Martes"
    Caso 3: Escribir "Miércoles"
    De_otro_modo: Escribir "Otro día"
Fin_Según
```

### *Código en C*

```c
switch (dia) {
    case 1:
        printf("Lunes\n");
        break;
    case 2:
        printf("Martes\n");
        break;
    case 3:
        printf("Miércoles\n");
        break;
    default:
        printf("Otro día\n");
}
```

---

