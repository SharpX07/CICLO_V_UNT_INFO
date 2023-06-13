**Definición:** Herramienta para generar escáneres
**Funcionamiento:** *Lee el fichero* de entrada en una dirección específica o estándar, el cual **contiene** *la descripción de un escáner a generar*. Dicha descripción se encuentra las expresiones regulares y código en C (**REGLAS**).
Flex **genera un fichero** fuente en C, denominado *lexyy.c* que define una rutina de *yylex()*. Dicho **fichero** se *compila y se enlaza* a un **programa principal**, *produciendo* un **ejecutable del reconocedor léxico**.
El reconocedor léxico (fichero ejecutable generado) analiza una entrada en busca de las expresiones regulares. Al encontrar una de estas, ejecuta la acción escrita en C asociada a esta.
![[Pasted image 20230612182746.png]]
# Partes de FLEX
___
```
Definiciones
%%
Reglas
%%
Código de usuario
```
___
# Contenido
- **Declaraciones en C:** Declaración de elementos que se van a utilizar en la especificación del analizador léxico como *estructuras de datos*. Sintaxis:
```
%{
/* Código en C */
%}
```

- **Declaraciones de definiciones regulares o macros:** *Macros* son ***nombres*** que se les da a las *expresiones regulares*. Su objetivo es brindar la capacidad de definir nuevas expresiones mucho más compactas y complejas.
```
nombre definición //Declaración de una macro

// Cómo hacer referencia a una macro anterior
// Macro inicial
digito [0-9]
// Referencia en una nueva macro
numero {digito}+
```

- **Declaración de patrones**: Contiene todos los *patrones* que el ***analizador léxico*** reconocerá en *función* a las macros antes especificadas, *además de las acciones* a realizar en C. El patrón debe estar en una misma línea y sin sangría.
```
patrón acción en C;

// Ejemplo
"int" {std::cout<<"int reservada"<<"\n";}
```

- **Declaración de funciones:** Se encuentra en la última parte del archivo flex. Aquí se llama al escáner y a otras funciones. *Es una sección opcional*. 



