# Pasos para la codificación manual
1. Identificar tokens (Realizar expresiones regulares).
2. Construir un *AFD* para cada token.
3. Construir un *AFD* para el Lenguaje de Programación.
4. Programar lo anterior.
# Ejemplo
**1. Tokens**
```
Identificador : letra(letra/digito)*
Entero : Digito+
Asignación : :=
Mas : +
Por : *
Paréntesis Izq. : (
Paréntesis Der. : )
Punto y coma : ;
```

**2. AFD de los tokens**
![[Pasted image 20230612195956.png]]

**3. AFD del Lenguaje de Programación**
![[Pasted image 20230612200041.png]]

# Reconocimiento de palabras reservadas e identificadores
**Primera Solución:** Ubicar las palabras reservadas en la tabla de símbolos (*estas han sido previamente ubicadas*) e indicar el token que representan. Luego todo lo que venga después será identificador.
![[Pasted image 20230612200505.png]]

**Segunda Solución:** Crear diagramas de transición para cada palabra reservada.
![[Pasted image 20230612200441.png]]
