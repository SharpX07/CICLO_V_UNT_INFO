# Planteamiento inicial del problema
## Objetivo
- Trasladar los discos de la aguja A a B en el mismo orden
## Reestricción
- Un disco mayor nunca debe reposar sobre uno de menor tamaño.

# Soluciones
## Solución 1: tablas de actuación
- Para **cada situación hay una entrada** en una **tabla de actuación**.
- La entrada es la secuencia de acciones a emprender.
![[Pasted image 20230514004158.png]]
- **Flexibilidad:** Permite *aprender* nuevas entradas.
- **Problema:** *Límitaciones* de memoria.

## Solución 2: Algoritmo
- El programador **(diseñador del agente)** conoce un *método para resolver* el problema **(algoritmo)**.
- *Codifica* el método en un algoritmo.
- **Flexibilidad:** parametriza el algoritmo.
- **Problema:** el diseñador debe *anticipar* todos los *escenarios posibles*. Los *problemas reales* suelen ser complejos de *anticipar*.

## Solución 3: Búsqueda
![[Pasted image 20230514010201.png]]

- Se desarrolla e implementa un algoritmo de búsqueda, puesto que este es capaz de *generar una solución a cualquier problema representado mediante el modelo simbólico*.
- **Flexibilidad:** El diseñador *no necesita* conocer la solución. Es *más fácil de adaptar* a nuevas características.
