# Vista gráfica complementaria del proceso

> **Esta vista sirve para lectura rápida y no sustituye la notación BPMN del archivo editable.** El XML BPMN debe abrirse y diagramarse en un modelador antes de presentar la evidencia final.

```mermaid
flowchart LR
  A([Reporte de incidente]) --> B[Registrar y diagnosticar - N1]
  B --> C{¿N1 resuelve?}
  C -- Sí --> D[Solución conocida]
  C -- No --> E[Escalar a N2]
  E --> F[Reproducir y corregir defecto]
  F --> G[Ejecutar QA y CI/CD]
  G --> H{¿Pruebas aprobadas?}
  H -- No --> F
  H -- Sí --> I[Notificar al usuario]
  D --> I
  I --> J{¿Usuario conforme?}
  J -- No / reabrir --> B
  J -- Sí --> K[Cerrar ticket y documentar]
  K --> L([Fin])
```

## Roles
- **Usuario/Cliente:** origina el reporte y valida la resolución.
- **Mesa de ayuda N1:** triaje, diagnóstico, solución conocida y cierre.
- **Soporte N2:** análisis y corrección de defectos.
- **QA y CI/CD:** pruebas y validación de cambios antes de informar solución.

Las decisiones de modelado son propuestas académicas, no pasos ejecutados por un software productivo.
