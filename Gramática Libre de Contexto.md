La estructura sintáctica de los lenguajes de programación se especifica mediante **gramáticas libre de contexto**, los cuales son la base con la cual se realizan otros esquemas de traducción en la etapa de análisis sintáctico.
___
Contiene: Símbolos no terminales, terminales, símbolo inicial y producciones (Reglas).
- **Símbolos Terminales:** Son las cadenas básicas (if, else, +, -, etc.) o los tokens.
- **Símbolos no Terminales:** Variables sintácticas que denotan un conjunto de cadena (ej. declaración de la estructura de un condicional tiene una combinación de bastantes cadenas). Forman parte fundamental del análisis sintáctico.
- **Símbolo inicial:** Símbolo no terminal.
- **Producciones:** Especifica como los símbolos terminales y no terminales están dispuestos en la gramática (Indican el orden de estos y el cómo se expandirían - Reglas Gramaticales).

![[Pasted image 20230613083334.png]]
# Convenciones
- Letras griegas representan un conjunto de terminales y no terminales.
- Un conjunto de símbolos terminales se puede representar por medio de una letra minúscula. Las cadenas en negrita como: **if** y **else**.
- Un conjunto de símbolos no terminales se puede representar por medio de una letra mayúscula, donde *S* denota al *símbolo inicial*. Las cadenas se escriben en cursiva como: *expresion*, y *statement*.
- X, Y, Z representan símbolos gramaticales (terminales y no terminales). 
- u, v, x, y, z representan cadenas de terminales.

# Derivaciones
Regla de producción de una GLC:
*E → E + E | E * E | - E | (E) | id*
- **Derivación:**
*E → - E → - (E) → -(id)*
- **Forma Sentencial:**
![[Pasted image 20230613084901.png]]
- **Sentencia:**
Forma sentencial con tan solo símbolos terminales. También, es una cadena generada a partir de una gramática, en este caso, una GLC.
Ejemplo:
Sentencia → *-(id+id)*, porque existe una derivación que llega a esta cadena.
- **Tipos:** Por la izquierda (lm) y por la derecha (rm).

# Notación de las producciones
![[Pasted image 20230613085410.png]]
*Nota:* N es el conjunto de no terminales. El otro conjunto es el de los símbolos terminales o tokens.

# Gramática Ambigua
- Se da cuando el lenguaje que genera la gramática contiene **una o más sentencias** las cuales tienes más de un [[Árbol de Análisis Sintáctico]].
- **No** existe ni *metodología para eliminar* la ambigüedad ni tampoco *fórmula para detectarla*.
- Se rediseñan para encontrar una gramática equivalente no ambigua.
Ejemplo:
![[Pasted image 20230613090339.png]]

# Diseño de gramáticas
## Recursividad
- Recursividad por la izquierda: *A→Aß*
- Recursividad por la derecha: *A→ßA*
## Asociatividad
La **asociatividad de un operador por la izquierda** *requiere* que en las **reglas de producción** en las que interviene dicho operador, tengan **recursividad por la izquierda**. Lo mismo aplica para la recursividad por la derecha.
## Precendencia
- Se utiliza un **símbolo no terminal** por cada **operador de distinta precedencia**.
- Mientras más cerca esté al símbolo inicial, el operador será de menor precedencia.
## Parentización
- Tienen máxima precedencia.
- Se debe **añadir un símbolo no terminal** que produzca expresiones entre paréntesis que esté a la **mayor distancia del símbolo inicial** (de esta manera alcanza la máxima precedencia).
