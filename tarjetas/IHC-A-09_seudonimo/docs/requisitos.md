# Fase 2 · Requisitos verificables — IHC-A-09 · Dashboard UX · Participantes anónimos con código seudónimo

**Responsable:** González Álvarez Vladimir Humberto

| ID | Requisito | Criterio de verificación | Origen |
|---|---|---|---|
| RF-01 | Registrar al participante con un código seudónimo. | El paso 2 tiene «Código de participante». | Fallo de la tarjeta (Issue #9) |
| RF-02 | Registrar resultados por tarea (resultado, errores, tiempo, observaciones). | La tabla agrega filas. | Tarea crítica |
| RF-03 | Mostrar solo el código en tablas, resumen y confirmación. | Ninguna pantalla muestra nombres. | Tarea crítica |
| RF-04 | Finalizar con resumen y código de sesión. | Aparece S-2026-0XX. | Tarea crítica |
| RNF-01 | Privacidad: no solicitar ni almacenar nombres reales. | No existe campo de nombre. | Restricción de la tarjeta |
| RNF-02 | Operable con teclado; errores asociados al campo. | El error usa aria-describedby. | Accesibilidad (WCAG 2.2) |
