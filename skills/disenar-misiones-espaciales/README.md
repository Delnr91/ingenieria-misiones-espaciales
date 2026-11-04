# 🛠️ Skill de diseño de misiones espaciales

[Inicio](../../README.md) · [Instrucciones](SKILL.md) · [Fuentes](references/fuentes.md)

Esta skill orienta a un asistente para ayudar a formular un concepto educativo de misión espacial, identificar requisitos, alternativas, interfaces, riesgos y evidencia faltante. **Es una primera versión sin prueba de funcionamiento independiente ni validación para vuelo.**

## Instalar

Copia la carpeta completa `disenar-misiones-espaciales`, incluida `references`, a la ubicación que utilice tu asistente:

- **Codex:** `~/.codex/skills/`, para uso personal; inicia una sesión nueva.
- **Claude Code:** `~/.claude/skills/` para uso personal o `.claude/skills/` para el proyecto.
- **Gemini CLI:** `.agents/skills/` dentro del proyecto; comprueba con `/skills list`.
- **GitHub Copilot:** `.github/skills/` dentro del proyecto, para las modalidades de agente compatibles.

Consulta las instrucciones oficiales de [Claude Code](https://code.claude.com/docs/en/skills), [Gemini CLI](https://geminicli.com/docs/cli/skills/) y [GitHub Copilot](https://docs.github.com/en/copilot/how-tos/copilot-on-github/customize-copilot/customize-cloud-agent/add-skills). Estas rutas se presentan como orientación documental: no se ha probado la instalación o activación en esas herramientas para esta skill.

## Primer uso

> Usa la skill `disenar-misiones-espaciales` para ayudarme a formular un concepto ficticio de observación terrestre. Distingue objetivos, requisitos, supuestos, interfaces y lo que falta comprobar. No ejecutes ni publiques nada.

Revisa la respuesta y sus fuentes. Una propuesta con apariencia técnica no es evidencia de que un sistema pueda operar.

## Diseño y evaluación

La carpeta sigue el formato de [Agent Skills](https://agentskills.io/specification). Se mantiene una entrada breve y una referencia separada; las [buenas prácticas](https://agentskills.io/skill-creation/best-practices) recomiendan contrastar la skill con tareas reales y mejorarla con los resultados. Esa evaluación sigue pendiente.
