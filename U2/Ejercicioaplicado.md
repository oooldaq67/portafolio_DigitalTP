

# Ejercicio con Estructura Condicional y Repetitiva

## 1. Planteamiento del Problema

>Desarrollar un programa en lenguaje C que calcule la nota final de una unidad para un grupo de estudiantes. El programa debe solicitar el número de estudiantes, leer las cuatro notas de cada uno (ACD, AA, APE y ES), validar que cada nota esté entre 0 y 10, calcular la nota ponderada final y mostrar el nivel de desempeño correspondiente.

---

## 2. Análisis del Problema

| Categoría | Variable | Descripción |
|---|---|---|
| Entrada | `ce` | Número total de estudiantes |
| Entrada | `ACD` | Nota de Actividades de Clase y Deberes |
| Entrada | `AA` | Nota de Actividades Autónomas |
| Entrada | `APE` | Nota de Actividades Prácticas y Experimentales |
| Entrada | `ES` | Nota del Examen Sumativo |
| Proceso | `pACD = ACD × 0.20` | Ponderación del ACD |
| Proceso | `pAA = AA × 0.20` | Ponderación del AA |
| Proceso | `pAPE = APE × 0.25` | Ponderación del APE |
| Proceso | `pES = ES × 0.35` | Ponderación del ES |
| Proceso | `notaUnidad = pACD + pAA + pAPE + pES` | Suma de ponderaciones |
| Salida | `notaUnidad` | Nota final de la unidad |
| Salida | Nivel de desempeño | Excelente / Bueno / Regular / Deficiente |

---

## 3. Diagrama de Flujo

<img width="516" height="2011" alt="diagrama_notas drawio" src="https://github.com/user-attachments/assets/63465ade-98d0-46f4-90ec-d85f01ba19d9" />

---

## 4. Codificación (Código Fuente)

```c
int main(){

    // Definir las variables para cada actividad dentro de los ponderados ACD, AA, APE y ES
    float ACD, AA, APE, ES, pACD, pAA, pAPE, pES, notaUnidad;
    int i, ce;

    // Se le pide al usuario que ingrese el número de estudiantes a calcular
    do{
        printf("Ingrese el numero total de estudiantes:");
        scanf("%d", &ce);
    }while(ce<=0);

    // Los datos de entrada serán las calificaciones de cada actividad en su respectivo ponderado
    for(i=1; i<=ce; i++){

        printf("Estudiante %d\n", i);

        do{
            printf("Ingresar nota de ACD: ");
            scanf("%f", &ACD);
            if(ACD<0 || ACD >10){
                printf("ERROR:Ingrese nuevamente nota del ACD\n");
            }
        }while(ACD<0 || ACD>10);

        do{
            printf("Ingresar nota de AA: ");
            scanf("%f", &AA);
            if(AA<0 || AA >10){
                printf("ERROR:Ingrese nuevamente nota del AA\n");
            }
        }while(AA<0 || AA>10);

        do{
            printf("Ingresar nota de APE: ");
            scanf("%f", &APE);
            if(APE<0 || APE >10){
                printf("ERROR:Ingrese nuevamente nota del APE\n");
            }
        }while(APE<0 || APE>10);

        do{
            printf("Ingresar nota de ES: ");
            scanf("%f", &ES);
            if(ES<0 || ES >10){
                printf("ERROR:Ingrese nuevamente nota del ES\n");
            }
        }while(ES<0 || ES>10);

        // Proceso para calcular los ponderados
        pACD= ACD * 0.2;
        pAA=  AA  * 0.2;
        pAPE= APE * 0.25;
        pES=  ES  * 0.35;
        notaUnidad= pACD + pAA + pAPE + pES;

        // Se muestra por pantalla la nota final y el nivel de desempeño
        printf("Su nota final es: %.2f\n", notaUnidad);

        if(notaUnidad >= 9){
            printf("Nivel de desempenio: Excelente\n");
        }
        if(notaUnidad >= 7 && notaUnidad < 9){
            printf("Nivel de desempenio: Bueno\n");
        }
        if(notaUnidad >= 5 && notaUnidad < 7){
            printf("Nivel de desempenio: Regular\n");
        }
        if(notaUnidad < 5){
            printf("Nivel de desempenio: Deficiente\n");
        }
    }

    return 0;
}
```

---

## 5. Validación (Prueba de Escritorio)

**Datos de entrada:** `ce = 1`, `ACD = 10`, `AA = 10`, `APE = 10`, `ES = 10`

| Variable | Operación | Valor |
|---|---|---|
| `pACD` | 10 × 0.20 | 2.00 |
| `pAA` | 10 × 0.20 | 2.00 |
| `pAPE` | 10 × 0.25 | 2.50 |
| `pES` | 10 × 0.35 | 3.50 |
| `notaUnidad` | 2.00 + 2.00 + 2.50 + 3.50 | **10.00** |

**Salida esperada:**
```
Su nota final es: 10.00
Nivel de desempenio: Excelente
```



### [*⬅️ Volver a Unidad 2*](../ContenidosU2.md)

<div align="center">
  <sub>Pablo Namicela &nbsp;·&nbsp; Teoria de la Programación &nbsp;·&nbsp; Universidad Nacional de Loja &nbsp;·&nbsp; 2026</sub>
</div>

---

<div align="center">
  <sub>Facultad de la Energía, las Industrias y los Recursos Naturales No Renovables &nbsp;·&nbsp; Loja, Ecuador &nbsp;·&nbsp; 2026</sub>
</div>
