___
![[Pasted image 20230613092338.png]]
___

# Métodos de análisis sintáctico
___

![[Pasted image 20230613092402.png]]
![[Pasted image 20230613092427.png]]
___

# Problemas en el análisis sintáctico descendente
La recursividad por la izquierda en este caso da lugar a un bucle infinito de recursión. Como no se sabe qué producción elegir se probaría una y si da error se haría un retroceso (Backtracking). Otra alternativa es utilizar algoritmos de eliminación de la recursividad por la izquierda.

## Eliminación de la recursividad por la izquierda
*A→Aα | ß*
- Ordenar las producciones de A en la forma siguiente:
![[Pasted image 20230613092926.png]]
- Reemplazar las producciones de A por:
![[Pasted image 20230613093308.png]]
*Nota:* No olvidar colocar épsilon, puesto ß no necesariamente van concatenados con A'

# Factorización por la izquierda
Una gramática se factoriza por la izquierda cuando dos producciones para un mismo no terminales tienen símbolos comunes por la izquierda.
### Pasos:
- Para cada no terminal, encontrar el prefijo α más largo común.
- Ordenar las producciones.
  ![[Pasted image 20230613093639.png]]
- Reemplazar las producciones de A por:
  ![[Pasted image 20230613093656.png]]
- **Repetir** este proceso hasta que *no existan* producciones con **prefijos comunes**.