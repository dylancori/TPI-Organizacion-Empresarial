# Proceso BPMN de incidentes integrado con QA y CI/CD

**Participantes**: Usuario/Cliente (pool externo), TechLogix Solutions (pool con lanes Mesa de Ayuda N1, Soporte N2, QA/CI-CD). La separación de pools muestra el intercambio de mensajes; los flujos de secuencia se mantienen dentro del proceso interno.

1. Un usuario informa un incidente.
2. N1 registra, clasifica y diagnostica.
3. Compuerta XOR: si N1 puede resolverlo, aplica solución y notifica; si no, escala a N2.
4. N2 reproduce el defecto y propone corrección. QA ejecuta pruebas y validaciones automatizadas del pipeline CI/CD.
5. Compuerta XOR: si las pruebas fallan, la corrección vuelve a N2; si pasan, se informa al usuario.
6. El usuario valida; una respuesta negativa reabre el ticket y lo devuelve a diagnóstico.
7. Al confirmar conformidad, se cierra el ticket y se documenta el aprendizaje.

**Alcance:** modelo propuesto para un caso ficticio; no representa un sistema ya implementado. El autor debe abrir y validar personalmente el archivo editable BPMN y describir sus decisiones.