Se da cuando la secuencia de tokens no es reconocida por la gramática del lenguaje. 
Se debe indicar:
- Posición del error (archivo, línea y caracter).
- Mensaje de error al usuario.
- Reanudar el proceso de análisis.

# Mecanismos de recuperación de errores
___
- Ignorar problema (**Modo Pánico**).
- Recuperación a nivel de frase.
- Producciones de error.
___
## Modo Pánico
Consiste en leer tokens de la entrada hasta encontrar un token que especial que permita reconocer un error en una línea anterior. Estos tokens especiales se encuentran usualmente al final de la sentencia.
![[Pasted image 20230613091842.png]]
## Recuperación a nivel de frase
Consiste en realizar **algún tipo de corrección local en la sentencia** para así continuar con el análisis. Esto es difícil, puesto que el *espacio de búsqueda en el árbol de derivación es infinito*, por lo que predecir un token en específico se vuelve **muy complicado**.
## Producciones de errores
Consiste en *agregar* a la gramática del lenguaje de programación **producciones de errores comunes** para que se genere un árbol sintáctico asociado.

