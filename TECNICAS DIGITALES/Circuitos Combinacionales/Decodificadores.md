#flashcards 
# ¿Qué son los circuitos de decodificadores?
---
Los circuitos de decodificadores son aquellos que :: por cada código de entrada activan una salida o varias.
<!--SR:!2023-05-16,23,290-->
Al tratarse de un circuito combinacional, este convierte la información binaria en lineas de entrada a un máximo de $2^n$ líneas de salida.

> [!important]
> Si la información decodificada de $n$ bits tiene combinaciones no usadas o de no importa, la salida del decodificador tendrá menos de $2^n$ salidas.

___
## Grupos de decodificadores

Estos se clasifican en dos grandes grupos:
1. Los que generan una sola salida por cada combinación de entrada. [[Decodificadores de una salida por combinación]]
2. Los que generan varias salidas por cada combinación de las entradas.