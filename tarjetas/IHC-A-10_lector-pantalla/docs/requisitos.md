# Fase 2 · Requisitos verificables — IHC-A-10 · Dashboard UX · Stepper y checklist con lector de pantalla

**Responsable:** Vinces Cueva Boris Yussef

| ID | Requisito | Criterio de verificación | Origen |
|---|---|---|---|
| RF-01 | Indicar el paso actual con texto y número, no solo color. | «Paso 2 de 5 · Participante» visible. | Fallo de la tarjeta (Issue #10) |
| RF-02 | Marcar pasos completados con ✓ y texto oculto «completado». | El lector lee «Plan… (completado)». | Tarea crítica |
| RF-03 | Checklist con progreso anunciado («n de 5 listos»). | El contador cambia al marcar. | Tarea crítica |
| RF-04 | Mensajes de error y éxito anunciados. | role="alert" / role="status". | Restricción de la tarjeta |
| RNF-01 | Información no transmitida solo por color (WCAG 1.4.1). | La vista en grises conserva el significado. | Tarea crítica |
| RNF-02 | Operable con teclado y lector (NVDA). | Toda la tarea con Tab/Espacio/Enter. | Accesibilidad (WCAG 2.2) |
| **RF-07** | **Paso activo con `aria-current="step"`, anuncio «Paso n de 5: Nombre» en cada cambio y foco visible de 3 px.** | NVDA lee «Participante, paso actual»; el anillo de foco es visible. | Incidencia sorpresa |

## Cambio por la incidencia
«Añadir texto/estado accesible del paso activo y foco visible» → se agregó **RF-07**. Flujo actualizado en `diagramas/user-flow.png` (nodos en naranja).
