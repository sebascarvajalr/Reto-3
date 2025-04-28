# Reto 3
## Pseudocódigo:
```
Paso 1: Definir n como entero.

Paso 2: Escribir "Ingrese el número límite n:"

Paso 3: Leer n.

Paso 4: Crear una lista de números desde 2 hasta n, marcándolos como primos inicialmente.

Paso 5: Definir p = 2.

Paso 6: Mientras (p * p <= n) hacer:

Paso 6.1: Si p está marcado como primo, entonces:

Paso 6.1.1: Marcar todos los múltiplos de p (desde p * 2 hasta n) como no primos.

Fin

Paso 6.2: Incrementar p en 1.

Fin
```

## Diagrama de flujo:
```mermaid
---
config:
  theme: redux
---
flowchart TD
    A(["Incio"]) --> n1["n: Número límite"] & n4["i = número que se desea verificar"]
    n1 --> n5@{ label: "Lista de números desde <code data-start=\"296\" data-end=\"299\">2</code> hasta <code data-start=\"306\" data-end=\"309\">n</code>" }
    n4 --> n5
    n5 --> n6["Ej: p = 2"]
    n6 --> n7["¿p * p &lt;= n?"]
    n7 --- n8["No"] & n9["Si"]
    n8 --> n11["Fin"]
    n9 --> n13["¿p esta marcado como primo?"]
    n13 --- n15["Si"]
    n15 --> n12["Marcar todos los múltiplos de p como no primos"] & n16["Incrementar p<br>"]
    n16 --> n7
    n1@{ shape: proc}
    n4@{ shape: proc}
    n5@{ shape: proc}
    n6@{ shape: proc}
    n7@{ shape: decision}
    n8@{ shape: text}
    n9@{ shape: text}
    n11@{ shape: rounded}
    n13@{ shape: decision}
    n15@{ shape: text}
    n12@{ shape: proc}
    n16@{ shape: rect}
```
