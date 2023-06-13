# Agentes basados en búsqueda
___
- Mantienen un **modelo simbólico** del mundo.
- Modifican el **estado del mundo** de acuerdo a sus  **objetivos** *(estado meta)*.
- **Anticipan** los efectos esperados de sus acciones sobre el **estado del mundo**.
___

# Entorno: **problemas** bien definidos
___
## Discreto
- Se puede **concebir el** **mundo en estados**.
- En cada **estado** hay un **conjunto finito de acciones** y percepciones.

## Accesible
El agente accede a las *características relevantes del mundo*, como las siguientes:
- El **agente** puede **determinar** el **estado actual del mundo**.
- El **agente** puede **determinar el estado del mundo** que le **gustaría alcanzar**.

## Estático y Determinista
El *agente planifica todas sus acciones*, puesto que:
- El mundo **cambia** cuando el agente interactúa.
- El **resultado** de cada acción es **previsible** y se puede **definir**.