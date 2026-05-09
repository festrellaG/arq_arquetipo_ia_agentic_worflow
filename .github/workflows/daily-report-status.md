---
on:
  workflow_dispatch:
permissions:
      contents: read
      issues: read
      pull-requests: read
engine: copilot
network: defaults
tools:
  github:
    lockdown: false
    min-integrity: none # This workflow is allowed to examine and comment on any issues
    #toolsets: [default]
safe-outputs:
  mentions: false
  allowed-github-references: []
  create-issue:
    title-prefix: "[repo-status] "
    labels: [report, daily-status]
    close-older-issues: true
---

# daily-report-status

# Estado diario del repositorio

Crea un informe de estado diario positivo para el repositorio como una incidencia de GitHub.

## Qué incluir

- Actividad reciente del repositorio (incidencias, solicitudes de extracción, discusiones, lanzamientos, cambios de código)
- Seguimiento del progreso, recordatorios de objetivos y aspectos destacados
- Estado del proyecto y recomendaciones
- Próximos pasos concretos para los mantenedores

## Estilo

- Sé positivo, alentador y útil 🌟
- Usa emojis con moderación para fomentar la interacción
- Sé conciso: ajusta la extensión según la actividad real

## Proceso

1. Recopila la actividad reciente del repositorio
2. Analiza el repositorio, sus incidencias y sus solicitudes de extracción
3. Crea una nueva incidencia de GitHub con tus hallazgos y conclusiones

<!--
## TODO: Customize this workflow

The workflow has been generated based on your selections. Consider adding:

- [ ] More specific instructions for the AI
- [ ] Error handling requirements
- [ ] Output format specifications
- [ ] Integration with other workflows
- [ ] Testing and validation steps

## Configuration Summary

- **Trigger**: Manual trigger
- **AI Engine**: copilot
- **Tools**: github
- **Safe Outputs**: create-issue
- **Network Access**: defaults

## Next Steps

1. Review and customize the workflow content above
2. Remove TODO sections when ready
3. Run `gh aw compile` to generate the GitHub Actions workflow
4. Test the workflow with a manual trigger or appropriate event
-->
