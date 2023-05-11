A continuación se mostrará cómo es un circuito decodificador que representa codigos binarios con 4 salidas. En este caso al tener 2 entradas y 4 salidas, se le denominará 2x4 ($[N°entradas]\times[N°salidas]$) .
### Tabla de verdad:
![[Pasted image 20230417230400.png]]
### Circuito:
![[Pasted image 20230417225545.png]]
### Ecuaciones:
1. $S0=A'B'$
2. $S1=AB'$
3. $S2=A'B$
4. $S3=AB$
---
# Decodificador BCD
Dispone de 4 entradas (E0, E1, E2, E3) por las que recibe el código BCD y 10 salidas que representan los posibles valores decimales correspondientes a los códigos de entrada. 

> [!important]
> El número de salidas N debe ser igual o menor que $2^n$, siendo n, el número de entradas, es decir, $N\leq2^n$.

### Tabla de verdad:
![[Pasted image 20230417231353.png]]

---
# Decodificador con salidas de nivel bajo
Los valores de salida activos cuentan como sálida en alto (1), y con salida en nivel bajo deben ser (0). La tabla del decodificador BCD es un ejemplo de decodificador con salidas en nivel alto.