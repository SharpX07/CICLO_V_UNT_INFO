#flashcards 
# ¿Qué son los circuitos de codificadores?
---
Son aquellos que :: generan códigos binarios por cada entrada activada.
<!--SR:!2023-05-16,23,290-->
Tiene $2^n$ entradas y cada una corresponde a un código generado en las $n$ salidas que posee.

> [!hint]
> Realmente es sencillo obtener las ecuaciones de un codificador, ya que estas estarán dadas como la suma de las entradas que posean valor 1 en la tabla (si hablamos de un codificador en nivel alto). 
> ### Ejemplo:
> ![[Pasted image 20230509212654.png]]
> 
> Las ecuaciones para la tabla presentada serán:
> $S_1=I_2+I_4+I_6$
> $S_2=I_3$
> $S_3=I_4+I_5+I_6+I_7$

### *Circuito Codificador con pulsadores para las entradas*:
![[Pasted image 20230509222643.png]]
___
## Codificadores Mediante Diodos Rectificadores:
Se puede diseñar una matriz de diodos rectificadores para implementar los codificadores, esto siguiendo reglas sencillas para su armado:
- Graficar una linea horizontal por cada entrada.
- Graficar una linea vertical por cada salida.
- Conectar un diodo que unirá la linea vertical con cada una de las horizontales que conforman la ecuación.
### Ejemplo:
Para un codificador 4x2 se tienen las siguientes ecuaciones:
- $S_0=E_1+E_3$
- $S_1=E_2+E_3$
$S_0$ y $S_1$ son variables de salida, $E_0,E_1,E_2,E_3$ son variables de entrada.
La malla de diodos sería:

![[Pasted image 20230509213446.png]]

___
## Tipos de Codificadores:
Son dos, los que generan códigos con entrada prioritaria y los que generan códigos sin entrada prioritaria.
### Codificadores con prioridad:
Son aquellos que al activar 2 o más entradas, solamente generan un código de salida que responde a una entrada.
Los que generan código con entrada prioritaria se dividen en dos: *Con prioridad ascendente* y *con prioridad descendente*.
- **Prioridad Ascendente**: Son circuitos que permiten activar dos o más entradas generando un código de responde a una tecla pulsada de mayor prioridad.
	- Ejemplo: Si pulsas $S_5$ y $S_7$, el Cto. solo generaría el código 111.
- **Prioridad Descendente**: Son circuitos que permiten activar dos o más entradas generando un código de responde a una tecla pulsada de menor prioridad.
	- Ejemplo: Si pulsas $S_5$ y $S_7$, el Cto. solo generaría el código 101.
---
## Datos Extra:
### Corriente Continua Pulsante
Tenemos una onda senoidal que representa la corriente alterna de una línea, y queremos convertirla a una lineal continua podemos realizarlo mediante un diodo rectificador obteniendo de esta forma una corriente continua pulsante:

![[Pasted image 20230509215704.png]]
El resultado la misma onda pero únicamente con los valores positivos en el eje y.
### Display 7 Segmentos
Es un dispositivo electrónico que permite visualizar números del 0 al 9 mediante segmentos que se iluminan. Existen dos tipos:
- **De cátodo común**: Todos los cátodos se encuentran conectados a tierra, por lo que para activarlo se requieren entradas con valor 1.
- **De ánodo común**: Todos los ánodos se encuentran conectados a 5 voltios, por lo que para activarlo se requieren entradas con valor 0 (tierra).

Esquema de un Display 7 segmentos:

![[Pasted image 20230509220437.png]]