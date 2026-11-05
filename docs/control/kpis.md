# Indicadores de control propuestos

Las siguientes son metas académicas y **no mediciones reales**. Para medirlas hace falta un sistema operativo con registros de tickets.

| Indicador | Fórmula | Meta propuesta | Fuente |
|---|---|---|---|
| Tiempo medio de resolución (TMR) | Σ horas desde apertura hasta resolución / tickets resueltos | Menor a 4 horas | Timestamps de tickets |
| Cumplimiento de SLA | Tickets resueltos dentro de plazo / resueltos con SLA × 100 | Mayor a 95 % | Historial y SLA |
| Reapertura | Tickets reabiertos / tickets resueltos × 100 | Menor a 5 % | Historial de estados |

Se requiere definir período, zona horaria, casos duplicados, diferencia entre «resuelto» y «cerrado», y tratamiento del denominador cero. Las metas no deben presentarse como resultados.

## Relación con Entrega 2
El módulo CI/CD se había planificado con estos **objetivos**, no resultados: ejecución de pruebas ≤ 8 minutos, reducción de incidentes ≥ 40 % durante los 30 días posteriores a la implementación, cobertura ≥ 80 % de módulos críticos e implementación en 10 semanas. La gestión de incidentes aporta datos para evaluar la calidad de entregas futuras.