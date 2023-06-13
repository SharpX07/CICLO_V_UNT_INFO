# Operadores y Expresiones Regulares
**Operadores para las expresiones regulares:**
" [ ] ^ - ? . * + | ( ) $ / { } % < > \
*Nota:* Si estos se quieren emplear como símbolo se antepone "\" al operador o encerrarlo entre comillas dobles.
**Los patrones** se especifican utilizando un conjunto extendido de expresiones regulares.
![[Pasted image 20230612192201.png]]
![[Pasted image 20230612192242.png]]
![[Pasted image 20230612192249.png]]


# Acciones
Recordar: 
```
patrón acción;
```
___
## Acciones Simples
Pueden ser:
- **";"** → Acción a ejecutar al identificar un caracter.
- **"|"** → ?
- **Acción especial**
- **Sentencia en C**
## Acciones Compuestas
- Lista de acciones simples. Estas se encuentra encerradas **{y}**.
## Acciones Por Defecto
- Caracteres reconocidos → Ninguna acción.
- Caracteres no reconocidos → Los copia en el fichero de salida.
