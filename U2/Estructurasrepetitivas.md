
# Estructuras repetitivas

---

## *Ciclo Mientras (While)*

>Evalúa la condición **antes** de entrar al bloque. Si es falsa desde el inicio, el bloque nunca se ejecuta.

### *Pseudocódigo*

```
Mientras (condición) Hacer
    acción 1
    acción 2
Fin Mientras
```

### *Lenguaje C*

```c
while (condicion) {
    accion1;
    accion2;
}
```

### *Ejemplo en C*

```c
int i = 1;
while (i <= 5) {
    printf("%d\n", i);
    i++;
}
```

### *Diagrama de Flujo*

<img width="753" height="562" alt="image" src="https://github.com/user-attachments/assets/62bd2c1d-5c0d-4c33-862a-b0edf959a36f" />

---

## *Ciclo Hacer…Mientras (Do…While)*

>El bloque se ejecuta **al menos una vez**, porque la condición se evalúa al final.

### *Pseudocódigo*

```
Hacer
    acción 1
    acción 2
Mientras (condición)
```

### *Lenguaje C*

```c
do {
    accion1;
    accion2;
} while (condicion);
```

### *Ejemplo en C*

```c
int i = 1;
do {
    printf("%d\n", i);
    i++;
} while (i <= 5);
```

### *Diagrama de Flujo*

<img width="941" height="570" alt="image" src="https://github.com/user-attachments/assets/88996c8f-0589-4bcb-afad-8424eb2b9b07" />


---

## *Ciclo Para (For)*

>Se usa cuando se conoce de antemano el número exacto de repeticiones. El contador se inicializa, verifica y actualiza en una sola línea.

### *Pseudocódigo*

```
Para i ← valor_inicial Hasta límite Con Paso paso Hacer
    acción 1
    acción 2
Fin Para
```

### *Lenguaje C*

```c
for (inicializacion; condicion; incremento) {
    accion1;
    accion2;
}
```

### *Ejemplo en C*

```c
for (int i = 1; i <= 5; i++) {
    printf("%d\n", i);
}
```
### *Diagrama de Flujo*

<img width="672" height="655" alt="image" src="https://github.com/user-attachments/assets/b55b5f74-7062-4da2-8927-9e6a89055ed4" />


---
### [*⬅️ Volver a Unidad 2*](../ContenidosU2.md)

<div align="center">
  <sub>Pablo Namicela &nbsp;·&nbsp; Teoria de la Programación &nbsp;·&nbsp; Universidad Nacional de Loja &nbsp;·&nbsp; 2026</sub>
</div>

---

<div align="center">
  <sub>Facultad de la Energía, las Industrias y los Recursos Naturales No Renovables &nbsp;·&nbsp; Loja, Ecuador &nbsp;·&nbsp; 2026</sub>
</div>
