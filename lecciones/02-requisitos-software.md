# Lección 2 · Del objetivo de una misión a los requisitos de software

**Origen:** material original basado en las guías públicas de NASA citadas al final. No es una traducción ni un resumen del capítulo 2 de SMAD.

## Objetivos

Al terminar podrás distinguir necesidad, requisito, evidencia y decisión; escribir un requisito verificable para un ejemplo ficticio y detectar cuándo una prueba no demuestra que se cumple.

## El recorrido

Necesidad → objetivo de misión → requisito de sistema → requisito de software → prueba → evidencia → revisión humana.

Las flechas indican trazabilidad, no una secuencia irreversible. Una prueba o un cambio en la necesidad puede obligar a revisar decisiones anteriores.

**Necesidad:** una persona quiere saber cuándo existen datos utilizables de un instrumento. **Objetivo:** facilitar que el equipo encuentre los datos generados durante una sesión. **Requisito:** define una condición concreta que un producto debe satisfacer. **Evidencia:** es el resultado registrado de una comprobación, junto con sus condiciones y versión.

## Ejemplo educativo: simulador de un satélite

La misión y todos los valores son ficticios. Un programa recibe mediciones simuladas, registra sus fechas y permite consultarlas. Considera este requisito propuesto:

> REQ-SW-01: Al recibir una medición simulada válida, el programa guardará su identificador y fecha UTC; al buscar por ese identificador devolverá ambos campos en la respuesta.

Condición: existe una medición válida con identificador y fecha UTC. Método: prueba automatizada en un entorno definido. Criterio: los dos campos devueltos coinciden con los introducidos. Evidencia: versión del código, datos ficticios de entrada, registro y resultado de la prueba. La persona responsable revisa también identificadores repetidos, campos ausentes y formatos de fecha incorrectos.

La prueba positiva no demuestra por sí sola que todos los casos límite estén resueltos, que los datos sean reales o que el sistema esté listo para vuelo.

## Verificar y validar

- **Verificar:** comprobar si el producto satisface un requisito especificado.
- **Validar:** evaluar si el producto resulta adecuado para la necesidad prevista, en el contexto pertinente.

Puede verificarse que un programa guarda fechas y, aun así, no satisfacer a sus usuarios si la información no llega cuando la necesitan. Revisión, análisis, demostración y prueba son métodos posibles; el método apropiado depende del requisito y contexto.

## Matriz mínima de trazabilidad

| Necesidad | Requisito | Comprobación | Evidencia | Estado |
|---|---|---|---|---|
| Consultar una medición simulada | REQ-SW-01 | Entrada válida y consulta | Registro de prueba y versión | Pendiente de ejecutar |
| Evitar ambigüedad por duplicados | Por definir | Por definir | No disponible | Pendiente |

**No confundas «pendiente» con «aprobado».** Una skill puede ayudar a buscar información faltante, pero no sustituye la ejecución de pruebas ni la aceptación responsable.

## Actividad

1. Escribe una necesidad de un simulador educativo de misión.
2. Formula un requisito que indique condición y comportamiento observable.
3. Propón un caso normal y uno de error, especificando resultados esperados.
4. Indica qué archivo o registro serviría como evidencia y quién lo revisaría.

<details><summary>Ejemplo de revisión</summary>

«El software funcionará bien» no es suficientemente preciso para comprobarse. En cambio, la respuesta a un dato de entrada concreto puede describirse y verificarse; todavía debe revisarse si esa conducta satisface la necesidad del usuario.

</details>

## Guion breve para escuchar

Un requisito describe lo que un sistema debe hacer en condiciones concretas. Para comprobarlo necesitamos un método y evidencia. En un simulador, podemos introducir una medición ficticia y comprobar que se guarda y recupera correctamente. Un resultado aislado no demuestra que todos los casos funcionen. Una persona revisa los límites, las pruebas y las decisiones.

El texto anterior puede leerse con la función de voz del dispositivo. No se ha generado un archivo de audio para esta lección.

## Fuentes

- NASA, [Fundamentos de ingeniería de sistemas](https://www.nasa.gov/reference/2-0-fundamentals-of-systems-engineering/).
- NASA, [Análisis de requisitos de software, SWE-051](https://swehb.nasa.gov/spaces/SWEHBVD/pages/102695426/SWE-051%2B-%2BSoftware%2BRequirements%2BAnalysis).
- NASA, [Validación de requisitos, SWE-055](https://swehb.nasa.gov/spaces/SWEHBVD/pages/102695440/SWE-055%2B-%2BRequirements%2BValidation).

Fuentes consultadas el 4 de noviembre de 2026. Estas guías no convierten el ejemplo en un proyecto NASA ni establecen cumplimiento normativo.
