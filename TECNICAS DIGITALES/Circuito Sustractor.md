La sustracción de dos números binarios puede lograrse tomando el complemento del sustraendo para agregarlo al minuendo. 

> [!Explicación detallada]
> ## Complemento a dos en la sustracción binaria
>
> La sustracción de dos números binarios se puede realizar mediante el uso del complemento a dos. Este proceso implica tomar el complemento a dos del sustraendo y luego sumarlo al minuendo. A continuación se muestra un ejemplo paso a paso.
>
> Supongamos que queremos restar el número binario `10011` (19 en decimal) del número binario `11010` (26 en decimal). Primero, necesitamos asegurarnos de que ambos números tengan la misma cantidad de bits:
>
> ```
>   11010
> - 10011
> -------
> ```
>
> En este caso, ambos números tienen 5 bits. Ahora, debemos tomar el complemento a dos del sustraendo (`10011`) porque es negativo. Para hacer esto, invertimos cada bit del número (cambiamos los 0 por 1 y los 1 por 0) y luego sumamos 1 al resultado obtenido:
>
> ```
>   10011  (sustraendo original)
>   01100  (complemento a uno del sustraendo)
> + 00001  (suma uno al complemento a uno)
> -------
>   01101  (complemento a dos del sustraendo)
> ```
>El complemento a dos del sustraendo es `01101`. Ahora, podemos sumar el sustraendo (complemento a dos) al minuendo usando la suma binaria normal:
> ```
>   11010  (minuendo)
> + 01101  (complemento a dos del sustraendo)
>-------
>  100111
> ```
>
> Observe que el resultado tiene un bit más que los números originales. Esto se debe a que el bit más significativo (el más a la izquierda) es un acarreo. Debemos descartar este bit adicional y el resultado final es:
>
> ```
>   11010
> - 10011
> -------
>   00101
> ```
> Por lo tanto, la diferencia entre los números binarios `11010` y `10011` es `00101` (5 en decimal).
> Es importante tener en cuenta que, en este ejemplo, el bit más significativo (el más a la izquierda) de los números binarios no se usó para indicar el signo, pero en general, en el sistema binario, se utiliza para ese propósito. Si el bit más significativo es 0, el número es positivo, mientras que si es 1, el número es negativo. En este caso, el bit más significativo del sustraendo (`10011`) es 1, lo que indica que es un número negativo.

---
## Tipos
- [[Circuito Sustractor Medio]]
- [[Circuito Sustractor Completo]]