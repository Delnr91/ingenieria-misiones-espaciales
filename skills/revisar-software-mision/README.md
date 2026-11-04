# Skill · Revisar software de misión

Esta skill ayuda a un asistente a organizar una revisión basada en evidencia. Es un prototipo educativo; no ha sido evaluada con casos independientes y no realiza pruebas automáticamente.

## Uso

En un asistente compatible con Agent Skills, instala la carpeta según la documentación vigente del asistente o comparte su archivo `SKILL.md` como instrucciones. Pide, por ejemplo:

> Revisa este simulador educativo frente a REQ-SW-01. Distingue pruebas presentes y ejecutadas, cita archivos y líneas para los hallazgos, identifica datos faltantes y no modifiques el proyecto.

En Claude, Codex, Gemini y otras herramientas la ubicación, activación y alcance pueden cambiar: comprueba la guía oficial de la herramienta que uses. Compartir el texto con un asistente no garantiza que este siga las instrucciones ni que tenga acceso a los archivos.

## Ejemplo de resultado esperado

Si hay un requisito pero no hay resultados de prueba, la salida debe indicar **no verificado**, no «cumple». Si una prueba existe pero no se ejecutó, debe distinguir ambas cosas. El responsable humano decide qué revisar a continuación.

Consulta la [especificación Agent Skills](https://agentskills.io/specification) para la estructura del archivo. El uso real en misiones exige procesos y revisión adecuados al proyecto.
